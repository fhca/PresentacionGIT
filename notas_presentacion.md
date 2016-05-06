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
- Repositorio local - Archivos del sistema git almacenados en el directorio de trabajo.
- Repositorio remoto - repositorio que no es local.
- Stagin area - area de preparación.
- Commited / commited - confirmado.
- Tracked - rastreado.
- Untracked - no rastreado.
- Branch - rama.