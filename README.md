# marvin

https://marcoscruz98-bot.github.io/marvin/

## 1. Construção de textos e parágrafos com HTML

<br>

### A) criação de parágrafos ou frases

#### Exemplo:


```html
<p id ="p1" onclick ="mudar_cor()">Aqui vai qualquer texto ou frase que queira</p>
```

<br>

### B) Adicionando CSS aos parágrafos

#### Exemplo adicionando cores:

```css
#p1{

	color: blue;
}
```

<br>

### C) Adicionando JavaScript aos parágrafos

#### Exemplo mudando cores:

```js
function mudar_cor(){

	document.getElementById("p1").style.color = "brown";
}
```

#### Observe que o mesmo p1 está sendo repetido no HTML, CSS e JavaScript!!!

<br>

## 2. Construção de títulos e subtítulos

<br>

### A) Toda página possui um único tema. Para isso, use h1.

#### Exemplo:

```html
<h1 id ="h1" onclick ="mudar_h1()">Tema da minha página</h1>
```

<br>

### B) Adicionando CSS ao tema

#### Exemplo adicionando um tipo de capitalização:

```css
#h1{

	text-transform: lowercase;
}
```

<br>

### C) Adicionando JavaScript ao tema

#### Exemplo mudando a capitalização padrão do CSS:

```js
function mudar_h1(){

	document.getElementById("h1").style.textTransform = "uppercase";
}
```

<br>

### D) Toda página pode ter subtítulos para cada pedaço de conteúdo, assim como um mercado possui um nome para cada corredor. Para isso, use h2.

```html
<h2 id ="h2" onclick ="mudar_h2()">Subtítulo da seção frutas</h2>

<h2 id ="h_2" onmouseenter="mudar_h_2()">Subtítulo da seção de frios</h2>
```

<br>

### E) Adicionando CSS aos subtítulos

#### Exemplos adicionando cor de fundo e alterando alinhamento:

```css
#h2{

	background-color: cyan;
}

#h_2{

	text-align: right;
}
```

<br>

### F) Adicionando JavaScript ao subtítulos

#### Exemplo mudandando a cor de fundo e o alinhamento padrão do CSS.

```js
function mudar_h2(){

	document.getElementById("h2").style.backgroundColor = "yellow";
}

function mudar_h_2(){

	document.getElementById("h_2").style.textAlign = "left";
}
```

<br>


## 3. Construção listas ordenadas e desordenadas

<br>

### A) Listas Ordenadas: agrupar itens que possuem uma relação de ordem crescente ou decrescente entre si.

### Exemplo:

```html
<h1>Seleções nacionais mais vencedoras da Copa do Mundo FIFA:</h1>

<ol id ="ol1" onclick ="mudar_ol1()">
	<li>Brasil - 5</li>
	<li>Alemanha - 4</li>
	<li>Itália - 4</li>
	<li>Argentina - 3</li>
	<li>Uruguai - 2</li>
	<li>França - 2</li>
	<li>Espanha - 2</li>
	<li>Inglaterra - 1</li>
</ol>
```

<br>

### B) Customizando com o CSS

<br>

#### Exemplo alterando o tipo de ordenamento e sua cor:

```css
#ol1{

	list-style-type: lower alpha;
}

#ol1 > li::marker{

	color: red;
}
```

<br>

### C) Adicionando interação com o JS.

#### Exemplo modificando o tipo de ordenamento:

```js
function mudar_ol1(){

	document.getElementById("ol1").style.listStyleType = "decimal";
}
```

<br>

### D) Listas Não Ordenadas: agrupar itens que não possuem uma relação de ordem crescente ou decrescente entre si.

### Exemplo:

```html
<h1>Os assuntos mais comuns em Estatística</h1>

<ul id ="ul1" onclick ="mudar_ul1()">
	<li>Média</li>
	<li>Moda</li>
	<li>Mediana</li>
	<li>Variância</li>
	<li>Amostragem</li>
	<li>Desvio Padrão</li>
	<li>Intervalo de confiança</li>
</ul>
```

<br>

### E) Customizando com o CSS

#### Exemplo alterando o símbolo de destaque ao lado do nome e sua cor:

```css
#ul1{

	list-style-type: square;
}

#ul1 > li::marker{

	color: coral;
}
```

<br>

### F) Adicionando interação com o JS.

#### Exemplo modificando o símbolo de destaque:

```js
function mudar_ul1(){

	document.getElementById("ul1").style.listStyleType = "circle";
}
```

<br>

## 4. Imagens

<br>

### A) Imagens por padrão em um site:

#### Exemplo:

```html
<figure>

	<img id ="gif0" onmouseenter ="mudar_gif0()" src="./imagens/html-css-js.gif" alt="GIF com a diferença entre HTML, CSS e Javascript" width="480" height="480">
	
</figure>
```

<br>

<br>

### B) Customizando com o CSS

#### Exemplo adicionando arredondamento da borda, opacidade, borrão, brilho e sombreado de uma imagem:

```css
#gif0{

	border-radius: 30px;
	opacity: 0.8;
	filter: blur(2px) brightness(150%) drop-shadow(10px 10px 1px red);
}
```

<br>

### C) Adicionando interação com o JS.

#### Exemplo modificando a imagem:

```js
function mudar_gif0(){

	document.getElementById("gif0").style.borderRadius = "15px";
	document.getElementById("gif0").style.opactiy = "0.7";
	document.getElementById("gif0").style.filter = "blur(3px)";
	document.getElementById("gif0").style.filter = "brightness(70%)";
	document.getElementById("gif0").style.filter = "drop-shadow(6px 7px 2px coral)";
}
```

<br>

## 5. Vídeos

<br>

### A) Vídeos por padrão em um site

#### Exemplo:

```html
<video id="video_0" width ="640" height="360" controls>
	
	<source src="./videos/movie1.mp4" type="video/mp4">

</video>
```

<br>

### B) Vídeos vindo do Youtube com iframe

#### Exemplo:

```html
<iframe width="640" height="360" src="https://www.youtube.com/embed/LXb3EKWsInQ" title="COSTA RICA IN 4K 60fps HDR (ULTRA HD)" allowfullscreen></iframe>
```

<br>

### C) Customizando com o CSS

#### Exemplo adicionando arredondamento da borda e sombreado no vídeo:

<br>

```css
#video_0{

	border-radius: 10px;
	filter: drop-shadow(2px 2px 5px gray);
}
```

<br>

## 6. Hiperlinks

<br>

### A) Hiperlinks para outros sites

#### Exemplo abrindo o link em outra aba do navegador:

```html
<nav>

	<a id="link_0" href ="https://www.google.com" target ="_blank">Google</a>

</nav>
```

#### Exemplo abrindo o link na mesma aba do navegador:

```html
<nav>

	<a id="link_1" href ="https://www.youtube.com">Youtube</a>

</nav>
```

<br>

### C) Customizando com o CSS

#### Exemplo com os 4 estados de um link:

<br>

```css
/* a aparência padrão do link */
#link_0:link {
	
	color: magenta;
	transition: font-size 2s;
}

/* segundos após o link ser clicado a aparência do link é alterada*/
#link_0:visited {
	
	color: none;
}

/* altera a aparência quando o mouse passa por cima (hover) do link */
#link_0:hover {
	
	color: hotpink;
	font-size: 2em;
	transition: font-size 2s;
}

/* altera a cor no exato momento que o link é clicado com o mouse */
#link_0:active {
	
	color: none;
}
```
