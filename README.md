# curso de Git y GitHub

## basico

Agregar todos los cambios al _stoged_
_git add ._
_git commit -m "comentario"_

Agregamos el origen remoto de tu repositorio al github
_git remote add origin https://github.com/samir141673/curso-git.git_

La primera vez que vinculamos el repositorio remoto con el local
_git push -u origin master_

Para las subsecuentes actualizaciones ,si no cambias de rama
_git push_

Para descargar los cambios del repositorio remoto al local
git _pull_

# Cambiar la rama principal a main

## Para repositorios nuevos

1. _git init_
2. _git add ._
3. _git commit -m "primer commit"_
4. _git branch -M main_
5. _git remote add origin https://github.com/samir141673/curso-git.git_
6. _git push -u origin main_

## Para repositorios exisitentes

1. \_git branch -M main
2. _git remote add origin https://github.com/samir141673/curso-git.git_
3. _git push -u origin main_

## Para reemplazar la rama master por main GitHub

1. Crea la rama local main y pasalo el historial de la rama master

   _git branch -m master main_

2. Haz un push en la nueva rama local main en el repositorio remoto de GitHub

   _git push -u origin main_

3. Cambia el HEAD actual a la rama main

   _git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main_

4. Cambia la rama default de master a main en tu repositorio de GitHub

   Para hacerlo, sigue las instrucciones de este [enlace](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/changing-the-default-branch)

5. Elimina la rama master del repositorio remoto
   _git push origin --delete master_

## Para reemplazar la rama master por main en Git

_git config --global init.defaultBranch main_

## Ayuda

Ayuda en la terminal

_git comando -h_

Ayuda en el navegador

git help comando

## Ignorar archivos

esto es un comentario

archivo.ext

carpeta

/archivo_desde_raiz.ext

ignorar todos los archivos que terminen en .log

\*.log

excepto production.log

!production.log

ignorar los archivos terminados en .txt dentro de la carpeta doc,

pero no en sus subcarpetas

doc/\*.txt

ignorar todos los archivos terminados en .txt dentro de la carpeta doc
y también en sus subcarpetas

doc/\*_/_.txt

## Clonar repositorios

_git clone https://github.com/usuario/repositorio.git_

## Rama

Una rama nos permite aislar una nueva funcionalidad en nuestro código que después podremos añadir a la versión principal.
