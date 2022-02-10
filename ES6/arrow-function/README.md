# [JavaScript Arrow Function](https://www.w3schools.com/js/js_arrow_function.asp)

#### Arrow functions foram introduzidas no ES6 (2015). Elas permitem que desenvolvedores escrevam funções com uma sintaxe mais curta. Como por exemplo:

```
// Modo tradicional de criar funções no JavaScript.

function calcValues(firstValue, secondValue) {
  return firstValue + secondValue;
}

calcValues(10, 20); // 30
```

#### Ou também podemos escrever da seguinte forma.

```
const calcValues = function(firstValue, secondValue) {
  return firstValue + secondValue;
}

calcValues(50, 80); // 130
```

#### Agora utilizando a arrow function a sintaxe é muito parecida com a anterior.

```
const calcValues = (firstValue, secondValue) => {
  return firstValue + secondValue;
}

calcValues(50, 80); // 130
```

#### Embora as arrow functions já venham com uma sintaxe curta ainda assim podemos encurtar mais coisas. Como por exemplo:

```
// Podemos remover as chaves que definem o escopo de bloco da função e o return.

const calcValues = (firstValue, secondValue) => firstValue + secondValue;

// Caso você for receber somente um parâmetro também podemos remover os parênteses.

const calcValues = firstValue => firstValue * firstValue;
```
