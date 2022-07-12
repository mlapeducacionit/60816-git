# Clase 02

# Status de arhivos

* UNTRACKED > Archivos que o se agregaron al index. O están en el WD

* STAGED > Archivos que  no fueron agregados al repositorio y cuyos cambios fueron validados.

* UNMODIFIED > Archivos que se encuentran en el repositorio y que no fueron modificados

* MODIFIEAD > Archivos que se encuentran en el repositorio pero difieren con lo que se encuentra en el WD


## GIT LOG

Ayuda de git log

    git log --help

Muestra versión completa

    git log

Muestra versión corta

    git log --oneline

Muestra una cantidad de commit seleccionado

    git log -<cantidad-commit>

    git log -3

Busco por fechas

    git log --since="2022-05-01"
    git log --after="2022-07-03"
    git log --before="2022-07-08"
    git log --since="<fecha>" --before="<fecha>" --oneline -4

## GITIGNORE

Archivo que nos permite no darle seguimiento a otros

    .gitignore

## GIT COMMIT

    git commit --help

### Sacar una foto o hacer commit. Se abre el editor que hayan configurado

    git commit

### Para poner un mensaje directamente en consola

    git commit -m "mensaje"

### Si quiero directamente hacer un git add y un git commit 

**IMPORTANTE**: El archivo tiene que estar dentro del repositorio de git. O sea los archivos UNTRACKED no los agrega a la foto.

    git commit -am "mensaje"

### Crear un commit vacío

    git commit --allow-empty -m "mensaje"

### Agrego algo que me olvidé en el último commit

    git commit --amend