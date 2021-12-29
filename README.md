# Atividade - Get Coffee Layout

Agora você irá criar uma página HTML replicando o design exibido abaixo: Página inicial do site Get Coffee. Use o que você aprendeu sobre os modelos de caixa e sobre como posicionar elementos usando CSS.

Para resolver essa atividade, faça o clone desse repositório.

Faças as alterações no arquivo css para praticar!


# Mockup:

<!-- ![Mockup - Desktop](https://files-kenzie-academy-brasil.s3.amazonaws.com/q1/sprint3/coffee2.png) -->

[Desktop](https://files-kenzie-academy-brasil.s3.amazonaws.com/q1/sprint3/coffee2.png)

<!-- ![Mockup - Mobile](https://files-kenzie-academy-brasil.s3.amazonaws.com/q1/sprint3/coffee1.png) -->

[Mobile](https://files-kenzie-academy-brasil.s3.amazonaws.com/q1/sprint3/coffee1.png)

---

# Dicas:

## Fontes:

```html
<link href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,200;0,300;0,400;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
```

- font-family: `'Nunito', sans-serif`

---

## Cores/Fontes:

```css

:root{
    --larguraContainerConteudo:1140px;
    --coresTexto: #242424 
    --coresSecundaria: #FCA60F
    --fontSizePrimaria: 18px
    --fontSizeSecundaria: 36px
}

```

## Dicas:

- __Sombra Header__

```css
header{
    box-shadow: 0px 1px 8px rgba(36, 36, 36, 0.15);
}
```

- __Como fazer o Link scroll down__

---

HTML do link:

```html
<a href="#" class="scrollDown">scroll down</a>
```

CSS para fazer o link: 

```css
a{

    font-weight: bold;
    font-size: 18px;
    line-height: 25px;
    text-decoration: none;
    color: #000000;
    display: block;
    text-align: center;
    max-width: 110px;
    margin: 0 auto;
    position: relative;
}
```

```css
a::before{

    width: 4px;
    height: 7px;
    background: #FFFFFF;
    border-radius: 50px;
    margin: 0 auto;
    position: absolute;
    bottom: 3px;
    left: 50%;
    right: 50%;
    transform: translate(-50%, -50%);
}
```

```css
a::after{

    content: "";
    display: block;
    width: 20px;
    height: 35px;
    background: #FCA60F;
    border-radius: 50px;
    margin: 9px auto 0;
}
```
