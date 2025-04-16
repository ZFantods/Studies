
# 📐 Números Matemáticos em JavaScript

JavaScript oferece suporte nativo para operações matemáticas usando o tipo primitivo `number`. Com ele, é possível trabalhar com números inteiros, decimais, positivos, negativos, e realizar operações aritméticas básicas ou avançadas.

## 🧮 Tipos de Números

Em JavaScript, todos os números são tratados como `number`, independente de serem inteiros ou ponto flutuante:

```js
let inteiro = 10;
let decimal = 3.14;
let negativo = -42;
```

## ➕ Operadores Aritméticos

| Operação      | Símbolo | Exemplo     | Resultado |
|---------------|---------|-------------|-----------|
| Adição        | `+`     | `5 + 3`     | `8`       |
| Subtração     | `-`     | `5 - 3`     | `2`       |
| Multiplicação | `*`     | `5 * 3`     | `15`      |
| Divisão       | `/`     | `10 / 2`    | `5`       |
| Módulo        | `%`     | `10 % 3`    | `1`       |
| Exponenciação | `**`    | `2 ** 3`    | `8`       |

## 📏 Métodos Úteis de Math

O objeto `Math` oferece várias funções para cálculos matemáticos:

```js
Math.round(4.7);     // Arredonda para o inteiro mais próximo → 5
Math.ceil(4.3);      // Arredonda para cima → 5
Math.floor(4.9);     // Arredonda para baixo → 4
Math.abs(-10);       // Valor absoluto → 10
Math.sqrt(16);       // Raiz quadrada → 4
Math.pow(2, 4);      // Potência → 16
Math.random();       // Número aleatório entre 0 e 1
```

## 📉 Cuidados com Decimais

Devido à forma como números de ponto flutuante são representados, certas operações podem ter resultados imprecisos:

```js
0.1 + 0.2 === 0.3  // false 😱
```

Para contornar isso, uma abordagem comum é arredondar os valores:

```js
let resultado = (0.1 + 0.2).toFixed(2);  // "0.30"
```

## 📌 Extras

Você pode converter strings para números usando `parseInt()`, `parseFloat()` ou o operador `+`. E verificar se algo **não é um número** com `isNaN()`:

```js
parseInt("10");      // 10
parseFloat("3.14");  // 3.14
+"42"                // 42
isNaN("hello")       // true
```

---

# 📊 Números Avançados em JavaScript

Além das operações básicas, o JavaScript possui funcionalidades mais avançadas para lidar com números, como `BigInt`, verificação de tipos, limites numéricos e manipulação precisa de valores.

## 🔢 BigInt

`BigInt` é um tipo primitivo que permite representar números inteiros muito grandes, além do limite do tipo `Number`.

```js
const numeroGrande = 1234567890123456789012345678901234567890n;
const outroBigInt = BigInt("987654321987654321987654321");

console.log(numeroGrande + 1n); // Funciona com outros BigInts
```

⚠️ Não é possível misturar `BigInt` com `Number` diretamente:

```js
const n = 10n + BigInt(5); // OK
const erro = 10n + 5;      // ❌ TypeError
```

## ✅ Verificações Numéricas

JavaScript possui formas modernas de validar e verificar números:

```js
Number.isInteger(10);           // true
Number.isFinite(100);           // true
Number.isNaN(NaN);              // true
Number.isSafeInteger(9007199254740991); // true
```

## 🔍 Limites Numéricos

```js
console.log(Number.MAX_VALUE);           // Maior número representável
console.log(Number.MIN_VALUE);           // Menor número positivo representável
console.log(Number.MAX_SAFE_INTEGER);    // Maior inteiro seguro
console.log(Number.MIN_SAFE_INTEGER);    // Menor inteiro seguro
```

## ♾️ Infinity e -Infinity

```js
1 / 0;         // Infinity
-1 / 0;        // -Infinity
Infinity > 999999999999; // true
```

## 🧪 Precisão com Bibliotecas

Para cálculos financeiros ou precisos, é recomendável usar bibliotecas como:

- [Decimal.js](https://mikemcl.github.io/decimal.js/)
- [Big.js](https://github.com/MikeMcl/big.js/)
- [Math.js](https://mathjs.org/)

Exemplo com `Decimal.js`:

```js
const Decimal = require("decimal.js");
const resultado = new Decimal(0.1).plus(0.2);
console.log(resultado.toString()); // "0.3"
```

## 🌐 Conversão Avançada de Tipos

```js
Number("42");        // 42
parseInt("1010", 2); // 10 (binário para decimal)
Number(true);        // 1
Number(false);       // 0
Number(null);        // 0
Number(undefined);   // NaN
```

---