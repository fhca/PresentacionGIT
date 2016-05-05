rdenar:


```
$ git add <archivo>

$ git diff
muestra las líneas exactas que fueron añadidas/elimiadas/modificadas

$ git commit
confirma los cambios preparados (lo que está en stagin 
area)
-a # add y commit en una sóla línea (agrega a staging todos los archivos tracked)
-m "<mensaje>"
-v # muestra las diferencias introducidas en éste commit.
--amend #corrige el mensaje del commit (justo después de haber hecho el commit)

$ git rm <archivo>
--cached

$ git mv <nombreActual> <nombreNuevo>
también se puede hacer con otra erramienta externa, por ejemplo CLI o GUI

$ git log
Historial de commits. En orden cronológico inverso. Muestra el SHA1, identida del autor, fecha, hora y mensaje del commit.
-p #muestra las diferencias introducidas en cada commit.
-3 #muestra los últimos 3 commits.
--stat #muestra estadísticas
--pretty [oneline, short, full, fuller, formar...
--graph
--since=[2.weeks]ó[2016-5-1]
--until
etc...

$ git diff #diferencia entre versiones de archivos en staged y local unstaged.
--cached #diferencias entre lo que haz preparado hasta ahora.
TODO: probar los comandos de arriba.

$ git reset HEAD <archivo> 
Quita el archivo del area de preparación y de tracked, pero mantiene en el directorio de trabajo.

$ git remote
Muestra nombre (alias) de remotos especificados.
-v #muestra los alias y la URL asociada a cada uno.
git remote add <nombre> <URL> 

$ git

$ git
$ git


```


