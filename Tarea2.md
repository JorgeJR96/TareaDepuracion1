# Tarea 2 

###### Jorge Jankovich Ramos - 2020

Dado el proyecto eclipse adjunto, comprobad mediante depuración del sistema:

1. En la función1 ¿Qué hacen estas líneas de código?<br>

String string2 = "string2";
string2= string2.substring(0,string2.length()-1);
string2=string2+"1";

Se crea el String2 con el texto "string2". Después se le resta la longitud del string, eliminando el ultimo contenido del string (2).
La última linea vuelve a añadir contenido al string. String2 cambia su contenido de "string2" a "string1".


2. ¿Qué valen las variables string1 y string2 antes de ejecutar el código de comprobación siguiente?<br>

if(string1 == string2 ) {
    System.out.println("SON IGUALES " + a);
}else{
    System.out.println("SON DIFERENTES");
}

String1: "string1". String2: "string2".

3. ¿Por qué no funciona el operador == ?¿Qué operador se debe usar en lugar de este?<br>

El operador == compara si ambos Strings son el mismo objeto, no su contenido. Para eso, se utiliza el equals()

if(string1.equals(string2)){
    System.out.println("SON IGUALES " + a);
}else{
    System.out.println("SON DIFERENTES");
}


4. La función2() está declarada como sigue:<br>

public void funcion2() {
    System.out.println("--------------------");
    System.out.println("Esta es la función 2");
    System.out.println("Cómo hago la llamada para que funcione????");

<br>
Esta función cómo la tengo que llamar desde el método MAIN para que funcione. Existen 2 posibilidades. Explícalas.<br>

dentro del main:
funcion2();
Introduciendolo en el main ejecuta la función.

si se introducen datos en la función, como por ejemplo x:
public void funcion2(int x);
funcion2 f2 = new funcion2(x);