# 🎨 CSS – Fundamentos e Layouts Modernos

O **CSS (Cascading Style Sheets)** é a tecnologia usada para definir a **aparência e o layout** das páginas da web.  
Enquanto o **HTML** fornece a **estrutura**, o **CSS** controla **cores, tipografia, espaçamento e responsividade**.

---

## 🏁 Conceitos Básicos

### Formas de Aplicação
- **Externo (preferido):** arquivo `.css` vinculado via `<link>` no `<head>`.
- **Interno:** bloco `<style>` no `<head>`.
- **Inline:** atributo `style` diretamente no elemento (evite em projetos grandes).

### Estrutura
```css
seletor {
  propriedade: valor;
}
```

Exemplo:
```css
body {
  font-family: Arial, sans-serif;
  background-color: #f5f5f5;
}
```

### Seletores
- **Por elemento:** `p`, `h1`, `div`
- **Classe:** `.botao`
- **ID:** `#menu`
- **Combinadores:** `div p`, `ul > li`
- **Pseudo-classes:** `a:hover`, `input:focus`
- **Pseudo-elementos:** `::before`, `::after`

---

## 🎨 Cores e Tipografia
- Cores em **hexadecimal** (`#ff0000`), **RGB** (`rgb(255,0,0)`), **HSL** (`hsl(0, 100%, 50%)`).
- Fontes: `font-family`, `font-size`, `line-height`, `font-weight`.
- Importar fontes externas (ex.: Google Fonts):
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
```

---

## 🧩 Box Model

Cada elemento em uma página é representado como uma **caixa**, composta por:

1. **Content:** conteúdo (texto, imagem).
2. **Padding:** espaço interno entre o conteúdo e a borda.
3. **Border:** linha ao redor do padding.
4. **Margin:** espaço externo entre elementos.

```css
.elemento {
  width: 200px;
  padding: 20px;
  border: 2px solid black;
  margin: 10px;
  box-sizing: border-box; /* inclui padding e borda no width/height total */
}
```

💡 **Dica:** Use `box-sizing: border-box` para facilitar o controle de tamanhos.

---

## 📍 Position

Controla o posicionamento dos elementos na página:

- **static:** padrão, segue o fluxo normal.
- **relative:** deslocado em relação à posição original.
- **absolute:** posicionado em relação ao elemento pai posicionado.
- **fixed:** fixo em relação à janela do navegador.
- **sticky:** combina comportamento de `relative` e `fixed`.

```css
.menu-fixo {
  position: fixed;
  top: 0;
  width: 100%;
}
```

---

## 🧱 Flexbox

O **Flexbox** facilita a criação de **layouts unidimensionais** (em linha ou coluna) com alinhamento flexível.

```css
.container {
  display: flex;
  justify-content: space-between; /* alinha horizontalmente */
  align-items: center;            /* alinha verticalmente */
}
```

Propriedades importantes:
- `flex-direction`: `row` | `column`
- `justify-content`: `flex-start`, `center`, `space-between`, `space-around`
- `align-items`: `flex-start`, `center`, `flex-end`
- `flex-wrap`: permite quebra de linha
- `gap`: define espaçamento entre itens

```css
.item {
  flex: 1; /* cresce para ocupar espaço disponível */
}
```

---

## 📱 Layouts Responsivos

### Meta viewport (em HTML)
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Media Queries
Permitem definir estilos diferentes para tamanhos de tela distintos:
```css
@media (max-width: 768px) {
  body {
    font-size: 14px;
    padding: 10px;
  }
}
```

💡 **Boas práticas:**
- Utilize unidades relativas: `%`, `em`, `rem`, `vw`, `vh`.
- Combine **Flexbox** ou **CSS Grid** para criar **layouts fluidos**.

---

## 🧮 CSS Grid (opcional para layouts mais complexos)

Embora o foco aqui seja Flexbox, vale conhecer o **CSS Grid**, ideal para layouts bidimensionais.

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 20px;
}
```

---

## ⚡ Performance e Organização
- Prefira arquivos CSS externos para cache e manutenção.
- Minifique o CSS em produção.
- Estruture o código em módulos ou use metodologias como **BEM** para organização.

---

## 📚 Referências

- [MDN Web Docs – CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
- [Guia Flexbox – CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Guia Grid – CSS Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [W3C CSS Specification](https://www.w3.org/Style/CSS/)

---

💡 **Resumo:**  
O CSS é a base da **estilização e do design responsivo** na web. Dominar o **Box Model**, **Position** e **Flexbox**, além de aplicar **media queries**, é essencial para criar interfaces modernas, adaptáveis e de alta performance.
