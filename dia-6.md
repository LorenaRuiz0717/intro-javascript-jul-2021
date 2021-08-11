# Ejercicios día 6

Recuerda que puedes hacer preguntas en el [Foro de Make It Real](https://foro.makeitreal.camp/c/intro-javascript-jul-2021/9).

## Ejercicio 29

Escribe una función llamada `suma` que reciba dos números y retorne la suma de los dos números.

```javascript
// escribe la función suma acá

// código de prueba, verifica que aparezcan los valores correctos en la consola
console.log(suma(1, 2)) // 3
console.log(suma(0, 0)) // 0
console.log(suma(245, 923)) // 1168
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-29-js-julio/4135). No incluyas el código de prueba.//OK

RESPUESTA

```
function suma(a,b){
  return a+b
}
```

## Ejercicio 30

Escribe una función llamada `hola` que reciba un argumento (una cadena de texto) y retorne "Hola " seguido del argumento y un signo de exclamación.

```javascript
// escribe la función hola acá

// código de prueba
console.log(hola("Pedro")) // "Hola Pedro!"
console.log(hola("Juan")) // "Hola Juan!"
console.log(hola("")) // "Hola !"
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-30-js-julio/4136). No incluyas el código de prueba.//OK

RESPUESTA

```
function print(name){
  let hello='Hola '
return(hello+name+ '!')
}
```

## Ejercicio 31

El índice de masa corporal (IMC), o BMI por sus siglas en inglés, es un valor que determina la cantidad de grasa de una persona.

El BMI se calcula con la siguiente formula:

`peso / altura^2`

Escribe una función llamada `bmi` que reciba dos argumentos: peso y altura. Utiliza la fórmula para retornar el BMI correspondiente.

```javascript
// escribe la función bmi acá

// código de prueba
console.log(bmi(65, 1.8)) // 20.061728395061728
console.log(bmi(72, 1.6)) // 28.124999999999993
console.log(bmi(52, 1.75)) //  16.979591836734695
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-31-js-julio/4137). No incluyas el código de prueba.//OK

RESPUESTA

```
function bmi(peso,altura){
  let alturaPotencia=altura*altura
  return peso/(alturaPotencia)
}
```

## Ejercicio 32

La función `calcularColor` recibe un número como argumento y retorna un string de acuerdo al número:

* Si el número es 1 retorna "El color es negro".
* Si el número es 2 retorna "El color es blanco".
* Si el número es 3 retorna "El color es azul".
* De lo contrario retorna "El color es verde".

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-32-js-julio/4138). No incluyas el código de prueba.//OK

RESPUESTA

```
function calcularColor(num) {
  let color=''
  if (num === 1) {
    color = "black";
  } else if (num ===2) {
    color = "blanco";
  } else if (num === 3) {
    color = "rojo";
  } else {
    color = "verde";
  }

  return "El color es " + color;
}
```

## Ejercicio 33

Escribe una función llamada `capitalizar` que reciba una cadena y capitalice cada palabra de la cadena.

**Nota:** puedes asumir que cada palabra está separada por espacio.

```javascript
// escribe la función acá

// código de prueba
console.log(capitalizar("pedro perez")) // "Pedro Perez"
console.log(capitalizar("make it real")) // "Make it Real"
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-33-js-julio/4139). No incluyas el código de prueba.//OK

RESPUESTA

```
function capitalizar(frase){
frase=frase.split(" ")  
for(let i=0;i<frase.length;i++){
   frase[i]=frase[i].charAt(0).toUpperCase()+frase[i].slice(1)
}
frase=frase.join(" ")
return frase
}

```

## Ejercicio 34

Escribe una función llamada `promedio` que reciba un arreglo de números y retorne el promedio los elementos.

```javascript
// escribe la función acá

// código de prueba
console.log(promedio([1, 2, 3, 4])) // 2.5
console.log(promedio([7, 8, 9])) // 8
console.log(promedio([300, 100])) // 200
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-34-js-julio/4140). No incluyas el código de prueba.//OK

RESPUESTA

```
const promedio=(arraynums)=>{
  let promedio=0
  // console.log(arraynums)
 for (let i=0;i<arraynums.length;i++){
  promedio+=arraynums[i]/arraynums.length
   }
 return promedio

}
```
