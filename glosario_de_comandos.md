# Glosario comandos comunes.

```

	______________________ Ayuda ____________________________
git
	# muestra ayuda muy básica por donde comenzar.
git help <verb>
git <verb> --help
man git-<verb>

	______________________ Configuración ____________________
git config [--global] user.name "NombreUsuario"
	# configura el nombre de usuario para la cuenta tipo unix activa.
    
git config [--global] user.email "correo@dominio.com”
	# configura el correo electrónico para la cuenta tipo unix activa.
    
git config --global core.editor "editor"
	# cambia el editor por defecto que se lanza cada que git necesita que edites un archivo.
    
git config –list
	# lista el estado de las variables de configuración.


	______________________  ____________________
git clone <url.git>
	# hace una copia (regularmente local) de un repositorio (recularmente remoto)

git add <archivo>
	# agrega <archivo> a staging area

git commit
    # confirma los cambios preparados (lo que está en stagin 
area)

git commit -a 
    # add y commit en una sóla línea (agrega a staging todos los archivos tracked)
    
git commit -m "<mensaje>"
	# pasa los archivos de staging a repository

git commit -v 
    # muestra las diferencias introducidas en éste commit.
    
git commit --amend 
    # corrige el mensaje del commit (si se ejecuta justo después de haber hecho el commit)

git rm <archivo>
    # 
    
git rm --cached
    # 

git mv <nombreActual> <nombreNuevo>
    # mueve/renombra un archivo
    # también se puede hacer con otra erramienta externa, por ejemplo CLI o GUI

	______________________ Log ____________________
git log
    # Historial de commits. En orden cronológico inverso. Muestra el SHA1, identida del autor, fecha, hora y mensaje del commit.
    
git log -p 
    # muestra las diferencias introducidas en cada commit.
    
git log -3 
    # muestra los últimos 3 commits.
    
git log --oneline 
    # muestra cada confirmación en una sóla línea.
    
git log --stat 
    # muestra estadísticas
    
git log --pretty [oneline, short, full, fuller, format...

git log --graph

git log --decorate

git log --oneline

git log --all

git log --grep <texto> 
    # busca <texto> en los mensajes de las confirmaciones.

git log --since=[2.weeks]ó[2016-5-1]

git log --until

git log --oneline --graph --color —decorate 
	# la forma mas bonita / completa de historial
etc...

	______________________  ____________________
git diff 
    # diferencias entre working directory y staging area
    
git diff —staged 
    # diferencias entre area de preparación y repositorio (lo último que se confirmó)


git reset HEAD <archivo> 
    # Quita el archivo del area de preparación y de tracked, pero mantiene en el directorio de trabajo.


git remote
    # Muestra nombre (alias) de remotos especificados.
git remote -v 
    # muestra los alias y la URL asociada a cada uno.
git remote add <alias> <URL> 
    # Agrega el remoto que pertenece a <URL> y le asigna el nombre <alias>
git remote show <alias> 
    # Inspecciona remoto. Muestra su información, qué ramas se están usando en local, en remoto, a donde van los push, de donde vienen los pull, etc.
git remote rename <alias-actual> <alias-futuro> 
    # Asigna un nuevo alias a un remoto.
git remote rm <alias> 
    # elimina el remote <alias>


git fetch <alias> 
    # 'Trae' los datos que aún no se tengan de <alias> a local.
git fetch —all
	# trae cambios de todos los servidores. No modifica el directorio de trabajo. (se tiene los datos actualizados al momento)


git pull
	# 'Trae' datos e intenta mezclarlos con local.
	# fetch y merge en un sólo paso. (identifica a qué servidor y qué rama remota está siguiendo la rama actual)
	

git push
    # Envía todos los commits que se hayan echo. (hay que tener permisos de escritura)
git push <nombre-remoto> <nombre-rama> 
    # Especifica el remoto y rama donde se enviaran las confirmaciones.
git push —delete <nombreRama>
    # elimina la rama <nombreRama> del servidor.
git push -u <nombreRemoto> <nombreRama>
    # 

git tag 
    # lista etiquetas en orden alfabético.
git tag -l 'v1.2.3' 
    # etiqueta ligera
git tag -a 'v1.2.3' 
    # etiqueta anotada. (Las etiquetas anotadas guardan más información, apuntan a una confirmación)
git tag -a 'v1.2.3' -m 'mensaje 


git status
    # muestra el estado en el repositorio local. Los archivos rastreados, modificados y el area de preparación.
git status -s 
    # lo muestra en versión reducida.
git status -b 
    # muestra el nombre de la rama activa.


git checkout -b <ramaLocal> <nombreRemoto/nombreRama> 
	# ó
git checkout —track <nombreRemoto/nombreRama>
	# te dá una rama local <ramaLocal> en la que puedes trabajar. Es decir convierte a <RamaLocal> en una rama de seguimiento.
git checkout -b <nombreRama>
	#crea y se cambia a nombreRama en una línea:

	______________________  ____________________
git branch <nombreRama>
	# crea rama con el nombre <nombreRama>
git branch -m <nombreViejo> <nombreNuevo>
	# cambia nombre de rama
git branch -d <nombreRama>
	# elimina rama <nombreRama>
git branch -D <nombreRama>
	# fuerza eliminar <nombreRama> (en caso de que no te deje con -d porque hay cambios que no han sido fusionados)
git branch -v 
	# ver última confirmación en cada rama.
git branch —merged
	# ver ramas fusionadas en rama activa. ( el * significa que su contenido no ha sido incorporado a otras ramas )
git branch —no-merged
	# ver ramas que no han sido fusionadas.
git branch -u <nombreRemoto/nombreRama>
	# ó
git branch ---set-upstream-to <nombreRemoto/nombreRama>
	# asigna rama local a una rama remota
git branch -vv
	# ver remotos de seguimiento.
git branch -h
	# ayuda sobre ramas


git merge <nombreRama> 
	# mezcla la rama <nombreRama> con la rama actual.

git config --global alias.<alias> '<comando>'
	# Crea alias. Ejecutar $git alias será como ejecutar $git <comando>
git config --global alias.visual '!<comando>'
	# Sirve igual pero <comando> es un comando externo a git
	












```
