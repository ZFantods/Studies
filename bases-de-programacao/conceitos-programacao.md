# Conceitos de Lógica de Programação, Objetos e Outros

## 1. Lógica de Programação (Logical Programming)

Lógica de programação é a capacidade de pensar e planejar como um programa vai funcionar. Consiste em entender problemas e transformá-los em soluções que possam ser executadas por um computador.

### Estruturas Lógicas (Logical Structures)

- **Sequência (Sequence)**: A execução de comandos de forma linear, um após o outro.
  - Exemplo: 
    ```plaintext
    1. Iniciar
    2. Ler dados
    3. Processar dados
    4. Mostrar resultado
    5. Fim
    ```

- **Condicional (Conditional)**: Permite que o programa tome decisões com base em condições.
  - Exemplo:
    ```plaintext
    Se (idade >= 18) então
        Mostrar "Maior de idade"
    Senão
        Mostrar "Menor de idade"
    ```

- **Laços (ou Repetição) [Loops]**: Permite que o programa repita uma ação várias vezes, enquanto uma condição for verdadeira.
  - Exemplo:
    ```plaintext
    Enquanto (x < 10) faça
        Imprimir "x"
        Incrementar x
    ```

### Algoritmos (Algorithms)

- **Algoritmo**: Conjunto de instruções ou passos para resolver um problema específico. A lógica de programação ajuda a criar algoritmos eficazes.

## 2. Objetos e Programação Orientada a Objetos (POO - Object-Oriented Programming)

A programação orientada a objetos é um paradigma de programação baseado na organização do código em "objetos", que são instâncias de classes.

### Objetos (Object)

- **Objetos**: São entidades que contêm tanto dados (atributos) quanto comportamentos (métodos). Cada objeto é uma instância de uma classe.
  - Exemplo: Um "carro" pode ser um objeto com atributos como `modelo`, `cor`, `ano` e métodos como `acelerar()` e `frear()`.

### Classes (Class)

- **Classe**: É um modelo ou um "molde" para criar objetos. Define os atributos e métodos que os objetos dessa classe terão.
  - Exemplo:
    ```python
    class Carro:
        def __init__(self, modelo, cor, ano):
            self.modelo = modelo
            self.cor = cor
            self.ano = ano

        def acelerar(self):
            print(f"O {self.modelo} está acelerando!")

        def frear(self):
            print(f"O {self.modelo} está frenando!")
    ```

### Encapsulamento (Encapsulation)

- **Encapsulamento**: Esconde os detalhes internos do funcionamento de uma classe e só expõe o necessário. Isso é feito por meio de atributos privados e métodos públicos.
  - Exemplo: 
    ```python
    class ContaBancaria:
        def __init__(self, saldo=0):
            self.__saldo = saldo  # Atributo privado

        def depositar(self, valor):
            if valor > 0:
                self.__saldo += valor
            else:
                print("Valor inválido")

        def obter_saldo(self):
            return self.__saldo
    ```

### Herança (Inheritance)

- **Herança**: Permite que uma classe herde atributos e métodos de outra, facilitando o reuso de código. 
  - Exemplo:
    ```python
    class Veiculo:
        def __init__(self, modelo, cor):
            self.modelo = modelo
            self.cor = cor

        def acelerar(self):
            print(f"{self.modelo} está acelerando!")

    class Carro(Veiculo):  # Herda de Veiculo
        def __init__(self, modelo, cor, portas):
            super().__init__(modelo, cor)
            self.portas = portas
    ```

### Polimorfismo (Polymorphism)

- **Polimorfismo**: Permite que métodos com o mesmo nome se comportem de maneira diferente em classes diferentes. 
  - Exemplo:
    ```python
    class Animal:
        def emitir_som(self):
            pass

    class Cachorro(Animal):
        def emitir_som(self):
            print("Au Au")

    class Gato(Animal):
        def emitir_som(self):
            print("Miau")
    ```

## 3. Algoritmos e Estruturas de Dados (Algorithms and Data Structures)

### Algoritmos de Busca (Search Algorithms)

- **Busca Linear (Linear Search)**: Consiste em percorrer uma lista de elementos e verificar cada um, até encontrar o item desejado.
  - Exemplo de código em Python:
    ```python
    def busca_linear(lista, item):
        for i in range(len(lista)):
            if lista[i] == item:
                return i
        return -1
    ```

- **Busca Binária (Binary Search)**: Utiliza uma lista ordenada e divide a lista ao meio a cada comparação, o que a torna mais eficiente que a busca linear.
  - Exemplo:
    ```python
    def busca_binaria(lista, item):
        baixo = 0
        alto = len(lista) - 1
        while baixo <= alto:
            meio = (baixo + alto) // 2
            chute = lista[meio]
            if chute == item:
                return meio
            if chute > item:
                alto = meio - 1
            else:
                baixo = meio + 1
        return -1
    ```

### Estruturas de Dados Comuns

- **Listas (Lists)**: São coleções ordenadas de elementos.
  - Exemplo de lista:
    ```python
    lista = [1, 2, 3, 4]
    lista.append(5)
    ```

- **Pilhas (Stacks)**: Estrutura de dados onde o último item inserido é o primeiro a ser retirado (LIFO - Last In, First Out).
  - Exemplo de pilha:
    ```python
    pilha = []
    pilha.append(1)  # Adiciona
    pilha.pop()      # Remove
    ```

- **Filas (Queues)**: Estrutura de dados onde o primeiro item inserido é o primeiro a ser retirado (FIFO - First In, First Out).
  - Exemplo de fila:
    ```python
    fila = []
    fila.append(1)  # Enfileira
    fila.pop(0)     # Desenfileira
    ```

## 4. Funções e Recursão

- **Função (Function)**: Bloco de código que pode ser chamado para executar uma tarefa específica. Ela pode ter parâmetros e retornar valores.
  - Exemplo:
    ```python
    def soma(a, b):
        return a + b
    ```

- **Recursão (recursion)**: Técnica onde uma função chama a si mesma para resolver um problema. Muito usado em algoritmos de busca.
  - Exemplo:
    ```python
    def fatorial(n):
        if n == 0:
            return 1
        else:
            return n * fatorial(n - 1)
    ```


