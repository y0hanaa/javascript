
# Fundamentos do JavaScript Clássico

## PRIMEIROS PASSOS

- Criar arquivo ***index.html*** na raiz do projeto

``` bash

.
│ index.html

```

- Criar estrutura básica para arquivo ***index.html*** e executá-lo no navegador

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
  </head>
  <body></body>
</html>

```

## INTEGRAÇÕES

### Integrar **JavaScript** de forma interna ao arquivo ***index.html***

- Adicionar tag ***script*** à tag ***head***

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
    <script></script>
  </head>
  <body></body>
</html>

```

- Imprimir "Hello World" no console do navegador

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
    <script>
      console.log("Hello World!");
    </script>
  </head>
  <body></body>
</html>

```

- Adicionar atributo ***defer*** para adiar a exucução do script até que o e o DOM esteja completamente construído

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
    <script defer>
      console.log("Hello World!");
    </script>
  </head>
  <body></body>
</html>

```

- Adicionar tag ***script*** à tag ***body***

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
  </head>
  <body>
    <script></script>
  </body>
</html>

```

- Imprimir "Hello World" no console do navegador

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
  </head>
  <body>
    <script>
      console.log("Hello World!");
    </script>
  </body>
</html>

```

### Integrar **JavaScript** de forma externa ao arquivo ***index.html***

- Criar diretório ***src*** na raiz do projeto

``` bash

.
│ index.html
└─src

```

- Criar arquivo ***script.js*** na raiz do diretótio ***src***

``` bash

.
│ index.html
├─src
│   script.js

```

- Integrar arquivo ***script.js*** ao arquivo ***index.html*** através do atributo ***src*** adicionado à tag ***script***

``` html
./index.html

<!DOCTYPE html>

<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript</title>
  </head>
  <body>
    <script src="./src/script.js"></script>
  </body>
</html>

```

- Imprimir "Hello World" no console do navegador

``` javascript
./src/script.js

console.log("Hello World!");

```

## COMENTÁRIOS

### Comentário de linha

- Escrever comentário de linha

``` javascript
./src/script.js

// comentário de linha

```

### Comentário de bloco

- Escrever comentário de bloco simples

``` javascript
./src/script.js

/*
comentário de bloco
*/

```

- Escrever comentário de bloco com marcadores

``` javascript
./src/script.js

/**
 * comentário de bloco com marcadores
 */

```

## VARIÁVEIS

### Declaração

- Declarar variável com identificador ***number***

``` javascript
./src/script.js

var number;

```

### Atribuição de valor

- Atribuir valor à variável ***number***

``` javascript
./src/script.js

var number;

number = 5;

```

### Declaração e atribuição de valor

- Declarar e atribuir valor à variável ***number***

``` javascript
./src/script.js

var number = 5;

```

### Reatribuição de valor

- Reatribuir valor à variável ***number***

``` javascript
./src/script.js

var number = 5;

number = 10;

```

### Nomeclaturas

- Caracteres permitidos para iniciar a nomeclatura de um indetificador

``` javascript
./src/script.js

// letra
var number;
var Number;

// sublinhado
var _number;

// cifrão
var $number;

```

- Case-sensitive

``` javascript
./src/script.js

// "number" é diferente de "Number"

```

- Nomeclaturas compostas

``` javascript
./src/script.js

// camelCase
var myNumber;

// PascalCase
var MyNumber;

// snake_case
var my_number;

```

## TIPOS DE DADOS

### Primitivos

``` javascript
./src/script.js

// number
var age = 18;
var weight = 85.6;

// string
var name = "Yoh";
var surname = 'Pinheiro';

// boolean
var active = true;
var permission = false;

// undefined
var contains;
console.log(contains);

// null
var data = null;

```

### Não primitivos

``` javascript
./src/script.js

// array
var numbers = [1, 2, 3, 4, 5];

// object literal
var person = {
  name: "Yoh",
  age: 18
}

// function
var messege = function(){}

```

### Inspecionar tipo

``` javascript
./src/script.js

var number = 5;

console.log(typeof number);

```

### Coerção de tipo

#### Implícita

``` javascript
./src/script.js

var age = 18;
var weight = "85.6";

console.log(age + weight);

```

#### Explícita

``` javascript
./src/script.js

// Number()
var age = Number("18");
console.log(typeof age);

// Sctring()
var age = String(18);
console.log(typeof age);

// Boolean()
var number = Boolean(0);
console.log(number);

```

## Operadores

### Aritmético

``` javascript
./src/script.js

// adição
var a = 10;
var b = 5;
var result = a + b;
console.log(result);

// subtração
var a = 10;
var b = 5;
var result = a - b;
console.log(result);

// multiplicação
var a = 10;
var b = 5;
var result = a * b;
console.log(result);

// divisão 
var a = 10;
var b = 5;
var result = a / b;
console.log(result);

// módulo
var a = 10;
var b = 5;
var result = a % b;
console.log(result);

// incremento
var x = 5;
x++;
console.log(x);

// decremento
var x = 5;
x--;
console.log(x);

```

### Atribuição

``` javascript
./src/script.js

// simples
var name = "Yoh";

// atribuição de adição
var balance = 100;
balance += 50;
console.log(balance);

// atribuição de subtração
var balance = 100;
balance -= 50;
console.log(balance);

// atribuição de multiplicação
var balance = 100;
balance *= 50;
console.log(balance);

// atribuição de divisão
var balance = 100;
balance /= 50;
console.log(balance);

// atribuição de módulo
var balance = 100;
balance %= 50;
console.log(saldo);

```

### Comparação

``` javascript
./src/script.js

// igual
console.log(10 == "10");

// estritamente igual
console.log(10 === "10");

// diferente
console.log(10 != "10");

// estritamente diferente
console.log(10 !== "10");

// maior que
console.log(10 > 5);

// menor que
console.log(10 < 5);

// maior ou igual
console.log(10 >= 10);

// menor ou igual
console.log(10 <= 10);

```

### Lógicos

``` javascript
./src/script.js

// AND
var age = 18;
var license = true;
console.log(age >= 30 && license);

// OR
var age = 18;
var license = false;
console.log(age >= 30 || license);

// NOT
var active = true;
console.log(!active);

```

## Estruturas de Controle de Fluxo

### Estruturas Condicionais

### Truthy and Falsy

- **truthy**: tudo que não for ***falsy***

- **falsy**: "", 0, false, undefined, null, NaN

#### if

~~~ javascript
./src/script.js

if (5 == "5") {
  console.log("Executou.");
}

~~~

#### else

~~~ javascript
./src/script.js

if (5 == "5") {
  console.log("Verdadeiro.");
} else {
  console.log("Falso.");
}

~~~

#### else if

~~~ javascript
./src/script.js

var age = 65;

if (age > 60) {
  console.log("Aposentado.");
} else if (age > 30) {
  console.log("CLT.");
} else {
  console.log("Colleger.");
}

~~~

#### Operador ternário

~~~ javascript
./src/javascript.js

var age = 16;

age >= 18 ? console.log("Adult") : console.log("Minor.");

~~~

#### Curto-circuito lógico

~~~ javascript
./src/javascript.js

var licensed = false;

!licensed && console.log("Precisa tirar a carta de habilitação.");

~~~

#### switch case
~~~ javascript
./src/javascript.js

var light = "green";

switch (light) {
    case "red":
        console.log("Stop!");
        break;
    case "yellow":
        console.log("Attention!");
        break;
    case "green":
        console.log("Go!");
        break;
    default:
        console.log("Invalid color.");
}

~~~

### Estruturas de Repetição

#### for

~~~ javascript
./src/script.js

for (var n = 0; n <= 5; n++) {
  console.log("Number: " + n);
}

~~~

#### while

~~~ javascript
./src/script.js

var n = 0;

while (n <= 5) {
  console.log("Number: " + n);
  n++;
}

~~~

#### do while

~~~ javascript
./src/script.js

var n = 10;

do {
  console.log("Executed at least once.");
} while (n < 5)

~~~
