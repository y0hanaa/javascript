# Fundamentos do JavaScript Clássico

## INTEGRAÇÕES

### Integrar JavaScript de forma interna

~~~ html
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
        console.log("Hello Word!");
    </script>
</body>
</html>
~~~

### Integrar JavaScript de forma externa

- Criar diretório ***src*** na raiz do projeto
- Criar arquivo ***script.js*** na raiz do diretório ***src***
- Integrar de forma externa o arquivo ***script.js*** no arquivo ***index.html***


~~~ html
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
        console.log("Hello Word!");
    </script>
</body>
</html>
~~~

## COMENTÁRIOS

### Comentário de linha

~~~ javascript

// Comentário de linha

~~~

### Comentário de bloco simples

~~~ javascript

// Comentário de bloco simples */

~~~

### Comentário de bloco com marcadores

~~~ javascript

/** 
 * Comentário de bloco com marcador
*/

~~~ 



## VARIÁVEIS

### Declaração

~~~ javascript
./src/script.js

var number;

~~~

### Atribuição de valor

~~~ javascript
./src/script.js

var number;

number = 5;

~~~

### Declaração e atribuição de valor

~~~ javascript
./src/script.js

number = 5;

~~~

### Reatribuição de valor
~~~ javascript
./src/script.js

var number = 5;

number = 10;

~~~

### Nomenclaturas

- Caracteres permitidos para iniciar a nomenclatura de um indentificador

~~~ javascript
./src/script.js

//letras
var number;
var Number;

//sublinhado
var = _number;

//sifrão
var $number;

~~~

- Case-sensitive
~~~ javascript
./src/script.js

// "number" é diferente de "Number"

~~~

- Nomenclaturas compostas

~~~ javascript
./src/script.js

// camel case
var myName;

// pascal case
var MyName;

// snake case
var my_name;

~~~

## TIPOS DE DADOS

### Primitivos

~~~ javascript
./src/script.js

// string
var name = "Yoh"; 
var surname = 'Pinheiro';

// number
var age = 18;
var weight = 85.6;

// boolean
var active = true;
var permission = false;

// undefined
var contains;
console.log(contains);

// null
var data = null;

~~~

### Não Primitivos

~~~ javascript
./src/script.js

// array
 var values = [1, Yoh, true, null];

// Object literal
var person = {name: "Yoh", age:18};

var person = {
    name: "Yoh",
    age: 18
};

// function

var message = function(){};


## Estruturas de controle de fluxo

### Estruturas condicionais

### Truthy and Falsy

- **Truthy**: tudo que não for **falsy**

- **Falsy**: "", 0, false, undefined, null, NaN;

#### IF

~~~ javascript
./src/script.js

if (5 == "5") {
    console.log("Executou");
}

~~~ 

#### Else

~~~ javascript
./src/script.js

if (5 == "5") {
    console.log("Verdadeiro.");
} else {
    console.log("falso.");
}

~~~ 

#### Else if

~~~ javascript
./src/script.js

var age = 65;

if (age > 60) {
    console.log("Aposentado.");
} else if (age > 30){
    console.log("CLT.");
} else {
    console.log("Colleger.");
}

~~~ 

#### Operador ternário

~~~ javascript
./src/javascript.js

var age = 16;

age >= 18 ? console.log("Adult) : console.log("Minor);

~~~ 

#### Curto-circuito lógico

~~~ javascript
./src/javascript.js

var licensed = false;

!licensed && console.log("Precisa tirar carta de habilitação"); 

~~~ 
#### Switch case

~~~ javascript
./src/javascript.js

var light = "green";

switch (light) {
    case "red":
        console.log("Stop!");
        break
    case "yellow":
        console.log("attention!");
        break
    case "green":
        console.log("go!");
        break
    default:
        console.log("invalid color.");
}
~~~ 