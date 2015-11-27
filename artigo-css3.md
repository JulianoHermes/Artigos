#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Juliano Gustavo Hermes
#### E-mail: {j.hermes09@gmail.com}
### Artigo de revisão de CSS3
##### Funcionalidade: Animations
##### O que é?
São mudanças de estado de um objeto na página, essas mudanças podem ser de cor, tamanho, posição. As transições podem ocorrer tantas vezes quanto for especificado. O principal foco da animação é realizar a mesma em um período de tempo, assim executando a tranisação como um animação e não como um degrau de mudança.
##### Onde usar:
Em qualquer elemento.
##### Como usar:
Antes da utilização do atributo animation é necessária a declaração do Keyframe que define a animação a ser executada.
```css
@keyframes animationname {keyframes-selector {css-styles;}}

animation: name duration timing-function delay iteration-count direction fill-mode play-state;
```
##### Exemplo de uso
um exemplo de sintaxe atuando sobre uma div, executando a troca de valor do atributo background-color.

```css
/* Chrome, Safari, Opera */
div {
    width: 100px;
    height: 100px;
    background-color: red;
    -webkit-animation:example 1s linear infinite;
	animation:example 1s linear infinite;
}

/* Chrome, Safari, Opera */
@-webkit-keyframes example {
    0%   {background-color: red;}
    50%  {background-color: yellow;}
    100% {background-color: red;}
}

/* Standard syntax */
@keyframes example {
    0%   {background-color: red;}
    50%  {background-color: yellow;}
    100% {background-color: red;}
}
```
### Referencia:
####
[w3schools.com Animation](http://www.w3schools.com/cssref/css3_pr_animation.asp),
[w3schools.com Keyframe](http://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp),
[w3schools.com CSS3 Animations](http://www.w3schools.com/css/css3_animations.asp)

##### Funcionalidade: calc()
##### O que é?
é uma função que executa um determinado calculo matemático para determinar o valor de uma propriedade.
##### Onde usar:
Em qualquer propriedade onde um número é requisitado.
##### Como usar:
```css
calc(expression)
```
##### Exemplo de uso
um exemplo de sintaxe atuando sobre uma div, definindo o width atravez da expressão.

```css
div {
    /* property: calc(expression) */
	width: calc(100% / 2);
}
```
### Referencia:
[developer.mozilla.org Calc](https://developer.mozilla.org/en-US/docs/Web/CSS/calc)

##### Funcionalidade: @font-face
##### O que é?
permite adicionar uma fonte estilizada, para ser utilizada na página assim permitindo a utilização de fontes fora do "web-safe".
##### Onde usar:
Em qualquer elemento que utilize escrita.
##### Como usar:
```css
@font-face {
	descritivo: valor;
	descritivo: valor;
	...
}
```
##### Exemplo de uso

```css
@font-face {
	font-family: "RegencyScriptFLF Regular";
	src: url("http://site/fontes/RegencyScriptFLF-Regular.ttf");
	}

p { font-family: "RegencyScriptFLF Regular", Cursive; }
```
### Referencia:
[w3schools.com @Font-Face](http://www.w3schools.com/css/css3_fonts.asp), 
[maujor.com @Font-Face](http://www.maujor.com/tutorial/css3-@font-face.php)

##### Funcionalidade: @media
##### O que é?
é uma delimitação a respeito do tipo de media utilizada, habilitando alterações na visualização de acordo com os delimitadores utilizados.
##### Onde usar:
na definição de visualização especificas para determinadas midias e resoluções.
##### Como usar:
```css
@media not|only mediatype and (expressions) {
    CSS-Code;
}
```

##### Exemplo de uso

```css
@media screen and (max-width: 480px) {
    div{
        width:100px;
    }
}
```
### Referencia:
[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries), 
[w3schools.com](http://www.w3schools.com/css/css3_mediaqueries.asp)

##### Funcionalidade: multiplos backgrounds
##### O que é?
A partir do CSS3 novas propriedades foram adicionadas permitindo multiplas imagens de fundo, entre outras.
##### Onde usar:
em qualquer elemento que possua background.
##### Como usar:
```css
seletor {
  background: background1, background 2, ..., backgroundN;
}
```

##### Exemplo de uso

```css
div {
    background-image: url(img01.gif), url(img02.gif);
    background-position: right bottom, left top;
    background-repeat: no-repeat, repeat;
}
```
### Referencia:
[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Background_and_Borders/Using_CSS_multiple_backgrounds), 
[w3schools.com](http://www.w3schools.com/css/css3_backgrounds.asp)

##### Funcionalidade: text-shadow
##### O que é?
é a aplicação de uma sombra sobre o texto existente no seletor.
##### Onde usar:
em um seletor que possua um texto.
##### Como usar:
```css
seletor { 
	text-shadow: offsetX offsetY raioBlur cor [,offsetX offsetY raioBlur cor]*; 
} 
```

##### Exemplo de uso

```css
div { 
	text-shadow: 10px -10px 10px black; 
} 
```
### Referencia:
[maujor.com](http://www.maujor.com/tutorial/interativo-css3/inc/textshadow.php)

##### Funcionalidade: box-shadow
##### O que é?
é a aplicação de uma sombra sobre o corpo do seletor.
##### Onde usar:
em um seletor qualquer.
##### Como usar:
```css
seletor { 
	box-shadow: inset offsetX offsetY raioBlur spread cor;
} 
```

##### Exemplo de uso

```css
div {
    box-shadow: 10px 10px grey;
}
```
### Referencia:
[maujor.com](http://www.maujor.com/tutorial/interativo-css3/inc/boxshadow.php),
[w3schools.com](http://www.w3schools.com/css/css3_shadows.asp)

##### Funcionalidade: border-image
##### O que é?
consiste na utilização de uma imagem padrão para ser utilizada como borda do seletor especificado, definindo, além da imagem, o ponto de corte e o modo de prenchimento da borda. 
##### Onde usar:
em um seletor qualquer.
##### Como usar:
```css
seletor{
	border-image: source slice width outset repeat|initial|inherit;
}
```

##### Exemplo de uso

```css
div {
    border-image: url(image1.png) 5 round;
}
```
### Referencia:
[css-tricks.com](https://css-tricks.com/understanding-border-image/),
[w3schools.com](http://www.w3schools.com/css/css3_border_images.asp)

##### Funcionalidade: Counter
##### O que é?
Cria um contador para contabilizar quantas vezes a regra do css foi executada, pondendo retornar esse valor para o elemento.
##### Onde usar:
em um seletor qualquer.
##### Como usar:
função de incremento
```css
seletor{
	counter-increment: none|id|initial|inherit;
}
```
função de reset do contador
```css
seletor{
	counter-reset: none|name number|initial|inherit;
}
```

##### Exemplo de uso

```css
ol {
  counter-reset: section;
  list-style-type: none;
}
li::before {
  counter-increment: section;
  content: counters(section,".") " "; 
}
```
### Referencia:
[developer.mozilla.org](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Lists_and_Counters/Using_CSS_counters),
[w3schools.com counter-reset](http://www.w3schools.com/cssref/pr_gen_counter-reset.asp),
[w3schools.com counter-increment](http://www.w3schools.com/cssref/pr_gen_counter-increment.asp)

##### Funcionalidade: rotate
##### O que é?
executa uma rotação no objeto de acordo com o angulo definido e a função, podendo executar rotações nos eixos x, y e z. A função rotate se executa por meio do propriedade transform.
##### Onde usar:
em um seletor qualquer.
##### Como usar:
```css
seletor{
	transform: rotate(angle); /* Rotação 2D */
	transform: rotate3d(x,y,z,angle); /* Rotação 3D */
	transform: rotateX(angle); /* Rotação 3D pelo eixo X*/
	transform: rotateY(angle); /* Rotação 3D pelo eixo Y*/
	transform: rotateZ(angle); /* Rotação 3D pelo eixo Z*/
}
```

##### Exemplo de uso
exeplo utilizando rotateX
```css
div {
    transform: rotateX(45deg);
}
```
### Referencia:
[w3schools.com Propriedades transform](http://www.w3schools.com/cssref/css3_pr_transform.asp),
[w3schools.com 3d transform](http://www.w3schools.com/css/css3_3dtransforms.asp)

##### Funcionalidade: perspective
##### O que é?
utilizado em conjunto com as transformações 3d. Quando aplicadas essas transformações no child do seletor posibilita que a aplicação do 3d gere uma perspectiva do seletor child em relação ao seletor.
##### Onde usar:
em um seletor que possua um child com um efeito transform por exemplo rotate.
##### Como usar:
```css
seletor{
	perspective: length|none;
}
```

##### Exemplo de uso
exeplo utilizando rotateX com perspective
```css
.container{
	perspective: 150px;
}
.container>div {
    transform: rotateX(45deg);
}
```
### Referencia:
[w3schools.com](http://www.w3schools.com/cssref/css3_pr_perspective.asp)

##### Funcionalidade: gradient
##### O que é?
executa uma definição de gradiente podendo ser radial ou linear, definido com n cores.
##### Onde usar:
utilizado na propriedade background do seletor.
##### Como usar:
```css
seletor{
	background: radial-gradient(shape size at position, start-color, ..., last-color);
}
seletor{
	background: linear-gradient(direction, color-stop1, color-stop2, ...);
}
```

##### Exemplo de uso
exeplo utilizando rotateX com perspective
```css
div{
	background: repeating-linear-gradient(to right, black 10%, gray 30%, black 50%);
}
```
### Referencia:
[w3schools.com](http://www.w3schools.com/css/css3_gradients.asp)

##### Funcionalidade: columns
##### O que é?
realiza a quebra do texto contido em um determinado seletor, podendo especificar tamanho das colunas, divisor, quantidade de colunas, espaço entre colunas entre outras especificidades.
##### Onde usar:
em um seletor que possua texto.
##### Como usar:
existem varias propriedades separadas para cada elemento da coluna sendo esses
column-count
```css
seletor{
	-webkit-column-count: number;
}
```
column-gap
```css
seletor{
	-webkit-column-count: lenght;
}
```
column-rule
```css
seletor{
	-webkit-column-rule: width style color;
}
```
column-span
```css
seletor{
	-webkit-column-span: 1|all|initial|inherit;
}
```
column-width
```css
seletor{
	-webkit-column-width: width;
}
```

##### Exemplo de uso
```css
div {
    -webkit-column-count: 3;
    -webkit-column-gap: 90px;
    -webkit-column-rule: 1px dashed gray;
}
```
### Referencia:
[w3schools.com](http://www.w3schools.com/css/css3_multiple_columns.asp)