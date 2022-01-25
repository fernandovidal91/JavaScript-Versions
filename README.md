# The let keyword (A palavra-chave let)

#### A palavra `let` permite declarar uma variável com escopo de bloco, ou seja, caso a declare dentro de uma `function` ou dentro de um `if` seu valor ira valer somente para aquele bloco. Seu valor também e mutável, permitindo a alteração do mesmo ao executar determinado bloco de código.

```
let name = 'Fernando';

function calc() {
    let numberOne = 10;
    let numberTwo = 20;
    let result = numberOne + numberTwo;

    console.log({ numberOne, numberTwo, result, name })

    result = numberOne * numberTwo;

    console.log('Resultado multiplicado ' + result)
}

calc();
// {numberOne: 10, numberTwo: 20, result: 30, name: 'Fernando'}
// Resultado multiplicado 200

console.log(name);
// Fernando

console.log({ numberOne, numberTwo, result })
// Uncaught ReferenceError: numberOne is not defined
// Uncaught ReferenceError: numberTwo is not defined
// Uncaught ReferenceError: result is not defined
```

# The const keyword (A palavra-chave const)
#### A palavra `const` permite declarar uma variável com escopo de bloco, ou seja, caso a declare dentro de uma `function` ou dentro de um `if` seu valor ira valer somente para aquele bloco. Seu valor não e mutável, não permitindo a alteração do mesmo ao executar determinado bloco de código.

```
const name = 'Fernando';

function calc() {
    const numberOne = 10;
    const numberTwo = 20;
    const result = numberOne + numberTwo;

    console.log({ numberOne, numberTwo, result, name })

    result = numberOne * numberTwo; // Uncaught TypeError: Assignment to constant variable.

    console.log('Resultado multiplicado ' + result)
}

calc();
// {numberOne: 10, numberTwo: 20, result: 30, name: 'Fernando'}

console.log(name);
// Fernando

console.log({ numberOne, numberTwo, result })
// Uncaught ReferenceError: numberOne is not defined
// Uncaught ReferenceError: numberTwo is not defined
// Uncaught ReferenceError: result is not defined
```
