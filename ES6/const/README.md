# [JavaScript const keyword](https://www.w3schools.com/js/js_const.asp)

#### A palavra-chave `const` foi introduzida no ES6 (2015). Este tipo de variável é muito utilizada quando necessitamos criar um valor constante onde não é possível alterar seu valor. Caso o desenvolver tente reatribuir um valor para a variável a mensagem `(TypeError: Assignment to constant variable)` é exibida no console.

```
const userName = 'Fernando';

console.log(userName); // Fernando

userName = 'Fernando Angiolin Vidal'; // Error: Assignment to constant variable.
```

#### Uma característica importante sobre as variáveis criadas utilizando o `const` é que seu valor é valido somente no escopo em que foi criada.


```
const userName = 'Fernando';

console.log(userName); // Fernando

{
  const petName = 'Pé de pano';

  console.log({
    userName,
    petName
  }); // { userName: 'Fernando', petName: 'Pé de pano' }
}

console.log({
  userName,
  petName
}); // Error: petName is not defined

// O código a cima retorna um erro pois petName não foi declarado no escopo principal.
```
