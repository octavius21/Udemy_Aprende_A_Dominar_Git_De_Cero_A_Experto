# GIT

_Esta rama esta dedicada a la comprensión de los conceptos basicos como tambien conocer los comandos basicos para el uso correcto del mismo_

## Introducción 🚀

_Estas instrucciones te permitirán comprender mejor los comandos de git para su uso correcto._

### Pre-requisitos 📋

_Cosas que necesitas para hacer uso del software y como instalarlas, este apartado se enfocará en SO Windows 10 x64_

_Descargar los siguientes softwares_

* [Git](https://git-scm.com) - El versionamiento a usar en esta caso la 2.32.0
* [GitKraken](https://www.gitkraken.com) - El IDE para visualizar mejor el versionamiento, version 7.6.1
* [VisualCode](https://code.visualstudio.com) - El IDE para visualizar mejor los cambios realizados en los archivos, version 1.57

### Instalación 🔧

_Posteriormente de haberlos descargados_

_Realizar doble click en el archivo .exe deseado_

```
Da un ejemplo
```

_Y repite para el segundo y tercer archivo .exe deseado_

```
hasta finalizar
```

_Realmente la instalación no es dificil es dar next y finish_
_Al terminar la instalación de los software anteriormente mencionados se realizara una verificación rapida_

_Para realizar una verificación de los software que esten correctamente instalados, realizar los siguientes pasos:_
_Para verificar que el versionamiento[GIT] lo tenemos instalado_
_Abrir uno de estas terminales: powershell, CMD, Terminal_

_Escribir el siguiente comando_

```
git
```
_Debera aparecer algo parecido a lo siguiente_
```
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone             Clone a repository into a new directory
   init              Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add               Add file contents to the index
   mv                Move or rename a file, a directory, or a symlink
   restore           Restore working tree files
   rm                Remove files from the working tree and from the index
   sparse-checkout   Initialize and modify the sparse-checkout

examine the history and state (see also: git help revisions)
   bisect            Use binary search to find the commit that introduced a bug
   diff              Show changes between commits, commit and working tree, etc
   grep              Print lines matching a pattern
   log               Show commit logs
   show              Show various types of objects
   status            Show the working tree status

grow, mark and tweak your common history
   branch            List, create, or delete branches
   commit            Record changes to the repository
   merge             Join two or more development histories together
   rebase            Reapply commits on top of another base tip
   reset             Reset current HEAD to the specified state
   switch            Switch branches
   tag               Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch             Download objects and refs from another repository
   pull              Fetch from and integrate with another repository or a local branch
   push              Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
```
_Para verificar que los otros software esten correctamente instalados basta con buscarlos, o revisar si se nos creo algun acceso directo_

## Ejecución ⚙️

_A continuacion crearemos un directorio donde ubicaremos nuestro proyecto **Dummy** y la utilización de los software _

_Se abrira un CMD_
_Abrimos una venta ejecutar_
```
windows+R
```
_Escribimos `CMD` y damos enter_
_Nos posicionaremos en la ruta deseable a depositar el proyecto, en este caso haremos una carpeta en Desktop_
_Creamos una carpeta o nos posicionamos en la carpte deseada_
```
mkdir Repositorio
```
_Inicializamos que queremos que esta carpeta tenga versionamiento con el siguiente comando_
```
git init
```
_Posteriormente abrimos GitKraken_
*Para visualizar un repositorio ya creado:*
_Para Enlazarlo con gitHub visualizar el siguiente link_
* [Con GitHub](https://support.gitkraken.com/integrations/github/) - Enlazamiento con Github
* [Con Bitbucket](https://support.gitkraken.com/integrations/bitbucket/) - Enlazamiento con Bitbucket
_Nota 1:Deberas tener el link de tu repo obtenido del repositorio de tu seleccion para ponerlo en gitKraken_
_Nota 2:Deberas de otorgar acceso a gitKraken en caso de que te pida accesar a tus repositorios_

_¡Listo!, podremos vizualizar la linea de tiempo, estados(commits), Branchs(locales y remotos), etc en la aplicación de gitKraken_

_Abrimos Visual Code_
_En la barra de Menús->`File`->`Open Folder`->\[seleccionamos la carpeta de nuestro repositorio\]_
_¡Listo! podremos revisar los cambios aqui, resolvimiento de conflictos, modificacion de archivos_
_*Opcional* Podremos usar la termianl desde VC con el siguiente comando_
```
crtl+ñ
```


### Comandos de Git 🔩

_Crear una nuevo repositorio_

```
git remote add origin https://github.com/bluuweb/tutorial-github.git
git push -u origin master
```
_Subir los cambios locales despues que se aceptaran las postulaciones_

```
git push
```
_Bajar cambios remotos_

```
git pull
```
_Comparacion entre local y remoto_

```
git fetch
```
_Clonar Repositorio_

```
git clone https://github.com/bluuweb/tutorial-github.git nombreCarpeta
```
_Obtener un status de conclictos, modificaciones en los archivos, rama actual, mas información_

```
git status
```
_Agregar todos los archivos modificados a una "postulación"_

```
git add --all
```
_Agregarlos a un bloque_

```
git add [ARCHIVO.EXTENSION]
```
_nota: debes estar ubicado en la carpeta o poner la ruta para ubicar el archivo_
_Aceptar la postulacion, tambien en este punto se realiza un estado_

```
git commit -m "mensaje"
```
_nota:Es obligatorio el mensaje_
_Crear una rama_

```
git branch <rama_nueva>
```
_Cambio de rama_

```
git checkout <rama_a_moverte>
```
_listar todas las ramas disponibles tanto locales como remotas_

```
git branch -a
```
_Listado de los commits hechos_

```
git log
```
_Subir la nueva rama_local al Repositorio_

```
git push origin <rama>
```
_nota:si haces un push en la rama actual automaticamente se crea la rama sin la necesidad del comando pasado_

## Wiki 📖

_Puedes encontrar mucho más información al respecto en:_
* [Tutorial básico]( https://bluuweb.github.io/tutorial-github/guia/github.html) - Tutorial
* [Ramas y fuciones]( https://bluuweb.github.io/tutorial-github/guia/github.html) - Ramas y Funciones
* [Merge](https://www.atlassian.com/es/git/tutorials/using-branches/git-merge) - Merge
* [Manejo de ramas](https://desarrolloweb.com/articulos/trabajar-ramas-git.html) - Manejo de ramas
* [Clonacion de ramas](https://www.freecodecamp.org/espanol/news/como-clonar-una-branch-en-git/) - Clonación 
* [Ramas y fuciones](https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Procedimientos-B%C3%A1sicos-para-Ramificar-y-Fusionar) - Ramificar y Fusionar




## Autores ✒️

* **Luis Gomez** - *Trabajo Inicial* - [Ing. Luis Octavio](https://github.com/octavius21)
