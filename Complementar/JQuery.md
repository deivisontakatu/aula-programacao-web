# 📘 Introdução ao jQuery

## O que é jQuery?

👉 **jQuery é uma biblioteca de JavaScript.**  
Ela foi criada para simplificar o uso do JavaScript, permitindo que o desenvolvedor escreva menos código para fazer as mesmas coisas.  

### O que o jQuery facilita?
- **Manipular o DOM** (mudar textos, cores, atributos, imagens).  
- **Trabalhar com eventos** (cliques, teclado, mouse).  
- **Criar animações** (esconder/mostrar, fades, slides).  
- **Compatibilidade entre navegadores** (funciona de forma padronizada).  

---

## Comparação: JavaScript puro vs. jQuery

**JavaScript puro:**
```javascript
document.getElementById("botao").addEventListener("click", function() {
  document.getElementById("texto").style.display = "none";
});
```

**jQuery:**
```javascript
$("#botao").click(function(){
  $("#texto").hide();
});
```

➡️ Com jQuery o código fica mais curto e mais fácil de entender.

---

## Como usar o jQuery

Basta importar a biblioteca no seu HTML, geralmente usando um **CDN**:

```html
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
```

Depois, você pode escrever código jQuery dentro de:

```javascript
$(document).ready(function(){
  // Seu código aqui
});
```

---

## Exemplo 1: Mostrar / Esconder Texto

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Exemplo jQuery - Mostrar/Esconder Texto</title>
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <style>
    #caixa {
      width: 300px;
      margin: 20px auto;
      padding: 20px;
      border: 2px solid #333;
      background: #f0f0f0;
      display: none; /* começa escondido */
    }
  </style>
</head>
<body>
  <h1>Exemplo com jQuery</h1>
  <button id="botao">Mostrar / Esconder Caixa</button>
  <div id="caixa">
    <p>Este é um texto que aparece e desaparece com efeito!</p>
  </div>

  <script>
    $(document).ready(function(){
      $("#botao").click(function(){
        $("#caixa").slideToggle("slow"); 
      });
    });
  </script>
</body>
</html>
```

✅ Ao clicar no botão, a caixa aparece e desaparece com efeito de **slide**.

---

## Exemplo 2: To-Do List Simples

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>To-Do List com jQuery</title>
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <style>
    body { font-family: Arial, sans-serif; text-align: center; }
    ul { list-style: none; padding: 0; }
    li { padding: 8px; background: #f0f0f0; margin: 5px; cursor: pointer; }
    li.done { text-decoration: line-through; color: gray; }
  </style>
</head>
<body>
  <h1>Minha To-Do List</h1>
  <input type="text" id="tarefa" placeholder="Digite uma tarefa">
  <button id="adicionar">Adicionar</button>

  <ul id="lista"></ul>

  <script>
    $(document).ready(function(){
      // Adicionar tarefa
      $("#adicionar").click(function(){
        let texto = $("#tarefa").val();
        if(texto !== ""){
          $("#lista").append("<li>" + texto + "</li>");
          $("#tarefa").val(""); // limpa input
        }
      });

      // Marcar como concluída ao clicar
      $(document).on("click", "li", function(){
        $(this).toggleClass("done");
      });
    });
  </script>
</body>
</html>
```

✅ Neste exemplo:
- O usuário adiciona tarefas.  
- Pode clicar em cada tarefa para marcar como concluída.  

---

## Resumo

- **jQuery = JavaScript mais simples.**  
- Permite manipular **elementos, eventos e efeitos** com poucas linhas.  
- É muito útil para quem está começando e quer ver resultados rápidos.  

---
