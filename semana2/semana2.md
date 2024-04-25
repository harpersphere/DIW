#Dinâmica da Web

## HTML e CSS

### HTML

- Linguagem de marcação baseada em tags no formato de hipertextos.

- Indica quais outros arquivos serão requisitados.

**Estrutura de um documento HTML**

```<!DOCTYPE html>¹
<html>
	<head>²
		<meta name="author" content="Rommel">³
	</head>
	<body>
		<h1> título </h1>
		<p> parágrafo </p>
	</body>
</html>```

##### 1: versão html 2:elementos -> <tag> [conteúdo] </tag> 3: atributos -> nome="valor"

- Indica ID e classes dos elementos.

### CSS

- Define características dos elementos html (cor, tamanho, fonte e etc).

- Utiliza IDs(#) e Classes(.) como referência.

## Dinâmica e carga e processamento

1. Informar endereço.

2. Requesitar, receber e carregar HTML.

3. Requisitar, receber e carregar CSS.

4. Requisitar, receber e carregar JavaScript.

5. Requistar, receber e carregar Imagens e outros arquivos.

# Linguagem HTML

## Sintaxe

### Elementos HTML

Os elementos são a estrutura básica do documento HTML, marcados por meio de tags que são delimitadas pelos símbolos < e >. Veja o exemplo:

```<body> [conteúdo] </body.```

Toda página deve estar contida dentro de um elemento HTML.

```<html> [conteúdo] </html>```

Os nomes dos elementos nas tags **NÃO** são sensíveis ao case (maísculo ou minúsculo é indiferente."

- - -

Elementos HTML podem se apresentar em quatro formatos:

- Elementos com elemento filhos

```<html> <head></head> <body></body> </html>```

- Elementos com texto

```<title> PUC Minas Web Site </title>```

- Elementos vazios

```<meta name="author" content="Rommel"> ou <br>```

- Elementos de conteúdo misto (texto e elementos filhos)

```<p> Documento <span lang="en">Web</span> </p>```

### Atributos

- Os atributos podem ser incluídos em elementos HTML.

- Um atributo não se repete em um elemento.

- São definidos pelo par nome/valor

```<input disabled name="Nome_Usuario" value="rommelcarneiro">```

- Recomenda-se utilizar aspas duplas

- Os atributos alteram o funcionamento dos elementos do HTML.

- Cada elemento possui um conjunto próprio de atributos.

- Os atributos possuem valores livres ou pré-definidos.

### Comentários

- Os comentários não são exibidos pelo navegador

- São delimitados por <!-- e -->

```<!-- os comentarios documentam o codigo HTML -->```

### Doctype

O **DOCTYPE** indica ao browser qual versão do HTML está sendo utilizada no documento, alternando entre *quirks mode* e *strict mode*.

HTML5 	      	->      ```<!DOCTYPE html>```
     
HTML 4.01	- >	```<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">```

Para todos tipos de declaração, consulte [w3.org](https://www.w3.org/QA/2002/04/valid-dtd-list.html)

### Cabeçalho

Primeira parte do arquivo HTML, representada pela tag <head>, que inclui informações sobre o documento (metadados), referências a scripts, folhas de estilo (CSS) que complementam o documento.

```<!DOCTYPE html>
<html lang="pt-br">
      <head> ... </head>
      <body>
	<h1> título </h1>
	<p> parágrafo </p>
      </body>
</html>```

### Tipos de Elementos

- Metadados

  - Trazem informações sobre a página

- Textuais

  - Conteúdo de texto das páginas

- Multimídia

  - Imagens, áudio e vídeo

- Tabelas

  - Estruturar dados em tabelas

- Estrutura

  - Sepaaração e organização do conteúdo

- Formulários

  - Elementos para entrada de dados pelo usuário

- Scripting

  - Conteúdo dinâmico de aplicações Web

- Integração

  - Conteúdo externo ou multimídia avançada

### Tipos de Elementos quanto ao fluxo da página

- Elementos inline

  - Elementos inline são dispostos em linha seguindo o fluxo padrão

Exemplo: ```<img>, <span>, <a>, <button>, <input>, <label>```

- Elementos block

  - São elementos que iniciam uma nova linha não se dispondo a frente daquilo que o precede.

Exemplo: ```<div>, <h1> ... <h6>, <p>, <form>, <canvas>, <table>, <section>```

### Metadados

Os elementos metadados trazem informações sobre a página

- **title**: Define o título da documentação

- **style**: Define códigos de formatação  no padrão CSS

- **link**: Definem ligações com outros arquivos como: CSS, scripts e etc

- **meta**: As meta tags trazem informações sobre o documento tais como codificação de caracteres, descrição, palavras-chave, autor, etc.

```<head>
	<title>Página de Exemplo</title>
	<meta name="desciption" content="Puc Minas Web site">
	<meta name="author" content="Rommel">
	<meta name="keywords" content="html, web, css">
	<link rel="stylesheet" href="style.css">
</head>```

### Open Graph Protocol

O Open Graph Protocol é um protocolo de metadados, que permite com que redes sociais e embeds identifiquem o conteúdo do site.

```<html prefix="pg: https://ogp.me/ns#">
<head>
<title>The Rock (1996)</title>
<meta property="og:title" content="The Rock" />
<meta property="og:type" content="video.movie" />
<meta property="og:url content="https://www.imdb.com/title/tt0117500" />
<meta property="og:image" content="https://ia.media-imdb.com/images/rock.jpg" />
...
</head>
...
</html>```

### Elementos de Layout

<header>, <nav>, <main>, <article> e <footer>

