#Workflows - Flujos de trabajo

##Revisión de comandos básicos
* add / commit / status / log

##add
* `git add archivo` agrega el archivo a la lista de *rastreados* (tracking) y copia su contenido al *área de preparación* (staging).
* `git status` muestra el estado de los archivos, aparecen archivos no rastreados (untracked), añadidos (new file), etc.
* `git rm -f archivos` borra archivos del directorio de trabajo, del rastreo y del área de preparación.
* `rm archivos` borra archivos del directorio actual, más no del área de preparación.
* `git rm --cached` borra archivos del área de preparación, pero los mantiene en el directorio de trabajo (y en la lista de rastreados)
* `git reset HEAD archivo` quita el archivo del área de preparación y de la lista de rastreo (sin borrarlo del directorio de trabajo)
* `git checkout -- archivos` recupera archivos desde el área de preparación hacia el directorio de trabajo (la versión de la última vez que se les hizo "add", véase *commit* para recuperar cualquier versión anterior), siempre y cuando se estén rastreando y por alguna razón se hayan borrado (por ejemplo, mediante `rm` de Unix), o modificado (por ejemplo, con un editor o IDE).

###Workflows:

* Recuperación de archivos borrados
	* crea un archivo.
	(Nota: si en este momento lo borras, no habrá forma de recuperarlo)
	* dale `git add archivo` para agregarlo al área de preparación.
	* bórralo con `rm archivo`
	* recupéralo con `git checkout -- archivo`
	* bórralo definitivamente con `git rm -f archivo`
* Recuperación de la versión "anterior" del archivo
	* crea un archivo. (Nota: si en este momento lo modificas, sólo dependes del editor o IDE para recuperar una versión anterior)
	* dale `git add archivo` para agregarlo al área de preparación.
	* modifícalo con un editor.
	* recupéralo con `git checkout -- archivo`

##commit
* revisar una versión anterior
* regresarse a una versión anterior
* revisar diferencias entre commits
