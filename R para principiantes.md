# R para principiantes

##1.1 Construcción de una base de datos

Para aprender a construir una base de datos ejemplificaremos utilizando tres variables:

**Género**: Variable nominal con valores 1 y 2, donde representaran la categoría respuesta *"hombre"* y *"mujer"*, respectivamente.

**Ingreso**: Variable de razón con valores arbitrarios de ingreso monetario.

**Opinión acerca del aborto libre**: Variable ordinal con valores *1, 2, 3, 4, 5*; las cuales representan las catergorías *"nada de acuerdo", "un poco de acuerdo", ni de acuerdo ni en desacuerdo", "bastante de acuerdo"* y *"muy de acuerdo"*

### Ingresar los datos en R:

Para ingresar los datos, se debe escribir:

```
genero <- c(1,1,2,1,2,2,2,1,2)

ingreso <-c(100000,300000,500000,340000,300000,500000,650000,
410000,750000)

acuerdo <- c(1,1,3,2,4,1,5,3,2)
```
Posterior a la construcción de las variables, podemos utilizar el comando `data.frame` para construir una base de datos. Para esto debemos asignar el resultado del *data.frame* al objeto *"aborto"* que contendrá la base de datos construida.

```
#Creación de base de datos a partir de variables previamente creadas. Donde se asigna el resultado al objeto "aborto"

aborto <- data.frame(genero, ingreso, acuerdo) 
```
Finalmente se puede visualizar la base datos de dos maneras: utilizando el comando `View` o presionando el botón que se encuentra al lado del objeto base de datos en el entorno de trabajo del software (Usualmente ubicado en la ventana superior derecha). 
En el siguiente código se explicita la primera forma:

```
View (aborto)

```
