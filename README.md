# Introducción rápida a la programación
## ¿Qué es un programa?
Un programa es una serie de instrucciones que dicen a una computadora que hacer. Se escribe en lenguajes parecidos al inglés. 

## Compiladores e intérpretes.
Dado que las computadoras no hablán inglés, es necesario traducir lo que escribimos a lenguaje máquina. 
Para esto usamos compiladores o intérpretes. 
### Compiladores
Imagina que escribes un libro en español y quieres que todo mundo lo entienda. Lo que debes hacer es entregar tu libro a 
alguien que lo traduzca a diferentes lenguajes. 
### Intérpretes
Imagina de nuevo que has escrito un libro en español y vas a presentarlo frente a una audiencia que solo habla Nahuatl. 
Para evitar el proceso de traducción, un intérprete se encargará de trasladar cada palabra que dices del español a Nahuatl. 
Todo en tiempo real.
### ¿Son mejores los lenguajes compilados que los interpretados?
En el mundo de la programación, lo mejor es lo que resuelve el problema. Aunque ambos, interprete y compilador se encargan de 
traducir nuestro lenguaje de programación a código máquina, la diferencia principal es que el interprete es más flexible. 
Sin embargo, esta flexibilidad, viene con un costo. Generalmente los lenguajes interpretados son más lentos pues necesitan
ser interpretados cada que vez que se ejecutan a diferencia de los programas compilados pues, una vez compilado, un programa 
ya no necesita intérprete y será más "rápido". 
El lenguaje intepretado agrega esa capa extra que indudablemente genera latencia. Con la velocidad de las computadoras 
actuales, el tiempo de interpretación es despreciable, sin embargo, para aplicaciónes que requieran cierta velocidad como 
videojuegos, procesadores de multimedia, o incluso navegadores de internet, se siguen prefiriendo los lenguajes compilados.

## ¿Cual es el mejor lenguaje de programación?
De nuevo, el mejor lenguaje es el que resuelve el problema. Hay lenguajes nacidos en la academia, lenguajes hechos por 
empresas para resolver un problema específico, lenguajes orientados a objetos. Sin embargo, todos los lenguajes tienen cosas en común como puntos de entrada, variables, control de flujo. 

## Punto de entrada.
Todos los lenguajes tienen un punto de entrada, un lugar que indica donde empezará la ejecución de nuestro programa.

Por ejemplo, en Lenguaje C, el punto de entrada se llama main.
```
int main(int argc, char* argv)
```

## Variables
Las variables son una forma de almacenar valores para su posterior procesamiento.
Por ejemplo:
```
var x = 10
var y = 20
var z = y + x
print z
```

Algunos lenguajes exigen que el tipo de dato de la variable sea especificado en su declaración.
## Tipos de dato
Un tipo de dato es un atributo que indica al compilador o intérprete que información puede contener una variable
Por ejemplo:
```
var x:int = 0
var y:String = "Hola"
```

## Control de flujo
## Métodos y Funciones
## Comentarios en el código fuente
