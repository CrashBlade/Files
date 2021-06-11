## Create a new repository on the command line

* git init

* git add README.md

* git commit -m "first commit"

* git branch -M main

* git remote add origin https://github.com/CrashBlade/Xxxxxxxxxxx.git

* git push -u origin main



## Push an existing repository from the command line

* git remote add origin https://github.com/CrashBlade/Xxxxxxxxxxxxx.git

========================

* git branch -M main

* git push -u origin main

========================

* git push -u origin master

========================

## Configuration Commands

* git pwd (path del area de trabajo)

* git config --global user.name "Xxxxxx" (Asigna nombre del usuario)

* git config --global user.email "Xxxxxx" (Asigna el email del usuario)

* git config --global user.name (Muestra nombre del usuario)

* git config --global user.email (Muestra el email del usuario)

* git config --list --show-origin (Muestra origenes de los archivos de configuarcion)

* ls -al (muestra archivos de la ruta donde apunta el Bash)

* git config core.autocrlf true (Posible error/warning)

## Status Commands

* git status

* git status -s (version simple del estatus)

* git status -s -b (version simple del status y la branch)

## Adding Commands

git add

git add *.jpg (todos los archivos del directorio actual)

git add "*.jpg" (todos los archivos del proyecto)

git commit -m "xxxxx"

-*-*-*-*-*-*-*-*-*




git add folder/ (agrega todos los archivos)
git add folder/*.jpg (agrega los archivos jpg de la carpeta)
git add -A // add --all(agrega todos los modificados o nuevos)

git reset index.html
git reset *.html (todos lo html) 
git reset --soft HEAD^ (regresa el commit anterior para ser modificado)

-*-*-*-*-*-*-*-*-*-*-*-*
LOGS

git log
git log --oneline (descripcion corta del log)
git log -- oneline --decotate --all -- graph

-*-*-*-*-*-*-*-*-*-*-*-*-*
ALIAS
git config --global alias.lg "log --oneline --decotate --all --graph"
git config --global alias.s "status -s -b"
git config --global -e (edicion del archivo de config)
git config --global -l (listado del archivo de config no edita)

-*-*-*-*-*-*-*-*
git diff (verifica diferencias en archivos)
git diff --staged (verifica diferencias en archivos en Stage)
git diff rama1 master (diferencias entre rama master y rama1)
git reset HEAD file.md (quita el archivo del stage)

git checkout -- file.md (regresa a un estado anterior el archivo)

git commit -am "comentarios" (Adiciona y hace el commit) 
git commit --amend -m "mensaje" (Enmienda la descripcion del commit)


git merge rama1
git branch -d rama1 (borra la rama) 
	
gir checkout -b rama1 (crea la rama y se cambia a ella)

-*-**-*-*-*-*-*-*
git tag nombreTag (crea tags)
git tag (lista los tags)

git tag -d nombreTag (borra el tag)
git tag -a nombreTag -m "comentarios" (el -a es como un anotacion - por eso el -m)
git tag -a nombreTag HASHCOMMIT -m "comentario" (crea un tag para ese HASHCOMMIT)
git show nombreTag 
