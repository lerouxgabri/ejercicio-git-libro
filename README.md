# ejercicio-git-libro
ejercicios 4 y 5 me han salido mal. No los entiendo.

## Al realizar el comando git diff no me han aparecido las diferencias entre ramas.

## Ejercicio 1

````bash
git tag version1.0
git push origin --tags

````
## Ejercicio 2

```bash
cat > capitulo1.txt
"Agregada linea de texto en capitulo 1".
CTLR+D
git revert
git log
```

## Ejercicio 3

```bash
git branch nueva-funcionalidad
cat > capitulo5.txt
"En este capítulo veremos cómo gestionar múltiples ramas en Git."
CTLR+D
git commit -a -m "Nuevo cambio."
git log
Obtengo el hash.
git checkout main
git cherry pick hash-commit
git log
```

## Ejercicio 6

```bash
git merge nueva-funcionalidad main
git log
Obtengo el numero 

git revert d936cee -m 1
[main 000ab2b] Revert "Se ha añadido nuevo texto."
 2 files changed, 3 insertions(+), 2 deletions(-)
 delete mode 100644 capitulo5.txt
 ```

 ## Ejercicio 7

 ```bash
 git tag -d version1.0
 Etiqueta 'version1.0' eliminada (era 911f7c1)

 git push origin :refs/tags/version1.0
 Username for 'https://github.com': lerouxgabri
 Password for 'https://lerouxgabri@github.com': 
 To https://github.com/lerouxgabri/ejercicio-git-libro
 - [deleted]         version1.0
 
 ```

 ## Ejercicio 8

 ```bash
 git add README.md 
 git commit -m "Esto se borrara despues del reset"
 [main 84167bc] Esto se borrara despues del reset
 1 file changed, 4 insertions(+), 1 deletion(-)

 git reset --hard
 HEAD está ahora en 84167bc Esto se borrara despues del reset
 ```










