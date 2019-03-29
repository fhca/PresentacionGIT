# =)
## Ejercicios ! 

###### Preparativos
* Poner el internet =P.
* Abrir terminal.
* Crear carpeta donde van a hacer su cotorreo.
* Moverse dentro de esa carpeta.
* `git clone https://github.com/fhca/PresentacionGIT`

___

### Configurar git

* nombre 

`git config --global user.name "NombreUsuario"`

* correo

`git config --global user.email "correo@dominio.com”`

* editor 

`git config --global core.editor "gedit"`

___

### Flujo individual sencillo.

1. Iniciar repositorio vacío.
	* `mkdir ejercicios`
	* `cd ejercicios`
	* `git init`
	* `ls -a`
1. Crear primer archivo del proyecto.
	* readme.md es buena idea
	* `se puede crear con un editor o copiar`
1. Revisar el estado del repositorio.
	* `git status`
1. Preparar primer archivo.
	* `git add readme.md `
1. Revisar estado.
	* `git status`
1. Hacer primer confirmación.
	* `git commit`
1. Revisar estado.
	* `git status`
1. Revisar historial de confirmaciones.
	* `git log`

Respira...

1. Modificar el primer archivo.
	* `gedit readme.md `
1. Revisar estado.
	* `git status`
1. Crear otro archivo para el proyecto.
	* `se puede crear o copiar 'principal.c'`
1. Revisar estado.
	* `git status`
1. Crear un archivo no necesario para el proyecto.
	* v.gr. Una lista de tareas o notas. 
	* `copiar 'tareas.txt'`
1. Revisar estado.
	* `git status` ó `git status -s`
1. Preparar todos los archivos nuevos.
	* `git add .`
1. Revisar estado.
	* `git status -s`
2. des-preparar archivo que no vá en el proyecto.
	* `git rm --cached tareas.txt `
3. Revisar estado.
	* `git status -s`
3. Confirmar.
	* `git commit`
4. Revisar estado.
	* `git status -s`
5. Revisar vitacora de confirmaciones.
	* `git log -p`

Inhalar...

1. Agregar varios archivos NO necesarios para el proyecto.
	* `Copiarlos a la raíz desde la carpeta: 'archivosNoNecesarios'`
2. Agregar varios archivos necesarios para el proyecto.
	* `Copiarlos a la raíz desde la carpeta: 'archivosNecesarios'`
3. Preparar todos.
	* `git add .`
4. Quitar de preparados todos los archivos.
	* `git rm --cached *`
5. agregar .gitignore.
	* `abrir un editor de texto`
	* `agregar el texto (sin comillas) "secreto*"`
	* `guardarlo con el nombre (sin comillas) ".gitignore"`
6. cambiar nombre de 'tareas.txt' para que séa ignorado.
	* `por ejemplo 'secreto_tareas.txt'`
7. Revisar estado.
	* `git status`
7. Preparar todos.
	* `git add .`
8. Revisar estado.
	* `git status`
9. Confirmar los cambios
	* `git commit`
5. Revisar vitacora de confirmaciones.
	* `git log --oneline`

Exhalar...

1. Agregar varios archivos NO necesarios para el proyecto.
	* `Copiarlos a la raíz desde la carpeta: 'archivosNoNecesarios'`

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
- PD. GitLab existe.

___

### Compartir proyecto propio en Github.

1. Crear repositorio en GitHub.
	- En la página de GitHub.
 	- Clic en + (está en la esquina superior derecha).
	- Clic en 'New repository'.
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
