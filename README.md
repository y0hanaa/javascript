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