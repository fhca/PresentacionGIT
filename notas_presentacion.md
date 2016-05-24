#Taller de GIT
##Instalación
###Fedora
sudo yum install git-all
###Debian
sudo apt-get install git-all
###OSX
* https://git-scm.com/download/mac
* http://brew.sh

###Windows
https://git-scm.com/download/win

##Configuración inicial
Nombre y correo

	$ git config --global user.name "John Doe"	$ git config --global user.email johndoe@example.com

editor default (editor default del sistema, ej. vi)

	$ git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -no

Revisando los ajustes

```
$ git config --list
user.name=John Doe
user.email=johndoe@example.com
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
...
```

Ayuda

	$ git help config
	
----
##Notas:
- No se depende de una conexión a la red para trabajar con git.
- En git todo es identificado por checksum.
- Todo commit es una copia instantanea de todo el respositorio.
- Todo commit es recuperable, incluso después de `--amend` o desde ramas eliminadas.
- Por las dos razones anteriores no se recomienda guardar información sensible (por ejemplo contraseñas).

##Glosario:
- Commit - Confirmación - Cada confirmación es una copia puntual de los archivos como se encuentran en ese momento. Guarda; autor, confirmador, mensaje de confirmación, apuntador a confirmación padre (anterior) y el checksum.
- Local - Repositorio local - Archivos del sistema git almacenados en el directorio de trabajo.
- Remoto - Repositorio remoto - repositorio que no es local.
- Stagin area - area de preparación.
- Commited / commited - confirmado.
- Tracked - rastreado.
- Untracked - no rastreado.
- Branch - rama.
- Pull - 
- Push - 
- WIP - work in progress, se usa en los merge request
- Blob - copia de un archivo almacenado en el repositorio. Sucede al preparar un archivo.
- Head - Apuntador a la última confirmación de la rama que se encuentra activa.
- Tracking branch - rama de seguimiento - así al hacer pull por ejemplo Git sabe donde hacer el fetch y el merge.
- ahead - adelantada - por ejemplo una rama adelantada por 2 , tiene 2 confirmaciones que no han sido enviadas a las demás.
- behind - atrasada 
- puntual branch - rama puntual - rama que es creada con un propósito puntual y eliminada una vez cumplido su prpopósito. Por ejemplo: se detecta un pequeño defecto en la rama de producción, se crea la rama 'correccion' para parchar el defecto, una vez corregido se mezcla dicha rama con la rama de producción y se elimina la rama 'correccion'.
- long term branch - rama de larga duración - ramas que tienen una larga vida. Regularmente son casi tan largas como la rama master (o de producción).
- fork - bifurcación 
- origin - es el alias que git le da a la primer rama remota que se da de alta.
- hook - gancho - un script que se ejecuta cada que sucede cierta acción a la que está ligado.