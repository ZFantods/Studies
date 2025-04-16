# 🎨 Variáveis no HTML e CSS – Tudo o Que Você Precisa Saber!  

As variáveis são um conceito essencial na programação, e no **CSS** não é diferente! Elas permitem reutilizar valores, facilitar a manutenção do código e melhorar a organização do projeto.  

## 🎯 O Que São Variáveis no CSS?  

No CSS, as variáveis são chamadas de **Custom Properties**. Elas permitem armazenar valores reutilizáveis, como **cores, tamanhos e espaçamentos**.  

### 📌 Sintaxe Básica  

```css
:root {
  --cor-primaria: #3498db;
  --cor-secundaria: #2ecc71;
  --tamanho-fonte: 16px;
}

body {
  background-color: var(--cor-primaria);
  color: white;
  font-size: var(--tamanho-fonte);
}
```

✅ **Explicação:**  
- `:root` define as variáveis globais, acessíveis em todo o código.  
- `--cor-primaria` é uma variável personalizada.  
- `var(--cor-primaria)` acessa o valor da variável.  

---

## 📌 Onde Declarar as Variáveis?  

### 🔹 **No `:root` (Recomendado)**
Usar `:root` permite que as variáveis sejam aplicadas globalmente.  

```css
:root {
  --fonte-principal: Arial, sans-serif;
}
```

### 🔹 **Em um Elemento Específico**
As variáveis podem ser declaradas dentro de elementos, tornando-as **locais**.  

```css
.card {
  --cor-fundo: #f4f4f4;
  background-color: var(--cor-fundo);
}
```

### 🔹 **Dentro de Media Queries**
Podemos alterar variáveis com **Media Queries**, tornando o site mais dinâmico.  

```css
:root {
  --tamanho-fonte: 16px;
}

@media screen and (max-width: 768px) {
  :root {
    --tamanho-fonte: 14px;
  }
}

p {
  font-size: var(--tamanho-fonte);
}
```

✅ **Dica:** Isso permite que a fonte se ajuste automaticamente conforme o tamanho da tela!  

---

## 🚀 Benefícios do Uso de Variáveis  

✅ **Facilitam a manutenção:** Se precisar trocar uma cor, basta mudar a variável no `:root`.  
✅ **Reduzem a repetição:** Menos código duplicado significa menos erros!  
✅ **Melhoram a organização:** O código fica mais legível e modular.  
✅ **Tornam o design mais dinâmico:** Combinadas com `@media`, criam **layouts flexíveis**.  

---

## 📏 Diferença Entre `var()` e `calc()`  

O `var()` é usado para **recuperar** valores de variáveis, enquanto o `calc()` permite realizar **cálculos dinâmicos** no CSS.  

```css
:root {
  --largura-base: 50px;
}

.box {
  width: calc(var(--largura-base) * 2);
}
```

✅ **Dica:** Você pode combinar `var()` com `calc()` para criar estilos dinâmicos!  

---

## 🔥 Usando JavaScript para Manipular Variáveis CSS  

Podemos modificar variáveis CSS dinamicamente usando **JavaScript**!  

### 📝 Exemplo  

```html
<input type="color" id="seletor-cor">
<p>Texto colorido dinamicamente!</p>

<script>
  const seletor = document.getElementById('seletor-cor');
  seletor.addEventListener('input', (evento) => {
    document.documentElement.style.setProperty('--cor-dinamica', evento.target.value);
  });
</script>

<style>
  :root {
    --cor-dinamica: #ff0000;
  }

  p {
    color: var(--cor-dinamica);
    font-size: 20px;
  }
</style>
```

🔹 **O que acontece aqui?**  
- O usuário escolhe uma cor no input.  
- O JavaScript altera a variável `--cor-dinamica`.  
- O CSS aplica a nova cor no texto **em tempo real**!  

---

## 🧐 Diferença Entre Variáveis CSS e Variáveis SASS  

Além das variáveis do CSS puro, o **SASS/SCSS** também oferece variáveis, mas com diferenças importantes:  

| Característica         | Variáveis CSS            | Variáveis SASS         |
|------------------------|-------------------------|------------------------|
| Definição              | `--minha-var: valor;`   | `$minha-var: valor;`  |
| Escopo                 | Podem ser globais ou locais | Sempre locais ao arquivo |
| Atualização dinâmica  | ✅ Sim, pode ser alterada no JS | ❌ Não, são compiladas no build |
| Suporte nativo        | ✅ Sim, compatível com navegadores | ❌ Não, precisa de pré-processador |

✅ **Dica:** Se precisa de algo dinâmico, prefira **variáveis CSS**. Se quer **organização pré-processada**, use **SASS**.  

---

## 🎯 Conclusão  

As variáveis CSS são uma **ferramenta poderosa** para criar projetos mais organizados e flexíveis. Com elas, podemos:  
✔️ **Reutilizar valores** sem repetir código.  
✔️ **Criar temas dinâmicos** facilmente.  
✔️ **Melhorar a manutenção e escalabilidade** do CSS.  
✔️ **Integrar com JavaScript** para efeitos avançados.  

💡 **Bônus:** Quer aprender mais? Confira a documentação oficial do CSS:  
🔗 [MDN Web Docs - Variáveis CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)  

