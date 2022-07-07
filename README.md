# Git desarrollo Colaborativo

## Markdown
Sistema de etiquetado como HTML

# H1
## H2
### H3
#### H4
##### H5
###### H6

**Soy un texto en negrita**

*Soy un texto en cursiva*

### Listas 

1. Item
2. Item
3. Item

* Item
* Item
* Item

### Incluir snippets

```js
    function sumar(a,b) {
        return a + b
    }
```

## Requisitos

* https://cmder.net/
* https://code.visualstudio.com/
* https://git-scm.com/
* https://github.com/

## COMANDO CONSOLA

* ls - Listar directorios
* cd - Cambiar directorios
* cd <directorio>
* cd .. - Salgo de directorio
* clear - Limpiar consola
* mkdir - Creo directorios
* touch - Crea archivo
* rm - Borrar archivos
* rm -rf - Borrar directorios

### Verificar que tengo GIT

    git --version

### Configuro GIT

    git config --global user.name "<nombre>"
    git config --global user.email "<email>"

### Puedo configurar git por repositorio

    git config --local user.name "<nombre>"
    git config --local user.email "<email>"

### Para ver el estado del Working directory

    git status

### Para subir al escendario los archivos (Staging Area)

    git add <nombre>
    git add . # Agrega todos los archivos al escendario

### Para sacar la foto (Hacer un commit)

    git commit -m "<mensaje>"

### Para ver las fotos (Historia del repositorio)

    git log



