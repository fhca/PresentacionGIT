#Workflows - Flujos de trabajo

##Revisión de comandos básicos
* add / commit / status / log

##add
* `git add archivo` agrega el archivo a la lista de *rastreados* (tracked) y los *prepara*, o sea, copia su contenido al *área de preparación* (staged).
* `git status` muestra el estado de los archivos, aparecen archivos no rastreados (untracked), añadidos (new file), etc.
* `git rm -f archivos` borra archivos del directorio de trabajo, del rastreo y del área de preparación.
* `rm archivos` borra archivos del directorio actual, más no del área de preparación.
* `git rm --cached` borra archivos preparados, pero los mantiene en el directorio de trabajo (y en la lista de rastreados)
* `git reset HEAD archivo` borra el archivo del área de preparación y de la lista de rastreo (sin borrarlo del directorio de trabajo)
* `git checkout -- archivos` recupera archivos desde el área de preparación hacia el directorio de trabajo (la versión de la última vez que se les hizo "add", véase *commit* para recuperar cualquier versión anterior), siempre y cuando se estén rastreando y por alguna razón se hayan borrado (por ejemplo, mediante `rm` de Unix), o modificado (por ejemplo, con un editor o IDE).
* `git diff` muestra la diferencia (interna) entre los archivos en el directorio de trabajo y los archivos preparados.

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
A la etapa anterior se le llama *preparación* del proyecto y sus archivos, el paso siguiente en el control de versiones es la *confirmación* (commit).

* `git commit archivos` para transferir archivos del área de preparación al área de confirmación. Esto abre el editor del sistema git, que se puede definir con `git config --global core.editor`.
* `git commit -a -m "msg"` como antes de confirmar, hay que actualizar el área de preparación añadiéndole los archivos rastreados modificados, esto hace las dos operaciones en una sola instrucción. Con la opción `-m "msg"` permite agregar un texto descriptivo sin abrir el editor.
* `git diff --staged` muestra las diferencias (internas) entre archivos preparados y archivos confirmados (sinónimo de `git diff --cached`).
* `git log` muestra el historial de las confirmaciones
* *`git log -p -2` muestra las diferencias (internas) de las últimas dos confirmaciones.
* `git commit --amend` confirma de nuevo el área preparada (posiblemente actualizada) o permite modificar el msg, sin registrar un commit extra.
* 


* revisar una versión anterior
* regresarse a una versión anterior
* revisar diferencias entre commits
