# Breve introducción a la programación

## ¿Qué es un programa?
Un programa es una serie de instrucciones que dicen a una computadora que hacer. Estas instrucciones se escribe en lenguajes parecidos al inglés llamados lenguajes de programación.
Al conjunto de instrucciones escritas en algún lenguaje de programación, le llamamos código fuente.
El código fuente puede ser convertido en código ejecutable mediante el uso de compiladores o ejecutado directamente mediante el uso de intérpretes.

## Lenguajes de programación.
Existen diferentes lenguajes de programación, todos ellos con diferentes filosofías de diseño. La finalidad es la misma, dar instrucciones a la computadora. 
Cada lenguaje tiene una sintaxis distinta además de un conjunto de palabras reservadas que no pueden ser usadas por el programador libremente.
Algunos lenguajes famosos son, C, Java, Javascript.

## Editores de Texto y Entornos de desarrollo.
Es posible utilizar cualquier editor de texto para escribir un programa de computadora, sin embargo para facilitar esta tarea existen los editores de texto especializados y los entornos de desarrollo o 
IDE por sus siglas en inglés. Los editores ayudan autocompletando palabras o coloreando la sintaxis del lenguaje.
Los IDEs, por su parte, ayudan al programador con todo su flujo de trabajo. Agrupan archivos creando proyectos, revisan sintaxis, advierten de posibles errores en el código, convierten el código fuente

## Compiladores e intérpretes
Imagina que escribes un libro en español y planeas editarlo en diferentes idiomas para que todo el mundo lo entienda. Para ello necesita ser traducido y escrito en otro idioma. Esto es similar al trabajo
del compilador que se encarga de traducir tu código fuente a código máquina. 
Otra opcion que tienes para que todos sepan que dice tu libro, es que alguien lo traduzca mientras lo lee. Este es el trabajo del intérprete. 
 
## Escribiendo un programa
### Punto de entrada.
Todos los lenguajes tienen un punto de entrada, un lugar que indica donde empezará la ejecución de nuestro programa.

Por ejemplo, en Lenguaje C, el punto de entrada se llama main.
```
int main(int argc, char* argv)
```

De la misma manera, en Java, el punto de entrada se llama main.
```
public static void main(String [ ] args)
```

### Variables
Las variables son una forma de almacenar valores para su posterior procesamiento.
Por ejemplo:
```
var x = 10
var y = 20
var z = y + x
print z
```

Algunos lenguajes exigen que el tipo de dato de la variable sea especificado en su declaración.
### Tipos de dato
Un tipo de dato es un atributo que indica al compilador o intérprete que información puede contener una variable
Por ejemplo:
```
var x:int = 0
var y:String = "Hola"
```

### Control de flujo
El control de flujo, es la forma en la que podemos realizar decisiones en nuestros programas.
Los flujos básicos son:
+ if-then-else
+ loops
+ switch/case
#### if then else
El *if then else* nos permite ofrecer una bifurcación y ejecutar código basado en una condición.

```
var x:int = 10
if x < 10 then
 print "x es menor a 10"
else
 print "x es mayor a 10"
end
```

#### Loops
Los loops nos permiten ejecutar un bloque de código hasta o mientras se cumpla una condición.
Hay diferentes tipos de loops:
+ while do
```
var x:int = 10
while x > 0 do
 print "El valor de x es :\(x)"
 x = x - 1
end 
```
+ do while
```
var x:int = 10
do
 print "El valor de x es :\(x)"
 x = x - 1
while x > 0
```
+ for loop
```
for (var x:int = 0; x < 10; x = x+1 )
 print "El valor de x es :\(x)"
end
```

Los loops son equivalentes entre si, sin embargo el do while, ejecutará siempre alguna instrucción antes de evaluar la condición. El for loop permite definir valores iniciales y condiciones en una sola linea 
 

### Funciones y procedimientos
Los procedimientos son bloques de código reutilizable. Una función es un procedimiento que devuelve un valor.

```
funcion 
```

## Precedencia de operadores

