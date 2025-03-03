# Bibliotech - Estante Virtual de Livros 📚

O **Bibliotech** é um projeto de estante virtual de livros desenvolvido como parte de um trabalho escolar.

## Demonstração

Para visualizar o projeto, clique [aqui](https://kaitotsubaki.github.io/bibliotech/).

## Recursos e Funcionalidades Implementadas

### estante virtual

1. **Livros em 3D com Rotação Interativa**
   - Os livros são representados em um ambiente 3D simulado com CSS.
   - Cada livro possui uma rotação interativa quando o usuário passa o mouse sobre ele.

   Exemplo de código relevante:

   ```css
   .book {
     position: relative;
     display: block;
     width: 220px;
     height: 350px;
     margin: 5% auto;
     border-radius: 2px 4px 4px 2px;
     background: linear-gradient(45deg, #dad5dc 0%, #f2ebf4 100%);
     box-shadow: 13px 13px 8px 0px rgba(22, 22, 22, 0.6);
     transform-style: preserve-3d;
     transition: transform 0.5s;
   }

   .book:hover {
     transform: rotateY(0deg);
   }
   ```

2. **Efeitos de Sombra e Iluminação**
   - Os livros têm efeitos de sombra e iluminação para simular profundidade e realismo.

   Exemplo de código relevante:

   ```css
   .book {
     box-shadow: 13px 13px 8px 0px rgba(22, 22, 22, 0.6);
     background: linear-gradient(45deg, #dad5dc 0%, #f2ebf4 100%);
   }
   ```

3. **Links para PDFs Integrados**
   - Cada livro na estante é um link para um arquivo PDF correspondente, permitindo que o usuário visualize as reviews dos livros.

   Exemplo de código relevante:

   ```html
   <a href="pdfs/fyodor.pdf">
     <img src="imagens/fyodor.jpg" alt="Livro de Fyodor Dostoyevsky" />
   </a>
   ```

   ### site principal

4. **Animação de Elementos com Scroll**
   - Utilizei a biblioteca ScrollReveal.js para criar animações dinâmicas à medida que o usuário rola a página.

   Exemplo de código relevante:

   ```javascript
   ScrollReveal().reveal("#bookshelf .shelf-row", { delay: 300 });
   ```



---
