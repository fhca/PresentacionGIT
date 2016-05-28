# =)
## Ejercicios ! 

######preparativos
* Abrir terminal.
* Crear carpeta donde van a hacer su cotorreo.
* Moverse dentro de esa carpeta.
* Poner el internet =P.

___

### Configurar git

1. nombre
* correo
* editor 

___

### Flujo individual sencillo.

1. Iniciar repositorio vacío.
	* `mkdir ejercicios`
	* `cd ejercicios`
	* `git init`
	* `ls -a`
1. Crear primer archivo del proyecto.
	* readme.md es buena idea
vim readme.md
1. Revisar el estado del repositorio.
git status
1. Preparar primer archivo.
git add readme.md 
1. Revisar estado.
git status
1. Hacer primer confirmación.
git commit 
1. Revisar estado.
git status
1. Revisar historial de confirmaciones.
git log


git status -s
git commit 
git status -s

Respira...

1. Modificar el primer archivo.
vim readme.md 
1. Revisar estado.

1. Crear otro archivo para el proyecto.
vim principal.c
1. Revisar estado.
git status
1. Crear un archivo no necesario para el proyecto.
	* v.gr. Una lista de tareas o notas. 
vim tareas.txt
1. Revisar estado.
git status
git status -s
1. Preparar todos los archivos nuevos.
git add .
1. Revisar estado.
git status -s
2. des-preparar archivo que no vá en el proyecto.
git rm --cached tareas.txt 
3. Revisar estado.
git status -s
3. Confirmar.
4. Revisar estado.
git status -s
5. Revisar vitacora de confirmaciones.
git log -p

Inhala...

1. Agregar varios archivos no necesarios para el proyecto.
Copiarlos desde la carpeta: 
2. Agregar varios archivos necesarios para el proyecto.
Copiarlos desde la carpeta:
3. Preparar todos.
git add .
4. Quitar de preparados todos.
git rm --cached *
5. agregar .gitignore.
echo "secreto_*" >> .gitignore
6. Revisar estado.
git status
7. Preparar todos.
git add .
8. Revisar estado.
git status


___

###Ramas locales:

1. En un repositorio existente:
1. Crear una rama y en ella un archivo exclusivo de ella.
	* `git branch a` 
	* `git checkout a`
	* `vi archivo-a`
	* `git add archivo-a`
1. Repartir el paso anterior en otra rama. 
	* `git branch b`
1. Listar ramas existentes.
1. Fusionarlas sin causar problemas.
1. Intentar fusión causando problemas.
1. Resolver problemas.
1. Fusionarlas.

___

## Locales + remotos

### Crear cuenta en Hithub.

1. Entra a la página: www.github.com
1. Clic en botón: signup
1. Llena formulario.
1. Escoger un plan, (por defecto ya está escogido el plan gratuito.
1. Clic en: Finish sign up
1. Verificar el correo: Entra a tu cuenta de correo, busca un correo cuyo remitente es Github, abrir el correo y clic en: Verify email adress.
- FIN
- PD. Gitlab existe.

___

### Compartir proyecto propio en Github.

1. Crear repositorio en Github.
	- Clic en + (está en la esquina superior derecha).
	- Clic en New repository.
	- Pon nombre al repositorio.
	- Pon su descripción.

___

### Clonar proyecto de Github.

1. Conseguir dirección de repositorio.
1. Clonar dicho repositorio.
1. Si se tiene derchos de escritura se puede contribuir directamente a ese proyecto.

___

### Fork.

1. Hacer un fork de la URL: https://github.com/fhca/PresentacionGIT.git

### Merge request.

1. Entrar a la dirección:
2. 

___
