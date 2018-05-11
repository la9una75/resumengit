# Consigna
Realizar un resumen sobre el trabajo con git. Cada grupo debera contribuir con una secciÛn determinada. 
Nota: el documento est· escrito en [Markdown](https://guides.github.com/features/mastering-markdown/)

```bash
git -v 
```


## ConfiguraciÛn inicial

```bash
git config --global user.name "tu nombre"
```
Nombre de la persona que este trabajando con git 

```bash
git config --global user.email "tu email"
```
DirecciÛn de correo de la persona que esta trabajando con git 

```bash
git config --global http.proxy http://192.168.0.250:3128
```
Habilita el uso del servidor proxy 
 
## Comenzando a trabajar

1. Para empezar se debe realizar primeramente la [configuraciÛn inicial](## ConfiguraciÛn inicial)
2) se debe realizar una carpeta con el siguiente comando: 
```bash
*mkdir [nombre de la carpeta]*
```
en la cual se guardan todos los documentos.
3) Luego se ingresa en esa carpeta con el siguiente comando: 
```bash
*cd [nombre de la carpeta]*
```
4) Luego mientras estes en la carpeta se realiza el siguiente comando:
```bash
*git init*
```
es para empezar a trabajar con git sino no te deja insertar comando


### Creando un repositorio local
*Hecho Por Belvedere y Artencio*  
 Luego de crear el la carpeta nueva se accede a ella y se pone el comando
 ```bash 
 git init
```
 Este comando sirve para que tome en cuenta que esa carpeta es un repositorio dentro de
 esta carpeta se crea un archivo .git el cual es el que realiaza el correcto 
 funcionamiento del Git 

 Luego se agregan archivos (pag. , documentos, etc)
 y se realiza el comando 
```bash
git status 
``` 
 Donde nos mostrara los archivos editados pero NO guardados. Para guardar los cambios de 
 los mismo se utiliza el siguiente programa 
```bash 
git add . 
```
 Luego si lo deceamos podemos comentar los cambios realizados con el siguiente comando 
```bash
git commit -m "Mensaje del cambio" 
```
 Y se finaliza la creacion del repositorio.
### Clonando un repositorio 


=======


## Clonando un repositorio
 **Esto fue hecho por medina y alvarez**
 Para obtener una copia de un repositorio GIT existente se tiene que ingresar elsiguiente comando
 ```bash
 *git clone [url]*
 ```
 Para clonar un repositorio remoto existente [SSH]
 ```bash
 *git clone git+ssh://[nombre de usuario en el servidor remoto][dirreccion ip] [ruta exacta de donde esta ubicado]*
 ```
 Para clonar un repositorio remoto existente [HTTPS]
 ```bash
 *git clone [URL]*
 ```
 una vez clonado el repositorio **se pueden realizar las mismas acciones que si 
hubiesemos iniciado nuestro propio repositorio local**
=======

## Clonando un reposito



## Trabajando con repositorios remotos 



## Diferencia entre fetch/merge y pull



## Etiquetas



## Gesti√≥n de logs


Podemos ver el historial de commits del proyecto usando el comando log.
Muestra el historial con el formato que indicamos:
git log --pretty=format:"%h - %an, %ar : %s"

Cambiamos la n por cualquier n˙mero entero:
git log -n

Muestra los commits realizados despuÈs de la fecha especificada:
git log --after="2016-04-07 00:00:00"

Muestra los commits realizados antes de la fecha especificada:
git log --before="2016-04-08 00:00:00"

Las banderas del comando git log se pueden usar juntas seg˙n nos convenga:
git log --after="2016-04-07 12:00:00" --before="2016-04-07 12:30:00"

Este comando nos muestra el historial en una sola lÌnea por commit:
git log --oneline


=======

## Deshaciendo cambios
**Los cambios pueden deshacer en cualquier momento.**
Ten cuidado, a veces no es posible recuperar algo luego que lo has deshecho. Esta es una de las pocas √°reas en las que Git puede perder parte de tu trabajo si cometes un error.

**Para deshacer el commit perdiendo las modificaciones:**
Para deshacer el ultimo commit usaremos:

```bash
*git reset --hard HEAD~1*
```
Donde "HEAD 1" indica la cantidad de commit a retoceder.
La sintaxis "HEAD 1" del comando anterior la podr√≠amos traducir como ‚ÄúEl commit al que est√° apuntando la rama activa menos uno‚Äù.

**Para deshacer el commit manteniendo las modificaciones:**
Existe la posibilidad de eliminar el commit pero manteniendo las modificaciones que contiene ese commit en el √°rea de trabajo. 
Para ello, ejecutar√≠amos el siguiente comando: 

```bash
*git reset HEAD~1*
```

As√≠ que podemos seguir trabajando, corregir el bug o completar las modificaciones que hab√≠amos dejado incompletas y hacer un nuevo commit con los cambios completos.
