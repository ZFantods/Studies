🎨 | Pseudo-classes no CSS  

As pseudo-classes são utilizadas para definir um estado especial de um elemento HTML, permitindo criar interações dinâmicas sem precisar de JavaScript. Elas ajudam a melhorar a experiência do usuário, tornando a navegação mais intuitiva.  

🔹 **O que são pseudo-classes?**  
Uma pseudo-classe é adicionada ao final de um seletor e permite aplicar estilos baseados no estado do elemento. Isso possibilita, por exemplo, destacar um botão quando o mouse passa sobre ele ou estilizar links já visitados.  

🔸 **Principais pseudo-classes:**  

☑️ `:focus` – Aplica um estilo quando o elemento está em foco.  
   📌 Exemplo: Um campo de formulário muda de cor quando o usuário clica nele.  

☑️ `:hover` – Ativado quando o mouse está sobre o elemento.  
   📌 Exemplo: Um botão muda de cor ao passar o cursor sobre ele.  

☑️ `:active` – Aplica um estilo enquanto o elemento está sendo pressionado.  
   📌 Exemplo: Um link muda de cor enquanto está sendo clicado.  

☑️ `:visited` – Define estilos para links que já foram acessados.  
   📌 Exemplo: Links clicados aparecem em uma cor diferente para diferenciar dos não visitados.  

☑️ `:link` – Aplica estilos a links que ainda não foram acessados.  
   📌 Exemplo: Links novos aparecem com uma cor específica antes do primeiro clique.  

💡 **Dica:** Combine pseudo-classes para criar interações mais ricas e responsivas!  

```css
a:hover {
    color: purple; /* Muda a cor do link ao passar o mouse */
}

input:focus {
    border: 2px solid blue; /* Destaca campos de formulário quando selecionados */
}
```  

# Pseudo-classes CSS: Detalhamento Completo

## 2. Pseudo-classes Básicas

Essas são as pseudo-classes mais comuns usadas para estilizar elementos com base em diferentes interações do usuário. Elas são usadas para aumentar a interatividade de páginas web. Aqui estão algumas das principais pseudo-classes:

- **`:focus`** → Aplica estilos quando um elemento recebe foco, como quando um usuário clica em um campo de formulário ou navega com o teclado.
- **`:hover`** → Estiliza um elemento quando o mouse está sobre ele, permitindo que você crie efeitos visuais ao passar o ponteiro.
- **`:active`** → Aplica estilos quando um elemento está em um estado ativo, por exemplo, quando o botão de um link está sendo pressionado.
- **`:visited`** → Aplica estilos a links que já foram visitados, ajudando a indicar ao usuário quais links já foram acessados.
- **`:link`** → Aplica estilos a links que ainda não foram clicados.

```css
a:link {
  color: blue;
}
a:visited {
  color: purple;
}
a:hover {
  color: red;
}
a:active {
  color: green;
}
```

## 3. Pseudo-classes de Formulário

Essas pseudo-classes são usadas para estilizar elementos interativos em formulários.

- **`:checked`** → Seleciona checkboxes e radio buttons marcados.
- **`:disabled`** → Estiliza inputs desativados.
- **`:enabled`** → O oposto de `:disabled`, selecionando inputs ativos.
- **`:required`** → Aplica estilos em campos de formulário que exigem preenchimento.
- **`:optional`** → O oposto de `:required`, para campos opcionais.
- **`:valid` / `:invalid`** → Estilizam campos de entrada com base na validação de formulário.

### 📌 **Dica:**

Use `:focus-within` para estilizar um elemento pai quando um dos seus filhos estiver em foco.
```css
.form-group:focus-within {
  border-color: blue;
}
```

## 4. Pseudo-classes Dinâmicas

Essas pseudo-classes permitem aplicar estilos dependendo do estado atual de um elemento.

- **`:focus-within`** → Estiliza um elemento pai quando um dos seus filhos está em foco.
- **`:not(selector)`** → Seleciona elementos que **não** correspondem ao seletor indicado.
- **`:empty`** → Seleciona elementos que não possuem conteúdo (nem texto, nem filhos).
- **`:target`** → Estiliza o elemento que corresponde ao fragmento de URL. Exemplo: `#section1`.
- **`:root`** → Aplica estilos no elemento raiz do documento, geralmente a tag `<html>`.

### 📌 **Dica:**

Use `:not()` para aplicar estilos a todos os elementos, exceto os que você especificar:
```css
div:not(.special) {
  color: gray;
}
```

## 5. Pseudo-classes de Link e Navegação

Essas pseudo-classes permitem estilizar links e navegação de acordo com o estado do link ou a posição na página.

- **`:link`** → Estiliza links não visitados.
- **`:visited`** → Estiliza links visitados.
- **`:focus`** → Aplica estilos quando um link recebe foco.
- **`:hover`** → Estiliza links quando o usuário passa o mouse sobre eles.
- **`:active`** → Aplica estilos quando um link está sendo clicado.

### 📌 **Dica:**

Uma boa prática é usar as pseudo-classes de link em uma sequência para garantir consistência visual. Exemplo:
```css
a:link {
  color: blue;
}
a:visited {
  color: purple;
}
a:hover {
  color: red;
}
a:active {
  color: green;
}
```

## 6. Pseudo-classes de Estado do Elemento

Essas pseudo-classes permitem estilizar elementos dependendo de sua condição atual.

- **`:checked`** → Aplica estilos a checkboxes ou radio buttons que estão selecionados.
- **`:disabled`** → Seleciona elementos desabilitados.
- **`:enabled`** → Seleciona elementos habilitados.
- **`:required`** → Aplica estilos a campos de formulário obrigatórios.
- **`:optional`** → Aplica estilos a campos de formulário opcionais.

### 📌 **Dica:**

Use `:disabled` para aplicar estilos em elementos de formulário que estão desabilitados:
```css
input:disabled {
  background-color: lightgray;
}
```

# 🔗 **Referências:**  

:pushpin: **Alura - Criando pseudo-elementos com SASS** - [Alura](https://www.alura.com.br/artigos/criando-pseudo-elementos-mais-rapidamente-com-sass) *(Gratuito, Português, Artigo)*  
:pushpin: **Alura - Seletores Avançados** - [Alura](https://www.alura.com.br/artigos/css-seletores-avancados-aplicacoes-web) *(Gratuito, Português, Artigo)*  
:pushpin: **CSS-Tricks: All About CSS Pseudo-classes** - [CSS-Tricks](https://css-tricks.com/almanac/selectors/p/pseudo-class/) *(Gratuito, Inglês, Artigo)*  
:pushpin: **MDN Web Docs: Pseudo-classes** - [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) *(Gratuito, Inglês, Artigo)*  
:pushpin: **MDN Web Docs - Pseudo-classes** - [MDN](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-classes) *(Gratuito, Português, Artigo)*  
:pushpin: **Pseudo Element em WebDev** - [Web.dev](https://web.dev/learn/css/pseudo-elements?hl=pt-br) *(Gratuito, Português, Artigo)*  
:pushpin: **Tutorial em inglês** - [YouTube](https://www.youtube.com/watch?v=GNmz5dYjdcQ) *(Gratuito, Inglês, Vídeo)*  
:pushpin: **W3Schools: CSS Pseudo-classes** - [W3Schools](https://www.w3schools.com/css/css_pseudo_classes.asp) *(Gratuito, Inglês, Artigo)*  
