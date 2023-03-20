# M06ExemplesClase

ForEach, Map, Reduce, Some, Every, Filter

```javascript

//Mi array de ejemplo
let miLista = [4, 2, 1, 6, 1, 22, 12];

console.info("----- FOREACH -----");
//Imprime todos los elementos
miLista.forEach(e => { console.log(e) });

console.info("----- MAP -----");
//Multiplica cada elemento de la array *3
console.log(miLista.map((e) => e * 3));
//Suma cada elemento de la array + 2
console.log(miLista.map((e) => e + 2));

console.info("----- REDUCE -----");
//Todos los elementos se suma
console.log(miLista.reduce((e, acumulador) => e + acumulador));
//Todos los elementos se multiplican
console.log(miLista.reduce((e, acumulador) => e * acumulador));

console.info("----- SOME -----");
//Hay algun elementos impar
console.log(miLista.some(e => e % 2 !== 0));
//Hay algun numero menor a 10
console.log(miLista.some(e => e < 10));

console.info("----- EVERY -----");
//Todos los elementos son impares
console.log(miLista.every(e => e % 2 !== 0));
//Todos los elementos son menores a 10
console.log(miLista.every(e => e < 10));

console.info("----- FILTER -----");
//Devuelve todos los elementos mayor a 10
console.log(miLista.filter(e => e > 10));
//Devuelve todos los elementos menor a 20
console.log(miLista.filter(e => e < 20));



console.info("---- EXTRA ----");
//Cada funcion tiene una funcion dentro, la puedo extraer

//Funcion en una variable 
let condition1 = function (e) { return e > 10 }
console.log(miLista.filter(condition1));

//Funcion anonima en una variable 
let condition2 = (e) => e > 10;
console.log(miLista.filter(condition2));

//Funcion y directamente llamo a la funcion, IMPORTANTE, SIN '()'
function condition3(e) { return e > 10; }
console.log(miLista.filter(condition3));
```
