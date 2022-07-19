# Clase 04

## .gitkeep: Versionar carpetas vacías
Creo un archivo vacío llamado .gitkeep dentro  de la carpeta que quiero versionar

## Alias 
Forma resumidar para llamar a un comando

git config --global alias.l "log --oneline"
git config --global alias.s "status --short"
git config --global alias.ll log --oneline --decorate --all --graph

### Ver alias disponibles

git config --get-regexp alias

### Borrar un alias

git config --global --unset alias.c

## Buenas prácticas para construir mensajes de commit

https://medium.com/@jmz12/buenas-pr%C3%A1cticas-para-commits-5eb4c86b9a47

## Aplicaciones desktop

* Git Kraken
* GitHub Destkop

## GIT BRANCHES (RAMAS) - REPASO

> Ver ramas en repo

    git branch 

> Crear un rama 

    git branch <nombre-rama>
    git branch dev

> Cambiar de rama

    git switch <nombre-rama>
    git switch dev

> Borrar un rama

    git branch -d <nombre-rama>
    git branch -d dev

> Forzar el borrado

    git branch -d <nombre-rama>
    git branch -d dev

Ej: Si quiero traerme a **master** lo que tengo en **dev**, tengo que estar posicionado sobre la rama **master**

    git merge <nombre-rama>
    git merge dev

### TIPOS DE MERGE 

* Fast-Fodward (No hay ningun conflicto, se hace en forma automatica)
* Recursivo - Uniones automaticas (Tampoco hay conflicto) - Trabaja con algoritmo
* Manual - (Donde hay conflictos - Y acá es cuando hay que junstarse para resolver el conflicto)

## GIT STASH
**NOTA**: Los stash no están disponibles en el remoto. Solo localmente. No se subir al remoto.

Link: https://www.atlassian.com/es/git/tutorials/saving-changes/git-stash

### Crear un stash

    git stash

### Veo los stash

    git stash list

### Para borrar un stash

> Borrar el último stash

    git stash drop

> Borrar un stash particular

    git stash drop 
    git stash drop stash@{0}

> Aplicar un stash, el último

    git stash pop

> Aplicar cualquier stash de los que tengo

    git stash apply 
    git stash apply stash@{1}

