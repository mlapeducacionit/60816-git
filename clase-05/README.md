# Clase 05

## Trabajar en proyectos Open Source (Pull Request)

1. Hacer un fork del proyecto. (Me copia el repo a mi cuenta de github)
2. Me clono el fork desde mi cuenta GitHub
3. Trabajo normalmente. Subo los cambios
4. Me voy al proyecto original en el apartado Pull Request. Creo uno nuevo
5. Una vez tendré que actualizar mi fork.
6. Voy a cuenta del proyecto original y me copio la url del repositorio.
7. Agrego la url del repositorio original a mi repo local

    git remote upstream <URL-repositorio-original>

8. Me traigo los cambios

    git pull upstream <rama-que-quiero-actualizar>

9. Subir esas actualizaciones del repositorio local a mi remoto.
## TAG (Etiquetado)
Me permite etiquetar commits.

> Ver tags disponibles tengo

    git tag

> Como creo un tag en el commit actual

    git tag v1.1

> Como creo un tag en un commit en especifico

    git tag v1.1 <hash>
    git tag v1.1 25fc265

> Usan los tag: Con Versionado Semantico

    git tag -a v0.8.0 <hash> -m "Versión 0.8.0"
    git tag -a v0.8.0 d21e942 -m "Versión 0.8.0"

a: anotado
m: mensaje

> Muestra información detallada de los tags

    git show v0.8.0

> Para borrar el tag

    git tag -d v0.8.0

> Para subir todos los tags (NO RECOMENDABLE)

    git push --tags

> Para subir todos los tags (NO RECOMENDABLE)

    git push --tags

> Para subo un tag en especifico

    git push origin <nombre-tag>