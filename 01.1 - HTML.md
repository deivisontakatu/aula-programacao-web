# 📘 HTML

## 📌 O que é HTML
HTML (HyperText Markup Language) é a linguagem de marcação usada para estruturar páginas web.  
Ela define textos, imagens, links, tabelas e outros elementos exibidos no navegador.

---

## 🧱 Estrutura Básica

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Minha Página</title>
</head>
<body>
  <h1>Meu primeiro site</h1>
  <p>Bem-vindo ao HTML!</p>
</body>
</html>
```

---

## 🏷️ Tags Principais

```html
<html> <!-- início do documento -->
<head> <!-- configurações -->
<body> <!-- conteúdo visível -->
```

---

## 🧠 Cabeçalhos (Headings)

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Seção</h3>
<h4>Subseção</h4>
<h5>Detalhe</h5>
<h6>Menor título</h6>
```

### Alinhamento
```html
<h1 align="center">Centralizado</h1>
<h2 align="left">Esquerda</h2>
<h3 align="right">Direita</h3>
```

---

## 📝 Parágrafos e Quebras

```html
<p>Este é um parágrafo</p>
<br>
<p align="justify">Texto justificado</p>
```

---

## 🎨 Formatação de Texto

```html
<b>Negrito</b>
<i>Itálico</i>
<sub>Subscrito</sub>
<sup>Sobrescrito</sup>
```

### Tag font (legado)
```html
<font face="Arial" size="3" color="blue">Texto</font>
```

---

## 💬 Comentários

```html
<!-- Comentário em HTML -->
```

---

## 🖼️ Imagens

```html
<img src="imagem.jpg" alt="Descrição">
<img src="img.png" alt="Imagem" width="100">
<img src="img.png" alt="Imagem" height="200">
```

---

## 🎥 Vídeo

```html
<video src="video.mp4" controls></video>
```

---

## 🔊 Áudio

```html
<audio src="audio.mp3" controls></audio>
```

---

## 🔗 Links

```html
<a href="https://google.com">Acessar</a>

<a href="https://google.com">
  <img src="img.jpg" alt="Imagem">
</a>

<a href="https://google.com">
  <h1>Título clicável</h1>
</a>
```

---

## 📋 Listas

### Ordenada
```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

### Não ordenada
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

---

## 📊 Tabelas

```html
<table border="1">
  <tr>
    <td>Linha 1</td>
    <td>Coluna 2</td>
  </tr>
</table>
```

---

## 🧩 Estrutura Semântica (HTML5)

```html
<header></header>
<footer></footer>
<section></section>
<article></article>
<nav></nav>
<aside></aside>
```

---

## 🧱 Div (Container)

```html
<div>
  <h2>Título</h2>
  <p>Conteúdo dentro da div</p>
</div>
```

---

## 🆔 ID e Class

```html
<p id="titulo">Único</p>

<p class="destaque">Texto 1</p>
<p class="destaque">Texto 2</p>
```

---

## 📝 Formulários

```html
<form>
  <label>Nome:</label>
  <input type="text">

  <label>Email:</label>
  <input type="email">

  <textarea></textarea>

  <input type="submit" value="Enviar">
</form>
```

---

## 📦 Conteúdo Extra

```html
<aside>Conteúdo lateral</aside>
```

---

## 🌐 Navegação

```html
<nav>
  <a href="#">Home</a>
  <a href="#">Sobre</a>
</nav>
```

---

## 🧠 Seções e Artigos

```html
<section>
  <article>
    <h2>Post</h2>
    <p>Conteúdo</p>
  </article>
</section>
```

---

## 🎨 Atributos do Body (legado)

```html
<body bgcolor="blue" text="white">
```

---

## ✅ Boas práticas

- Usar indentação
- Utilizar tags semânticas
- Sempre usar `alt` em imagens
- Organizar conteúdo em seções
- Evitar tags antigas (como font)