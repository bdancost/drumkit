# DRUM KIT 🥁

![Status](https://img.shields.io/badge/status-active-brightgreen)

### 🎶 Toque seu próprio tambor virtual!

Este é um projeto de **Kit de Bateria** interativo feito com HTML, CSS e JavaScript. Com ele, você pode tocar sons de bateria ao clicar nas teclas da interface ou pressionar teclas específicas no teclado.

![Drum Kit Screenshot](./img/back.jpg) <!-- Substitua pelo caminho correto para a imagem -->

## 🚀 Demonstração

Você pode acessar a demo do projeto [aqui](drumkit-psi-sooty.vercel.app).

## 📜 Funcionalidades

- Pressione teclas no teclado para tocar sons específicos de bateria.
- Efeitos visuais para simular uma experiência real de tocar em um instrumento.
- Sons de instrumentos de percussão, como _snare_, _kick_, _hihat_ e mais.

## 📂 Estrutura do Projeto

- **index.html**: Estrutura HTML para a interface do kit de bateria.
- **style.css**: Estilos e animações para o layout e os efeitos visuais.
- **index.js**: Funções e lógica para reprodução de sons e animações.
- **img/**: Imagens utilizadas no projeto, incluindo o fundo da interface.
- **sounds/**: Sons de bateria mapeados para cada tecla.

## 🛠️ Tecnologias Utilizadas

- **HTML5** para estrutura de página
- **CSS3** com _Flexbox_ para layout responsivo e efeitos visuais
- **JavaScript** para lógica e controle dos sons e efeitos

## 💻 Como Executar o Projeto

1. Clone este repositório:

   ```bash
   git clone https://github.com/bdancost/drumkit.git
   ```

2. Navegue até o diretório do projeto:

   ```bash
   cd drum-kit
   ```

3. Abra o arquivo `index.html` em um navegador para ver o projeto em ação.

## 🖥️ Interface

As teclas do kit são configuradas para ativar diferentes sons de bateria. Clique ou pressione as teclas **A, S, D, F, G, H, J, K, L** para experimentar.

## 🧩 Estrutura de Código

### HTML

A estrutura básica em HTML inclui uma `div` para o título e uma `div` container onde os botões são criados dinamicamente via JavaScript.

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>DRUM KIT</title>
  </head>
  <body>
    <main>
      <div class="title">DRUM KIT</div>
      <div class="container" id="container"></div>
    </main>
    <script src="./index.js"></script>
  </body>
</html>
```

### CSS

Estilos para criar um layout centralizado com efeitos visuais nas teclas ao serem pressionadas.

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-image: url(./img/back.jpg);
  background-size: cover;
  font-family: "Open Sans", sans-serif;
}
```

### JavaScript

Contém a lógica para mapear teclas, tocar sons e adicionar/remover efeitos.

```javascript
const sons = { A: "boom.wav", S: "clap.wav", D: "hihat.wav" }; // e mais...
const tocarSom = (letra) => {
  /* Código de reprodução de som */
};
```
