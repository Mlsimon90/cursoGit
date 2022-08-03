# CLASE 02

## .gitignore

Es un archivo. Me permite descartar archivos. Qué git ignore el archivo.
Se crea normalmente en el directorio raíz del proyecto

## .gitkeep

Le permite a git ver carpetas vacías y versionarlas

## GIT BRANCH (RAMAS)

### Crear rama

    git branch <nombre-rama>
    git branch rama-branches

### Listar ramas

    git branch

### Cambiarme de rama

    git switch <nombre-rama>
    git switch rama-branches

### Borramos una rama

    git branch -d <nombre-rama>
    git branch -d rama-branches

### Forzar borrado de rama (Con contenido que no fue fusionado)

    git branch -D <nombre-rama>
    git branch -D rama-branches

## GIT MERGE: Funsión de ramas

**IMPORTANTE:** Tengo que estar en la rama en al cual quiero traerme los cambios. Si quiero traerme lo rama-branches. Tengo que estar en master y ejecutar el git merge.

    git merge <rama-que-me-quiero-traer>
    git merge rama-branches

### TIPO DE FUSIONES (MERGE)

Fast-forward: (La fusión va a ser automática) No hay conflicto
Recursiva: (Unión automática) No hay conflicto
Manual: (No va poder resolver en forma automática) O sea hay conflictos.

## GIT LOG

    git log --help

    git log --oneline --decorate --all --graph

## GIT ALIAS

> Agregar alias

    git config --global alias.l "log --oneline"
    git config --global alias.l "log --oneline --all --decorate --graph"
    git config --global alias.c "commit -am"
    git config --global alias.s "status --short"
    git config --global alias.c "commit -m"

> Borrar alias

    git config --global --unset alias.c

> Listar alias disponisbles

    git config --get-regexp alias

## GIT COMMIT (Cont...)

Enmendar un commit. Corregir.

    git commit --amend
