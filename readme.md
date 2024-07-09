# ejercicio 2


* [ ] Crea un repositorio llamado ejercicio2 en local.
* [ ] Realiza un commit en local con el texto Inicializando el repositorio.

* [ ] Crea un branch que se llame develop
* [ ] Realiza el checkout del branch develop

* [ ] Crea un archivo README.md que contenga el texto como titulo ejercicio2.
* [ ] Realiza el commit con mensaje "Creando README.md"

* [ ] Inserta una descripción en el README.md
* [ ] Realiza el commit con mensaje "Modificando README.md"

* [ ] Crea un archivo de python que contenga el siguiente codigo:

```python

print('Hello')
```

* [ ] Realiza un commit en local.
* [ ] Realiza el push a github para crear el repositorio online.

* [ ] Realiza un merge a la rama main
* [ ] Realiza el push a github para crear la rama main online.

* [ ] Comparte el repositorio con mikelalda13
# Txuleta comandos git

En este repositorio voy a explicar brevemente los comandos para tenerlos a mano y saber que es lo que hace cada uno de ellos.

## Comandos básicos para la gestión de un repositorio

***git init***

```console
git init
```

Este comando inicializa un repositorio (en local)

---

***git status***

```bash
git status
```

Este comando muestra el estado de la rama en la que nos encontramos

---

***git add***

```bash
git add -u #añadir al staged area los archivos modificados
```

o

```bash
git add -A #añadir al staged area todos los archivos
```

o

```bash
git add <nombre archivo> #para añadir solo el archivo que queremos
```

* git add -u: añadir al staged area los archivos modificados
* git add -A: añadir al staged area todos los archivos

---

***git rm***

```bash
git rm --cached <file> [-f]
```

quitar del staged area los archivos añadidos para el commit

* -f: existe la opcion -f para forzar el unstage

---

***git commit***

```bash
git commit -m "mensaje" [-a]
```

Realiza un commit, es decir, lo guarda en el repositorio.

* -a: la opcion para añadir automatimaticamente al staged area los archivos modificados

---

***git log***

```bash
git log [--all] [--oneline] [-<cantidad>] [--first-parent] [<commit>]
```

podemos ver logs de los commits

---

***git checkout***

```bash
git checkout <filename>
```

o

```bash
git checkout <nombre-branch>
```

o

```bash
git checkout <7digitos-del-hash>
```

o

```bash
git checkout -b <nobre-del-nuevo-branch>
```

* git checkout filename: para deshacer los cambios
* git checkout nombre-branch: para ir al branch
* git checkout 7digitos-del-hash: para ir al commit
* git checkout -b: para crear una nueva rama y hacer el checkout

---

***git reset***

```bash
git reset
```

descarta las modificaciones de staged area

---

***git branch***

Solo muestra repositorios locales

```bash
git branch [-a] [-vv]
```

* -a: la opcion para mostrar los repositorios remotos.
* -vv: muestra la información del repositorio.

añadir una nueva rama o branch

```bash
git branch <nombre-rama>
```

---

***git push***

para el primer push de una nueva rama

```bash
git push --set-upstream origin <nombre-rama>
```

para los siguientes

```bash
git push
```

---

***git fetch***

Para traer los cambios de los repositorios remotos

```bash
git fetch
```

---

***git pull***

Para traer los cambios de los repositorios y volcarlo en el repositorio en el que estamos trabajando.

```bash
git pull
```

---

***git show***

Muestra los ultimos cambios realizados en los commit

```bash
git show
```

---

***git diff***

```bash
git diff
```

o

```bash
git diff <rama-antigua> <rama-nueva>
```

o

```bash
git diff <hash-commit> <rama-comparar>
```

* git diff: Para mostrar los cambios que tenemos para subir al staged area
* git diff rama-antigua rama-nueva: comparar dos ramas
* git diff hash-commit rama: para comparar entre rama y commits

---