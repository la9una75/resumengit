# Consigna
Realizar un resumen sobre el trabajo con git. Cada grupo debera contribuir con una sección determinada. 
Nota: el documento está escrito en [Markdown](https://guides.github.com/features/mastering-markdown/)

```bash
git -v 
```


## Configuración inicial


## Comenzando a trabajar


### Creando un repositorio local


### Clonando un repositorio 



## Trabajando con repositorios remotos 



### Diferencia entre fetch/merge y pull


## Etiquetas

## Gestión de logs

## Deshaciendo cambios
Los cambios pueden deshacer en cualquier momento.

Para deshacer el commit perdiendo las modificaciones:
Para deshacer el ultimo commit usaremos:

```bash
"git reset --hard HEAD~1" 
```
Donde "HEAD~1" indica la cantidad de commit a retoceder.
La sintaxis HEAD~1 del comando anterior la podríamos traducir como “El commit al que está apuntando la rama activa menos uno”.

Para deshacer el commit manteniendo las modificaciones:
Existe la posibilidad de eliminar el commit pero manteniendo las modificaciones que contiene ese commit en el área de trabajo. 
Para ello, ejecutaríamos el siguiente comando: 

```bash
git reset HEAD~1 
```

Así que podemos seguir trabajando, corregir el bug o completar las modificaciones que habíamos dejado incompletas y hacer un nuevo commit con los cambios completos.