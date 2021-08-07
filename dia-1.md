# Ejercicios día 1

Recuerda que puedes hacer preguntas en el [Foro de Make It Real](https://foro.makeitreal.camp/c/intro-javascript-jul-2021/9).

## Ejercicio 1

Escribe un programa que le pida al usuario ingresar una frase y la imprima en la consola.

Recuerda que para pedirle al usuario que escriba una frase debes utilizar el método `prompt()` y para escribir en la consola debes utilizar el método `console.log()`.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-1-js-julio/3346).//OK

REPUESTA
```
let message=prompt(‘Ingresa tu mensaje’)
console.log(message)
```

## Ejercicio 2

Escribe un programa que le pregunte al usuario su nombre e imprima "Hola " seguido del nombre y un signo de exclamación.

Por ejemplo, si el usuario ingresa "Pedro" el programa debe imprimir en la consola "Hola Pedro!".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-2-js-julio/3347)//OK

RESPUESTA
 
 ```
 let nombre=prompt(’¿Como te llamas?’);
 console.log( Hola ${nombre} ! )
```

## Ejercicio 3

Escribe un programa que le pida al usuario ingresar un número, luego le pide un segundo número, e imprima en la consola la suma de los dos números que ingresó el usuario.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-3-js-julio/3348)//OK

RESPUESTA

```
let number1=parseInt(prompt(‘Ingresa el primer digito a sumar’));
let number2=parseInt(prompt(‘Ingresa el segundo digito a sumar’)); 
let sum= number1+number2 console.log( El resultado de la suma es ${sum} )
```

## Ejercicio 4

Escribe un programa que le pida al usuario su año de nacimiento e imprima su edad actual en la consola con la frase "Tienes X años". Por ejemplo, asumiendo que el año actual es 2020 y el usuario ingresa 2000, el programa debe imprimir en la consola:

```
Tienes 20 años
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-4-js-julio/3349)//OK

RESPUESTA

```
let userYear=parseInt(prompt(‘Cual es tu ano de nacimiento’))
let year=new Date().getFullYear()
let age=year-userYear 
if(year > userYear & & userYear > 1900){ 
console.log( Tu edad actual es ${age} anos )
}else{
console.log(‘Verifica el ano ingresado’)}
```

## Ejercicio 5

El índice de masa corporal (IMC), o BMI por sus siglas en inglés, es un valor que determina la cantidad de grasa de una persona.

El BMI se calcula con la siguiente formula:

```
peso / altura^2
```

Escribe un programa que le pida al usuario su peso y su altura para calcular su BMI e imprima la frase "Tu BMI es X".

Por ejemplo, si el usuario ingresa 65 de peso y 1.8 de altura el programa debe imprimir en la consola la frase "Tu BMI es 20.061728395061728".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-5-js-julio/3350)//OK

RESPUESTA

```
let peso = parseFloat(prompt(‘Ingresa tu peso en kilos’)) 
let altura = parseFloat(prompt(‘Ingresa tu altura en metros’)) 
let masaCorporal =peso/(altura*altura) 
console.log( Tu BMI es ${masaCorporal} )
```


