# Consigna
Realizar un resumen sobre el trabajo con git. Cada grupo debera contribuir con una sección determinada. 
Nota: el documento está escrito en [Markdown](https://guides.github.com/features/mastering-markdown/)

```bash
git -v 
```


## Configuración inicial


## Comenzando a trabajar
 **colaboracion belve,ricardo,medina,gabo(arrestenlo)**
1) Para empezar se debe (primeramente realizar la configuracion inicial)
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

## Creando un repositorio local


## Clonando un repositorio 

 **Esto fue hecho por medina y gabo(llamen al 911 en el)**


## Trabajando con repositorios remotos 



## Diferencia entre fetch/merge y pull


## Etiquetas

## Gestión de logs

Podemos ver el historial de commits del proyecto usando el comando log.
Muestra el historial con el formato que indicamos:
git log --pretty=format:"%h - %an, %ar : %s"

Cambiamos la n por cualquier n�mero entero:
git log -n

Muestra los commits realizados despu�s de la fecha especificada:
git log --after="2016-04-07 00:00:00"

Muestra los commits realizados antes de la fecha especificada:
git log --before="2016-04-08 00:00:00"

Las banderas del comando git log se pueden usar juntas seg�n nos convenga:
git log --after="2016-04-07 12:00:00" --before="2016-04-07 12:30:00"

Este comando nos muestra el historial en una sola l�nea por commit:
git log --oneline


=======
<<<<<<< HEAD
## Deshaciendo cambi
=======
>>>>>>> 62eddef74fcc9ca6c5ffa44d16450760dee83d70
## Deshaciendo cambios
**Los cambios pueden deshacer en cualquier momento.**
Ten cuidado, a veces no es posible recuperar algo luego que lo has deshecho. Esta es una de las pocas áreas en las que Git puede perder parte de tu trabajo si cometes un error.

**Para deshacer el commit perdiendo las modificaciones:**
Para deshacer el ultimo commit usaremos:

```bash
git reset --hard HEAD~1
```
Donde "HEAD 1" indica la cantidad de commit a retoceder.
La sintaxis "HEAD 1" del comando anterior la podríamos traducir como “El commit al que está apuntando la rama activa menos uno”.

**Para deshacer el commit manteniendo las modificaciones:**
Existe la posibilidad de eliminar el commit pero manteniendo las modificaciones que contiene ese commit en el área de trabajo. 
Para ello, ejecutaríamos el siguiente comando: 

```bash
git reset HEAD~1 
```

Así que podemos seguir trabajando, corregir el bug o completar las modificaciones que habíamos dejado incompletas y hacer un nuevo commit con los cambios completos.
>>>>>>> f20b62a5964b619a63e484cb669e6b434e9d14d8
