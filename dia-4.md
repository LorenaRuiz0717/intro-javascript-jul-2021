# Ejercicios día 4

Recuerda que puedes hacer preguntas en el [Foro de Make It Real](https://foro.makeitreal.camp/c/intro-javascript-jul-2021/9).

## Ejercicio 18

Crea un programa a partir de las siguientes instrucciones:

1. Crea una variable llamada `nombres` con un arreglo que tenga los siguientes elementos: "Pedro", "Pablo", "María", "Juan", "Diana".
2. Pídele al usuario que ingrese un nombre e insértalo al final del arreglo que creaste en el paso 1.
3. Pídele al usuario que ingrese otro nombre y reemplaza la tercera posición del arreglo con este valor.
4. Recorre el arreglo e imprímelo.

Un ejemplo de cómo se comportaría el programa en la consola sería el siguiente:

```
Ingresa un nombre> Camilo
Ingresa otro nombre> Ariel
Pedro
Pablo
Ariel
Juan
Diana
Camilo
```

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-18-js-julio/4073).//OK
Respuesta
```
let names=['Pedro','Pablo','Maria','Juan','Diana']

let addName=prompt('Ingrese su nombre')

names.push(addName)//añade elementos al array

console.log(names)

let addName1=prompt('Ingrese otro nombre')
names[2]=addName1

for(let i=0;i<names.length;i++){

console.log(names[i])
}
```
## Ejercicio 19

Escribe un programa que:

1. Le pida al usuario un número y cree un arreglo de números empezando en el 1 hasta el número que el usuario ingrese (incluyéndolo)
2. Elimine el segundo elemento.
3. Recorra e imprima el arreglo.

Ejemplo:

```
Ingresa un número> 5
1
3
4
5
```

**Nota:** los 3 pasos de este ejercicio se deben realizar con programación según lo visto en clase.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-19-js-julio/4074).//OK

Respuesta
```
let num=parseInt(prompt('Ingrese un numero'));
let conteo=[]
for(let i=0;i<num;i++){
 conteo.push(i+1)
}
// console.log(conteo)
conteo.splice(1,2)    //array.splice(start[, deleteCount[, item1[, item2[, ...]]]])
//Opcion
// for(let i=0;i<conteo.length;i++){
//   console.log(conteo[i])
}
//Opcion
for (num of conteo)(console.log(conteo)) //for/of : recorre los valores de un objeto iterable
```


## Ejercicio 20

Imprime la matriz en la consola, el resultado final debe ser el siguiente:

```javascript
const mat = [
  ["Pablo", "Maria", "Pedro"],
  ["Diana", "Juan", "Federico"],
  ["Roberto", "Daniel", "Sandra"]
];
```

```markdown
Grupo 1:
  Pablo
  Maria
  Pedro
Grupo 2:
  Diana
  Juan
  Federico
Grupo 3:
  Roberto
  Daniel
  Sandra
```

**Nota 1:** utiliza ciclos anidados para solucionar este ejercicio
**Nota 2:** agrega dos espacios al principio de cada nombre

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-20-js-julio/4076).//OK

Respuesta

```
const mat = [["Pablo", "Maria", "Pedro"],
  ["Diana", "Juan", "Federico"],
  ["Roberto", "Daniel", "Sandra"]
];
for(let i=0;i<mat.length;i++){      // ciclos anidados
  console.log('Grupo'+[i+1]+':');
  for(let j=0;j<mat.length;j++){
    console.log('  '+ mat[i][j])
  }
}
```
## Ejercicio 21

Completa el siguiente programa para imprimir los números que sean mayores a 10.

```javascript
const nums = [1, 23, 5, 8, 40, 12, 2, 67, 24, 9, 39]
// escribe tu código acá
```

El resultado debería ser el siguiente:

```
23
40
12
67
24
39
```

**Nota:** este ejercicio lo debes hacer con ciclos y sin ayuda de la función `filter` de JavaScript. Al terminarlo cambia el arreglo original para verificar que funcione con otros números.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-21-js-julio/4075).//OK

Respuesta

```
const nums = [1, 23, 5, 8, 40, 12, 2, 67, 24, 9, 39]
for(let i=0;i<nums.length;i++){
 if(nums[i]>=10)
  console.log(nums[i])
}
```
## Ejercicio 22

Completa el siguiente programa e imprime la cantidad de unos (1) que haya en el arreglo:

```javascript
const nums = [1, 0, 1, 1, 1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
```

El resultado debería ser el siguiente:

```
11
```

**Nota:** este ejercicio lo debes hacer con ciclos y sin ayuda de la función `filter` de JavaScript. Al terminarlo, cambia el arreglo original para verificar que funcione con otras combinaciones de ceros y unos.

Comparte tu respuesta [en este enlace](https://foro.makeitreal.camp/t/respuestas-ejercicio-22-js-julio/4077).//OK

Respuesta

const nums = [1, 0, 1, 1, 1, 0, 0, 1, 0, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1]
let conteo=0
for (let i=0;i<nums.length;i++){
  if(nums[i]==1){
  conteo=conteo+1
  }
 }
  console.log(conteo)
