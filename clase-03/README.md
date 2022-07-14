# CLASE 03

## GIT BRANCH

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

## GIT MERGE (Fusiones de ramas)

**IMPORTANTE**: Es que siempre tengo que estar en la rama que quiero recibir los cambios. 

Ej: Si quiero traerme a **master** lo que tengo en **dev**, tengo que estar posicionado sobre la rama **master**

    git merge <nombre-rama>
    git merge dev

### TIPOS DE MERGE 

* Fast-Fodward (No hay ningun conflicto, se hace en forma automatica)
* Recursivo - Uniones automaticas (Tampoco hay conflicto) - Trabaja con algoritmo
* Manual - (Donde hay conflictos - Y acá es cuando hay que junstarse para resolver el conflicto)


