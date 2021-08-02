# Ejercicios día 5

Recuerda que puedes hacer preguntas en el [Foro de Make It Real](https://foro.makeitreal.camp/c/intro-javascript-jul-2021/9).

## Ejercicio 23

Escribe un programa que le pida una frase al usuario y la repita en mayúsculas. Por ejemplo:

```
Ingresa una frase> Hola Mundo
HOLA MUNDO
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-23-js-julio/4100).//OK

RESPUESTA
``` 
let frase=prompt('Ingrese una frase')
console.log(frase.toUpperCase())
```

## Ejercicio 24

Escribe un programa que le pida una frase al usuario y le muestre el número de caracteres "a" que hay en la frase. Por ejemplo:

```
Ingresa una frase> Hasta la próxima
La frase tiene 4 caracteres "a"
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-24-js-julio/4101).//OK

RESPUESTA
```
let frase=prompt('Ingrese una frase')
let contador=0
for(let i=0;i<frase.length;i++){
  if(frase[i]==='a')
  contador=contador+1
}
console.log(contador)
```
## Ejercicio 25

Escribe un programa que le pida una frase al usuario y le muestre una nueva frase con los siguientes cambios:

* Las mayúsculas se reemplazan por minúsculas.
* Se eliminan los espacios en blanco.
* Reemplaza el caracter "a" por "4".
* Reemplaza el caracter "e" por "3".
* Reemplaza el caracter "i" por "1".
* Reemplaza el caracter "o" por "0".

Ejemplo:

```
Ingresa una frase> esta es una prueba
3st43sun4pru3b4
```

**Nota:** Aunque esta es una forma de generar contraseñas no se considera segura y no la recomendamos.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-25-js-julio/4102).//OK

RESPUESTA

```
let frase = prompt('ingrese una frase')
frase = frase.toLowerCase()
let string = frase.split(" ")
string = string.join('')
let replace = string.replaceAll('a', '4')
replace = replace.replaceAll('e', '3')
replace = replace.replaceAll('i', '1')
replace = replace.replaceAll('o', '0')
```

## Ejercicio 26

Escribe un programa que le pida una frase al usuario y capitalice cada palabra. Por ejemplo:

```
Ingresa una frase> esta es una prueba
Esta Es Una Prueba
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-26-js-julio/4103).//OK

RESPUESTA

```
let frase=prompt("Ingresa una frase");
let palabras=frase.split(' ')
let nuevaFrase=[]

for (let palabra of palabras){
  let letra= palabra[0]
  let primeraLetra=letra.toUpperCase()
  for (let i=1;i<palabra.length;i++){
    let nuevaPalabra=palabra[i];
    primeraLetra+=nuevaPalabra
  }
  nuevaFrase.push(primeraLetra)
  
  }
  console.log(nuevaFrase.join(' '))
```  

## Ejercicio 27

Escribe un programa que le pida una frase al usuario e imprima cada palabra en una nueva línea. Por ejemplo:

```
Ingresa una frase> esta es una prueba
esta
es
una
prueba
```

**Nota:** Las palabras se separan por espacio.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-27-js-julio/4104).//OK

RESPUESTA

```

let frase=prompt("Ingresa una frase");
frase=frase.split(' ')
for(let i=0;i<frase.length;i++){
console.log(frase[i])
}
```

## Ejercicio 28 (Bonus)

Escribe un programa que le pida dos frases al usuario e imprima los caracteres que tienen en común. Si no tienen caracteres en común debe imprimir "No se encontraron caracteres en común".

Ejemplo 1:

```
Ingresa frase 1> German
Ingresa frase 2> Gabriela
Los caracteres en común son: G, e, r, a
```

Ejemplo 2:

```
Ingresa frase 1> Hola
Ingresa frase 2> Bye
No se encontraron caracteres en común
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-28-js-julio/4105).//OK

RESPUESTA

```
let frase1=prompt("Ingresa una frase");
let frase2=prompt("Ingresa otra frase")
let concidencia=''

for(let i=0;i<frase1.length;i++){
  if(frase2.includes(frase1[i])){
    concidencia=concidencia+frase1[i]+','
  }
} 
if(concidencia.length!=0){
console.log('Los caracteres repetidos son '+ concidencia)
}else{
  console.log('No tiene concidencias')
}
```
