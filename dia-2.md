# Ejercicios día 2

Recuerda que puedes hacer preguntas en el [Foro de Make It Real](https://foro.makeitreal.camp/c/intro-javascript-jul-2021/9).

## Ejercicio 6

Escribe un programa que le pida un número al usuario e imprima en la consola si el número es mayor o menor/igual a 10.

Si es mayor debe imprimir "El número es mayor a 10".

Si es menor debe imprimir "El número es menor o igual a 10".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-6-js-julio/3856).//OK

RESPUESTA
``` 
 let num = parseInt(prompt(‘Ingresa el numero a comparar’))
 if(num < 10){
 console.log( ${num} es menor a 10 ) 
 }else if(num > 10){
 console.log( ${num} es mayor a 10 )
 }else if(num = 10){ 
 console.log( El numero ingresado es ${num} ) }
 ```

## Ejercicio 7

Escribe un programa que piense un número de forma aleatoria del 1 al 10 y le pida al usuario que lo trate de adivinar. Si el número es correcto debe imprimir en la consola "Felicitaciones, ese era!", de lo contrario debe imprimir "Lo siento, intenta nuevamente!"

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-7-js-julio/3859).//OK

RESPUESTA

```
 let numRandom = Math.floor((Math.random()*10)+1);
 let num = parseInt(prompt(“Ingresa un numero”));
 if(numRandom===num){
 console.log( Felicitaciones ${num} es correcto )
 }else if(num > 10){
 console.log(‘Ingresa un numero del 1 al 10’) 
 }else{
 console.log( Lo siento, intenta nuevamente el numero correcto era ${numRandom})
 }
 ```

## Ejercicio 8

Un múltiplo de 5 es aquel que dividido por 5 da por resultado un número entero (sin residuo). Por ejemplo 10, 15, 20, etc. son múltiplos de 5. 11 no es múltiplo de 5 porque quedaría un residuo de 1.

Escribe un programa que le pida al usuario un número e imprima si es un múltiplo de 5 o no.

Si es múltiplo debe imprimir "Si, el número x es múltiplo 5", de lo contrario debe imprimir "No, el número x no es múltiplo de 5".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-8-js-julio/3861).//OK

RESPUESTA

```
 let num = parseInt(prompt(“Ingresa un numero”));
 if(num%5===0){
 console.log( Si el numero ${num} es multiplo de 5 )
 }else { 
 console.log( No, el numero ${num} no es multiplo de 5 ) 
 }
 ```

## Ejercicio 9

Escribe un programa que le pida un número al usuario e imprima en la consola si el número si es mayor, menor o igual que 10.

Si el número es menor a 10 debe imprimir "El número es menor que 10".

Si el número es mayor a 10 debe imprimir "El número es mayor que 10".

Si el número es igual a 10 debe imprimir "El número es igual a 10".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-9-js-julio/3862).//OK

RESPUESTA

```
let num = parseInt(prompt(“Por favor,Ingresa un número”));

if ( num > 10 ) {

console.log(El número ${num} es mayor a 10)

} else if ( num < 10 ) {

console.log(El número ${num} es menor a 10)

} else if ( num ===10 ){

console.log(El número ingresado es igual a 10)

} else {
console.log(Por favor, ingrese un número)
}
```

## Ejercicio 10


El índice de masa corporal (IMC), o BMI por sus siglas en inglés, es un valor que determina la cantidad de grasa de una persona.

El BMI se calcula con la siguiente formula:

```
peso / altura^2
```

Escribe un programa que le pida al usuario su peso y altura. El programa deberá calcular el BMI e imprimir:

* "Bajo de peso" si el BMI < 18.5
* "Normal" si está entre 18.5 y 24.9
* "Sobrepeso" si está entre 25 y 29.9
* "Obeso" si es igual o mayor a 30

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-10-js-julio/3863).//OK

RESPUESTA

```
let peso = parseFloat(prompt(“Ingrese su peso en kilos”));

let altura = parseFloat(prompt(“Ingrese su altura en metros”));

let masaCorporal= peso/ (Math.pow(altura,2))

if(masaCorporal<18.5){

console.log(Esta bajo de peso, su BMI es ${masaCorporal})

}else if(masaCorporal>18.5 && masaCorporal< 24.9){

console.log(Su peso es normal , su BMI es ${masaCorporal})

}else if(masaCorporal>=25 && masaCorporal< 29.9)

{console.log(Esta en sobrepeso , su BMI es ${masaCorporal})

}else if(masaCorporal>=30){console.log(Obeso, su BMI es ${masaCorporal})

}
``` 

## Ejercicio 11

Escribe un programa que le pida al usuario ingresar un número.

* Si el número es múltiplo de 3 debe imprimir en la consola "bing".
* Si el número es múltiplo de 5 debe imprimir en la consola "bong".
* Si el número es múltiplo tanto de 3 como de 5 debe imprimir en la consola "bingbong".
* Si no cumple ninguna de las condiciones anteriores debe imprimir el mismo número.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-11-js-julio/3865).//OK

RESPUESTA

```
let num = parseFloat(prompt("Ingrese el número a validar"));
if(num%5===0 && num%3===0){
  console.log('bingbong')
}else if(num%3===0){
  console.log('bing')
}else if(num%5===0){
  console.log('bong')
}else{ console.log(num)}

```


