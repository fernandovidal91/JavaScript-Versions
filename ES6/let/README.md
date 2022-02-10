# [JavaScript let keyword](https://www.w3schools.com/js/js_let.asp)

#### A palavra-chave `let` foi introduzida no ES6 (2015). Este tipo de variável é muito utilizado quando necessitamos reatribuir seu valor, como no exemplo a seguir.

```
let userName = 'Fernando';

console.log(userName); // Fernando

userName = 'Fernando Angiolin Vidal';

console.log(userName); // Fernando Angiolin Vidal
```

#### Uma característica importante sobre as variáveis criadas utilizando o `let` é que seu valor é valido somente no escopo em que foi criada.

```
let userName = 'Fernando';

console.log(userName); // Fernando

{
  let petName = 'Pé de pano';

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
