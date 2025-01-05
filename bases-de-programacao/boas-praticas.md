# 0. Nomes de variáveis e funções ✒️

##### Evite usar nomes de variáveis e funções com nomes comuns, pois podem ser confundidos com outros nomes.
- Exemplo: i, j, k, x, y, z.
##### Evite usar nomes de variáveis e funções que não expliquem o que a variável ou função representa.
- Exemplo: BUGA, BUGA, buga.
##### Evite usar nomes de variáveis e funções que não descrevem o que a variável ou função faz.
- Exemplo: contador. Contador do que?	
##### Evite usar nomes de variáveis e funções que são muito longos ou complexos.
- Exemplo: CorAzulDoCeuDasNuvensDaTerra.
##### Evite usar nomes de variáveis e funções que são repetidos em vários lugares do código.
- Exemplo: CorAzul, corAzul, cor_azul.
##### Evite usar nomes de variáveis e funções que não são úteis para a compreensão do código.
- Exemplo: Zé do céu, Zé da terra, Zé da Terra.
##### Nomes de variáveis e funções devem ser escritos em inglês ou em sua língua nativa para trazer mais clareza ao código.

## Consistência e Clareza
 **Descrição**: Seja consistente em todo o seu código e utilize nomes descritivos. "[self-documenting](https://en.wikipedia.org/wiki/Self-documenting_code)".
- Exemplo: Se utilizar `totalPreco`, use sempre `totalPreco`, não altere para `precoTotal`.

## Abreviações
**Descrição**: Evite abreviações a menos que sejam amplamente compreendidas. "[meaningful names](https://en.wikipedia.org/wiki/Meaningful_name)".
Exemplo: Em vez de `tmpVar`, use `variavelTemp`.

# Convenções de Nomenclatura por Linguagem 💬

## 1. CamelCase

### Descrição:
- A primeira palavra começa com letra minúscula e as palavras subsequentes começam com letras maiúsculas.
- Usada principalmente para funções, variáveis e métodos.

### Linguagens que usam:
- **JavaScript**
- **Java**
- **C#**
- **C++**
- **Swift**
- **Go**
- **Ruby**
- **PHP** (para variáveis, funções e métodos)

### Exemplos:
- `minhaVariavel`
- `calcularSoma()`

---

## 2. PascalCase

### Descrição:
- Semelhante ao CamelCase, mas a primeira letra também é maiúscula.
- Usada principalmente para classes e tipos de dados.

### Linguagens que usam:
- **C#**
- **Java**
- **C++**
- **Swift**
- **TypeScript**
- **JavaScript** (para classes e interfaces)

### Exemplos:
- `Pessoa`
- `ContaBancaria`

---

## 3. snake_case

### Descrição:
- As palavras são separadas por underscores (`_`), com todas as letras minúsculas.
- Usada principalmente para variáveis, funções e arquivos.

### Linguagens que usam:
- **Python**
- **Ruby**
- **PHP** (para variáveis e funções)
- **Elixir**
- **Perl**

### Exemplos:
- `minha_variavel`
- `calcular_soma()`

---

## 4. UPPERCASE

### Descrição:
- Todas as letras são maiúsculas, com palavras separadas por underscores (`_`).
- Usada para constantes ou variáveis que não devem ser modificadas.

### Linguagens que usam:
- **C**
- **C++**
- **JavaScript**
- **Python**
- **Go**

### Exemplos:
- `PI = 3.14159`
- `MAX_VALOR = 100`

---

## 5. kebab-case

### Descrição:
- As palavras são separadas por hífens (`-`), com todas as letras minúsculas.
- Usada principalmente para nomes de arquivos e URLs.

### Linguagens que usam:
- **JavaScript** (principalmente em pacotes, arquivos e URLs)
- **Ruby** (para alguns casos de arquivos e métodos)
- **CSS** (para propriedades e IDs)

### Exemplos:
- `nome-do-arquivo.js`
- `minha-aplicacao`

---

## 6. StudlyCaps

### Descrição:
- Variantes do CamelCase onde as letras podem alternar entre maiúsculas e minúsculas de maneira irregular.
- Geralmente considerada uma prática ruim, mas ocasionalmente utilizada em algumas linguagens para nomes de classes ou variáveis que precisam se destacar.

### Linguagens que usam:
- **JavaScript** (em alguns casos de bibliotecas e frameworks)
- **PHP** (em alguns padrões antigos de código)

### Exemplos:
- `MinhaVariable`
- `MinhaClasseDeTeste`

