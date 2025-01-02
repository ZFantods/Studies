
# Conceitos Básicos de JavaScript

## 1. Variáveis e Tipos de Dados

- **Variáveis**: São usadas para armazenar dados. O JavaScript tem três formas de declarar variáveis: `var`, `let` e `const`.
  - `var`: Declara uma variável com escopo global ou de função. / Antigamente conhecida como `global` e não é recomendada na versão ES6 (ECMAScript 2015).
  - `let`: Declara uma variável com escopo de bloco.
  - `const`: Declara uma constante (não pode ser reatribuída).

  Exemplos:
  ```javascript
  let nome = "João";  // string
  const idade = 25;   // número
  const ativo = true; // booleano
  ```

- **Tipos de Dados Comuns**:
  - **Number**: números (inteiros e flutuantes).
  - **String**: strings (sequências de caracteres).
  - **Boolean**: valores booleanos (true/false).
  - **Object**: objetos (pares chave-valor).
  - **Array**: listas (coleções ordenadas de valores).
  - **undefined**: variável declarada, mas sem valor atribuído.
  - **null**: valor nulo (não aponta para nada).

## 2. Operadores

- **Aritméticos**:
  ```javascript
  let soma = 2 + 3;      // 5
  let subtracao = 5 - 3; // 2
  let multiplicacao = 4 * 3; // 12
  let divisao = 10 / 2;  // 5
  let potencia = 2 ** 3; // 8
  ```

- **Comparação**:
  ```javascript
  let a = 10;
  let b = 5;
  console.log(a == b);  // false
  console.log(a === b); // false (compara o tipo e o valor)
  console.log(a != b);  // true
  console.log(a > b);   // true
  console.log(a < b);   // false
  ```

- **Lógicos**:
  ```javascript
  let x = true;
  let y = false;
  console.log(x && y);  // false
  console.log(x || y);  // true
  console.log(!x);      // false
  ```

## 3. Estruturas de Controle

- **Condicionais (if, else if, else)**:
  ```javascript
  let idade = 20;
  if (idade < 18) {
      console.log("Menor de idade");
  } else if (idade === 18) {
      console.log("Maior de idade, recém completado");
  } else {
      console.log("Maior de idade");
  }
  ```

- **Laços (for, while)**:
  - **for**: Itera sobre uma sequência.
    ```javascript
    for (let i = 0; i < 5; i++) {
        console.log(i);  // Vai imprimir de 0 a 4
    }
    ```

  - **while**: Executa enquanto uma condição for verdadeira.
    ```javascript
    let contador = 0;
    while (contador < 5) {
        console.log(contador);
        contador++;
    }
    ```

## 4. Funções

Funções são blocos de código que realizam uma tarefa específica. Elas são definidas usando a palavra-chave `function`.
```javascript
function saudacao(nome) {
    return `Olá, ${nome}!`;
}

console.log(saudacao("João"));  // Saída: Olá, João!
```

## 5. Arrays

- Arrays são listas de valores. Eles podem conter elementos de diferentes tipos.
  ```javascript
  let lista = [1, 2, 3, 4];
  lista.push(5);  // Adiciona 5 ao final
  console.log(lista[0]);  // Acessa o primeiro elemento
  lista[1] = 10;  // Altera o valor do segundo elemento
  ```

## 6. Objetos

- Objetos são coleções de pares chave-valor.
  ```javascript
  let pessoa = { nome: "João", idade: 25 };
  console.log(pessoa.nome);  // Acessa o valor da chave 'nome'
  pessoa.idade = 26;         // Atualiza o valor da chave 'idade'
  ```

## 7. Funções de Callback e Arrow Functions

- **Funções de Callback**: Funções passadas como argumento para outra função.
  ```javascript
  function saudacao(nome, callback) {
      callback(`Olá, ${nome}!`);
  }

  saudacao("João", (mensagem) => {
      console.log(mensagem);  // Saída: Olá, João!
  });
  ```

- **Arrow Functions**: Sintaxe curta para funções anônimas.
  ```javascript
  const somar = (a, b) => a + b;
  console.log(somar(2, 3));  // 5
  ```

## 8. Manipulação de Strings

- Strings são usadas para representar texto.
  ```javascript
  let texto = "Olá, Mundo!";
  console.log(texto.toUpperCase());  // "OLÁ, MUNDO!"
  console.log(texto.toLowerCase());  // "olá, mundo!"
  console.log(texto.replace("Mundo", "JavaScript"));  // "Olá, JavaScript!"
  ```

## 9. Exceções (Tratamento de Erros)

- O JavaScript permite capturar erros usando `try...catch`.
  ```javascript
  try {
      let x = 10 / 0;
  } catch (error) {
      console.log("Erro: ", error.message);
  }
  ```
