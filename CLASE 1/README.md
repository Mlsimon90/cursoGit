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