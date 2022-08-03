# Clase 01

{{1 | 1:03:08}} Lo primero que hace es crear la carpeta, luego la subcarpeta clase 1, y dentro el archivo README.md

## Markdown

{{2 | 1:03:30}} Explica que son los Markdown es un lenguaje de marcas. Similar al HTML y como previsualizarlos en VSC
Por ejemplo el # reemplaza al <h1>H1</h1>, dos # representan un H2, tres un H3 y así

# H1

## H2

### H3

#### H4

##### H5

###### H6

---

### Negrita

{{3 | 1:05:00}} Explica como colocar texto en negrita, cursiva, etc

**Soy un texto en negrita**

### Cursiva

_Soy un texto en cursiva_

---

{{4 | 1:06:50}} Explica como colocar listas ordenadas y desordenadas

### Lista ordenadas

1. Item
2. Item
3. Item

### Lista desordenada

- Item
- Item
- Item

{{5 | 1:07:20}} Separador

---

{{6 | 1:10:30}} Explica como poner código

    git --version #esto me muestra la versión

{{8 | 1:12:30}} Explica diferencia entre colocar código de la forma del punto 6 y de la forma del punto 7, y porque ésta última es mejor

```bash
    git --version #esto me muestra la versión
```

{{7 | 1:11:11}} Explica otra forma de poner código

```php
$variable = "Hola
```

```js
function sumar(a, b) {
  return a + b;
}
```

backtick = ALT + 96
https://elcodigoascii.com.ar/

---

{{12 | 1:23:15}} Lista algunos comandos muy útiles para trabajar con consola

## COMANDOS CONSOLA

- ls : Listar directorios
- cd : Cambiar directorios
- cd .. : Volver para atrás un directorio
- cd ../.. : Vuelve 2 directorios para atrás
- touch : Creo archivos vacios
- mkdir : Creo directorios

---

{{8 | 1:14:20}} Este comando ya es propio de GIT y lo ejecuta en la consola

## GIT

    git --version

{{9 | 1:16:00}} Explica como abrir y como trabajar con la consola

{{10 | 1:19:00}} Con esto configuro y coloco en consola mi mail y nombre

## Hacer la configuración global de GIT

    git config --global user.name "Maximiliano Principe"
    git config --global user.email "mlapeducacionit@gmail.com"

{{11 | 1:21:00}} Este comando me muestra las configuraciones que hice cuando arranqué a trabajar con GIT

## Para visualizar las configuraciones

    git config --get-regexp user

{{13 | 1:29:30}}

## Crear un repositorio

    git init

{{14 | 1:36:00}}

## Areas en GIT

- Working Directory (WD): Vamos a tener todos los archivos de proyecto

- Staging Area (SA): Area intermedia de confirmación de cambios

- Local REPO - Cajita de Fotos - Commits: Los commits que voy haciendo

{{15 | 1:38:00}} Con "git status" veo el status de todo mi repositorio. Los veo en el work directory porque mi repositorio no tiene nada aún. Para pasarlo al repositorio ejecuto el comando "git add ." No es recomendable usar el "." porque agrega todo, pero en este caso lo hacemos solo a modo de ejemplo

## Para saber el estado de los archivos en WD y SA

    git status

{{16 | 1:59:00}} Con el comando Commit confirmo y envío definitivamente al repositorio todos los cambios. Cuando envío al repositorio, me acuse cuanto agregué, y cuanto eliminé en caso de haber eliminado algo. También me arroja un numero HASH

## ¿Cómo sacamos la foto (Commmit)?

Una vez confirmados los cambios (Los archivos están en el SA)

    git commit -m "Mensaje"

{{17 | 2:02:10}} Esto me permite ver la diferencia entre lo que tengo modificado y lo ya efectivamente commiteado. Una vez que ejecuto el comando git diff aprieot enter y me va mostrando en cada línea las diferencias entre lo que tengo commiteado y lo que tengo en el WD(working directory). Sigo apretando enter hasta que me diga (END) cuando en ese momento se me va a trabar la consola, aprieto Q para acabar el proceso

## Para ver las diferencias entre el WD y el Local Repo

    git diff

{{18 | 2:08:00}} Me detalla todos los commits que hice. Primero me detalla el HASH, pero el numero entero. El autor, la fecha de la modificación, y los ordena de arriba a abajo siendo el primero de arriba el mas reciente commit. El HASH es una función matemática que es un único número, imposible que se repita. Para elaborarlo toma datos del autor, el mail, la fecha, y el nombre y mensaje y con todos esos datos elabora el HASH.
El "git log --oneline" me muestra lo mismo pero resumido, un commit por línea

{{19 | 2:21:00}} Muestra como acceder a Github y crear un nuevo repositorio, y una vez creado con el comando de abajo nos hace vincular nuestro repositorio local al repositorio remoto de Github que acabamos de crear

## Para ver las fotos o commits del repositorio

    git log
    git log --online

{{22 | 2:25:30}}

## Configurar en el repo local un remoto

    git remote add origin <url>
    git remote add origin https://github.com/Mlsimon90/cursoGit.git

{{20 | 2:21:30}} Me muestra la URL o link del git remoto al que esta vinculado mi GIT

## Para verificar si tengo el remoto configurado

    git remote
    git remote -v

{{21 | 2:23:00}} Con esto hago subir mi repositorio local (master, por defecto viene main pero es por todo el tema del progresismo que explicaba el profe) al repositorio remoto que lo identifico como origin

## Subir al repo remoto

    git push -u <repo-remoto> <repo-local>
    git push -u origin master
