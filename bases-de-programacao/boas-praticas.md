# 📌 Nomes de Variáveis e Funções

### ✒️ Evite más práticas:
- Evite nomes genéricos como `i, j, k, x, y, z`.
- Evite nomes que não explicam o que representam, como `buga, foo, bar`.
- Evite nomes muito genéricos, como `contador` (contador do quê?).
- Evite nomes longos e complexos, como `CorAzulDoCeuDasNuvensDaTerra`.
- Evite nomes inconsistentes em diferentes partes do código, como `CorAzul`, `corAzul`, `cor_azul`.
- Sempre prefira nomes que expliquem a função da variável ou método.
- **Use nomes descritivos e consistentes** (código autoexplicativo).

---

# 📌 Convenções de Nomenclatura

## ✅ CamelCase
📌 **Descrição:** Primeira palavra minúscula, as seguintes com inicial maiúscula. 
🔹 **Usado para:** Funções, variáveis e métodos. 

🛠️ **Linguagens:** JavaScript, Java, C#, C++, Swift, Go, Ruby, PHP.

💡 **Exemplos:**
```js
minhaVariavel
calcularSoma()
```

---

## ✅ PascalCase
📌 **Descrição:** Similar ao CamelCase, mas a primeira letra também é maiúscula.
🔹 **Usado para:** Classes e tipos de dados.

🛠️ **Linguagens:** C#, Java, C++, Swift, TypeScript, JavaScript (classes).

💡 **Exemplos:**
```js
Pessoa
ContaBancaria
```

---

## ✅ snake_case
📌 **Descrição:** Palavras separadas por `_`, todas em minúsculas.
🔹 **Usado para:** Variáveis, funções e arquivos.

🛠️ **Linguagens:** Python, Ruby, PHP, Elixir, Perl.

💡 **Exemplos:**
```py
minha_variavel
calcular_soma()
```

---

## ✅ UPPER_CASE
📌 **Descrição:** Letras maiúsculas com `_` separando palavras.
🔹 **Usado para:** Constantes.

🛠️ **Linguagens:** C, C++, JavaScript, Python, Go.

💡 **Exemplos:**
```js
PI = 3.14159
MAX_VALOR = 100
```

---

## ✅ kebab-case
📌 **Descrição:** Letras minúsculas separadas por `-`.
🔹 **Usado para:** Arquivos, URLs.

🛠️ **Linguagens:** JavaScript, Ruby, CSS.

💡 **Exemplos:**
```
nome-do-arquivo.js
minha-aplicacao
```

---

# 📌 Estrutura de Pastas 📁
Boas práticas na organização do código-fonte.

```
📦 meu-projeto
 ┣ 📂 src ➜ Código-fonte principal
 ┃ ┣ 📂 components ➜ Componentes reutilizáveis
 ┃ ┣ 📂 services ➜ Requisições e regras de negócio
 ┃ ┣ 📂 utils ➜ Funções auxiliares
 ┃ ┣ 📂 styles ➜ Arquivos de estilo (CSS, SASS, etc.)
 ┃ ┗ 📜 index.js ➜ Arquivo principal
 ┣ 📂 assets ➜ Imagens, fontes e outros recursos estáticos
 ┣ 📂 tests ➜ Testes unitários e de integração
 ┣ 📂 public ➜ Arquivos estáticos (HTML, imagens, etc.)
 ┣ 📂 config ➜ Configurações e variáveis de ambiente
 ┣ 📜 README.md ➜ Documentação do projeto
 ┣ 📜 package.json ➜ Dependências e scripts
 ┣ 📜 .gitignore ➜ Arquivos ignorados pelo Git
```

---

# 📌 Nomes que NÃO podem ser usados 🚫

- **Palavras reservadas da linguagem:** `class`, `function`, `return`, `if`, `else`, etc.
- **Caracteres especiais não permitidos:** Evite caracteres como `@, #, $, %, &, *` em nomes de variáveis.
- **Espaços em branco:** Use `_` ou `-` em vez de espaços.
- **Nomes duplicados:** Evite nomes idênticos em diferentes partes do código, o que pode causar conflitos.

---

# 📌 Referências 📚
- [Clean Code: A Handbook of Agile Software Craftsmanship](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882) - Robert C. Martin.
- [Self-Documenting Code](https://en.wikipedia.org/wiki/Self-documenting_code).
- [Meaningful Names](https://en.wikipedia.org/wiki/Meaningful_name).

🚀 **Mantenha seu código limpo, organizado e fácil de entender!**

