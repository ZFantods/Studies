
# Conceitos Básicos de Python

## 1. Variáveis e Tipos de Dados

- **Variáveis**: São usadas para armazenar dados. Não é necessário declarar o tipo da variável, pois o Python é uma linguagem dinamicamente tipada.
  ```python
  nome = "João"  # string
  idade = 25      # inteiro
  altura = 1.75   # ponto flutuante
  ativo = True    # booleano
  ```

- **Tipos de Dados Comuns**:
  - **int**: números inteiros.
  - **float**: números decimais.
  - **str**: strings (sequência de caracteres).
  - **bool**: valores booleanos (True/False).
  - **list**: listas (sequências mutáveis de valores).
  - **tuple**: tuplas (sequências imutáveis).
  - **dict**: dicionários (pares chave-valor).

## 2. Operadores

- **Aritméticos**:
  ```python
  soma = 2 + 3       # 5
  subtracao = 5 - 3  # 2
  multiplicacao = 4 * 3  # 12
  divisao = 10 / 2   # 5.0
  divisao_inteira = 10 // 3  # 3
  resto = 10 % 3     # 1
  potencia = 2 ** 3  # 8
  ```

- **Comparação**:
  ```python
  a = 10
  b = 5
  print(a == b)  # False
  print(a != b)  # True
  print(a > b)   # True
  print(a < b)   # False
  ```

- **Lógicos**:
  ```python
  x = True
  y = False
  print(x and y)  # False
  print(x or y)   # True
  print(not x)    # False
  ```

## 3. Estruturas de Controle

- **Condicionais (if, elif, else)**:
  ```python
  idade = 20
  if idade < 18:
      print("Menor de idade")
  elif idade == 18:
      print("Maior de idade, recém completado")
  else:
      print("Maior de idade")
  ```

- **Laços (for, while)**:
  - **for**: Itera sobre uma sequência (lista, string, etc.).
    ```python
    for i in range(5):
        print(i)  # Vai imprimir de 0 a 4
    ```

  - **while**: Executa enquanto uma condição for verdadeira.
    ```python
    contador = 0
    while contador < 5:
        print(contador)
        contador += 1
    ```

## 4. Funções

Funções são blocos de código que realizam uma tarefa específica. Elas são definidas usando a palavra-chave `def`.
```python
def saudacao(nome):
    return f"Olá, {nome}!"

print(saudacao("João"))  # Saída: Olá, João!
```

## 5. Listas

- Listas são coleções ordenadas e mutáveis de itens.
  ```python
  lista = [1, 2, 3, 4]
  lista.append(5)  # Adiciona 5 ao final
  print(lista[0])  # Acessa o primeiro elemento
  lista[1] = 10    # Altera o valor do segundo elemento
  ```

## 6. Dicionários

- Dicionários são coleções de pares chave-valor.
  ```python
  pessoa = {"nome": "João", "idade": 25}
  print(pessoa["nome"])  # Acessa o valor associado à chave 'nome'
  pessoa["idade"] = 26  # Atualiza o valor da chave 'idade'
  ```

## 7. Importando Bibliotecas

- Você pode usar bibliotecas externas em Python para adicionar funcionalidades.
  ```python
  import math
  print(math.sqrt(16))  # 4.0
  ```

## 8. Manipulação de Strings

- As strings são usadas para representar texto.
  ```python
  texto = "Olá, Mundo!"
  print(texto.upper())  # "OLÁ, MUNDO!"
  print(texto.lower())  # "olá, mundo!"
  print(texto.replace("Mundo", "Python"))  # "Olá, Python!"
  ```

## 9. Exceções (Tratamento de Erros)

- O Python permite capturar erros para evitar que o programa quebre.
  ```python
  try:
      x = 10 / 0
  except ZeroDivisionError:
      print("Não é possível dividir por zero.")
  ```
