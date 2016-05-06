#Glosario comandos comunes.

```
$ git add <archivo>
```
```
$ git diff
```
muestra las líneas exactas que fueron añadidas/elimiadas/modificadas

```
$ git commit
```
confirma los cambios preparados (lo que está en stagin 
area)

- -a # add y commit en una sóla línea (agrega a staging todos los archivos tracked)
- -m "<mensaje>"
- -v # muestra las diferencias introducidas en éste commit.
--amend #corrige el mensaje del commit (justo después de haber hecho el commit)

```
$ git rm <archivo>
```
--cached

```
$ git mv <nombreActual> <nombreNuevo>
también se puede hacer con otra erramienta externa, por ejemplo CLI o GUI

```
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

```
$ git diff #diferencia entre versiones de archivos en staged y local unstaged.
--cached #diferencias entre lo que haz preparado hasta ahora.
TODO: probar los comandos de arriba.

```
$ git reset HEAD <archivo> 
Quita el archivo del area de preparación y de tracked, pero mantiene en el directorio de trabajo.

```
$ git remote
Muestra nombre (alias) de remotos especificados.
-v #muestra los alias y la URL asociada a cada uno.
add <alias> <URL> #Agrega el remoto que pertenece a <URL> y le asigna el nombre <alias>
show <alias> #Inspecciona remoto. Muestra su información, qué ramas se están usando en local, en remoto, a donde van los push, de donde vienen los pull, etc.
rename <alias-actual> <alias-futuro> #Asigna un nuevo alias a un remoto.
rm <alias> #elimina el remote <alias>

```
$ git fetch <alias> 
'Trae' los datos que aún no se tengan de <alias> a local.

```
$ git pull
'Trae' datos e intenta mezclarlos con local.

```
$ git push [nombre-remoto] [nombre-rama] 
Envía todos los commits que se hayan echo. (hay que tener permisos de escritura)

```
$ git tag #lista etiquetas en orden alfabético.
-l 'v1.2.3' #etiqueta ligera
-a 'v1.2.3' #etiqueta anotada. (Las etiquetas anotadas guardan más información, apuntan a una confirmación)
-a 'v1.2.3' -m 'mensaje 
```
$ git status
muestra el estado en el repositorio local. Los archivos rastreados, modificados y el area de preparación.
-s #lo muestra en versión reducida.
-b #indica la rama de la que va mostrar el estado.


```
