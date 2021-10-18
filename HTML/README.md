# [HTML](../README.md/#my-library)

## [Índice](../README.md/#lista-de-cursos)

1. [Começando](#começando)
    1. [Introdução](#introdução)
        1. [Tags](#tags)
        2. [Estrutura](#estrutura)
        3. [Comentários](#comentários)
    2. [Elementos](#elementos)
        1. [Tags ou Elementos?](#tags-ou-elementos)    
        2. [Elementos Vazios](#elementos-vazios)
        3. [Elementos Aninhados](#elementos-aninhados)
2. [Formatação](#formatação)
    1. [Semântica](#semântica)
        1. [header](#header)
        2. [article](#article)
        3. [aside](#aside)
        4. [footer](#footer)
        5. [section](#section)


# Começando

Nesta seção você entenderá um pouco melhor de onde surgiu o HTML, para que serve, e quais suas principais características.
## [Introdução](#índice)

HTML significa _**H**yper**T**ext **M**arkup **L**anguage_, e é a linguagem de marcação mais utilizada para a criação de páginas Web. 

Como seu nome sugere, ela é capaz de "marcar" o texto usando **_tags_**, uma espécie de rótulo para separar o texto em partes. 

Essa separação é entendida pelos navegadores, formatando diretamente os documentos com extensão **_.html_**, utilizando as tags de marcação para configurar os elementos do texto para a visualização.

O HTML foi desenvolvido por **_Tim Berners-Lee_** em 1990 com o propósito de trocar documentos formatados entre pesquisadores de diferentes universidades.

Sua invenção fez tanto sucesso que Tim é reconhecido hoje como _pai da web_.

Em 1996, a World Wide Web Consortium se tornou a autoridade responsável por manter as especificações da linguagem. Mas foi apenas em 2000 que a linguagem se tornou um padrão internacional (_ISO_).

A última versão do HTML é o **HTML5**. Ele garante uma execução mais rápida e mais robusta para o desenvolvimento web, com novos elementos estruturais para aumentar a leitura de páginas web, como **\<main\>**, **\<header\>**, **\<article\>** e **\<footer\>**.

### [Tags](#índice)

Como os principais elementos do HTML são escritos em _tags_, são esses elementos que dão características fundamentais da linguagem. 

Toda tag de marcação é composta por uma palavra chave, e cercada por colchetes angulares - os mesmos que representam os simbolos de "maior que" e "menor que" na matemática. Alguns exemplos são: **\<html\>**, **\<head\>**, **\<body\>**, **\<p\>**, e assim por diante.

As tags de HTML geralmente possuem um par, como **\<html\>** e **\</html\>**. A primeira Tag serve para abrir a estrutura, e a segunda para fechar. Você pode inserir conteúdo _entre as tags_ de abertura e fechamento de uma estrutura. 

Por exemplo, a tag **\<p\>** indica a marcação de um parágrafo, então qualquer conteúdo entre **\<p\>** e **\</p\>** é interpretado pelo navegador como uma estrutura de parágrafo, e você pode escrever essa estrutura da seguinte forma:

~~~html
<p>Isso é um parágrafo</p>
~~~

As tags de abertura e fechamento são idênticas, com exceção da barra **/** presente após a abertura da tag de fechamento, que serve para indicar ao navegador que aquela estrutura está sendo finalizada.

### [Estrutura](#índice)

O documento HTML é dividido basicamente em duas partes:

**Head** - contém a informação sobre o documento HTML, como o título da página, a versão do HTML, Meta Dados, entre outros.

**Body** - Contém todo o restante que será visualizado na página web.

Veja a seguir um exemplo de uma página de "Olá Mundo!":

~~~html
<html>
    <head></head>
    <body>
        <h1>Olá Mundo!</h1>
    </body>
</html>
~~~

Irei explicar sobre outras tags posteriormente.

### [Comentários](#índice)

Comentários são uma parte importante de qualquer código, eles servem para _melhorar a leitura_ do código por outros desenvolvedores, e são ignorados pelo navegador durante a execução.

É uma boa prática adicionar comentários, especialmente em documentos complexos, para indicar seções dentro do documento, ou adicionar anotações para qualquer um que vá ler o código.

Um comentário em HTML é inserido entre as tags \<!-- e --\>. Veja o mesmo exemplo, só que agora com comentários:

~~~html
<html>
    <head></head>
    <body>
        <h1>Olá Mundo!</h1>
        <!-- Isso é um comentário -->
    </body>
</html>
~~~

Qualquer conteúdo inserido entre as tags de comentário será completamente _ignorado_ pelo navegador.

## [Elementos](#índice)

Um elemento HTML é um componente individual que possui um significado ou semântica. Por exemplo, o elemento **título** representa o título do documento, podendo ser inserido entre a tag _head_ da seguinte forma:

~~~html
<html>
    <head>
        <title>Título do documento</title>
    </head>
    <body>
        <h1>Olá Mundo!</h1>
        <!-- Isso é um comentário-->
    </body>
</html>
~~~

A maioria dos elementos é escrito com uma tag de abertura e uma tag de fechamento. Elementos também podem ter _atributos_, que definem propriedades especiais.

Por exemplo, o parágrafo, representado pelo elemento p, poderia ser escrito da seguinte forma:

~~~html
<p class="exemplo">Um Parágrafo com atributo</p>
~~~

Onde:
- **\<p\>** é a tag de abertura
- **class="valor"** é o atributo, contendo o valor _exemplo_
- **Um Parágrafo com atributo** é o conteúdo desse elemento
- **\</p\>** é a tag de fechamento

### [Tags ou Elementos?](#índice)

Você deve estar pensando qual a diferença entre tags e elementos.

Tecnicamento, um **elemento** de HTML é um conjunto de componentes, entre eles a tag de abertura, seus atributos, a tag de fechamento, e qualquer conteúdo entre as tags.

Por outro lado, uma **tag** de HTML é usada para marcar o começo e o fim de um elemento. 

É muito comum que esses termos sejam intercaláveis, então não se preocupe muito com o nome, e sim com a estrutura.

### [Elementos Vazios](#índice)

A maioria dos elementos começa com uma tag de abertura e termina com uma tag de fechamento, que indicam onde o elemento começa e onde termina.

Contudo, existe um grupo de elementos que são uma exceção à regra. Esses elementos são chamados de vazios (_empty_ ou _void_).

Elementos vazios possuem apenas tag de abertura, porque nenhum conteúdo pode ser adicionado a eles. Entenda o exemplo com o elemento **br**.

~~~html
<p>Olá<br>Mundo</p>
~~~

Esse código ira exibir na tela algo semelhante a isso:

<p>Olá<br>Mundo</p>

O elemento _br_ cria uma quebra de linha. Outros elementos vazios muito comuns são **\<img\>**, **\<input\>**, **\<link\>**, **\<meta\>** e **\<hr\>**

### [Elementos Aninhados](#índice)

A maioria dos elementos HTML pode conter qualquer número de outros elementos (com exceção de elementos vazios), que são em sua maioria feitos por tags, atributos e conteúdo, e qualquer outro elemento.

O exemplo a seguir mostra como o elemento **p** pode conter outros elementos dentro dele, sem quebrar sua estrutura.

~~~html
<p><i>Olá</i><br><b>Mundo</b></p>
~~~

Essa linha de de código irá exibir na tela algo semelhante a isso:

<p><i>Olá</i><br><b>Mundo</b></p>

Repare como mesmo contendo outros elementos, a estrutura do parágrafo se manteve a mesma.

Você também deve ter reparado em dois novos estilos de marcação, o _itálico_ e o **negrito**, que são marcados pelos elementos **\<i\>** e **\<b\>**, respectivamente.

# [Formatação](#índice)

Agora que você já conhece o básico de HTML, vamos nos aprofundar mais na formatação e na estrutura semântica de uma página web.

## [Semântica](#índice)

Durante muito tempo, o HTML seguiu um padrão baseado em _divs_, uma estrutura que permitia a criação de pequenos blocos de conteúdo para organizar a página.

Porém, em 2014, com o advindo do HTML5, essa sopa de divs virou passado. Agora é possivel estruturar melhor as páginas, melhorando a _performance_ do conteúdo, e também permitindo uma maior _acessibilidade_. 

As principais estruturas você já viu, sendo elas os elementos **\<html\>**, **\<head\>** e **\<body\>**, mas vamos nos aprofundar no seu funcionamento. Entenda agora um pouco mais sobre os elementos semânticos que formam a estrutura da página.

***\<html\>*** - Essa tag é a raiz do seu documento, todos os elementos HTML devem estar dentro dela. Dentro da tag html definimos propriedades gerais, como informar ao navegador qual o idioma do documento.

***\<head\>*** - A tag head contém elementos que serão lidos pelo navegador, como os metadados - alguns exemplos são: a codificação de caracteres, o JavaScript com a tag script, folhas de estilo CSS e o título da página, com a tag title.

***\<body\>*** - Dentro da tag body podemos colocar todo o conteúdo visível ao usuário, como textos, imagens e vídeos.

### [**\<header\>**](#índice)

É o cabeçalho da página, geralmente contendo logomarcas, menus, campos de busca e informações pertinentes.

### [**\<article\>**](#índice)

Representa o conteúdo independente e de maior importância dentro da página, o conteúdo principal. Um article pode conter _elementos aninhados_, como header, cabeçalhos, parágrafos e imagens.

### [**\<aside\>**](#índice)

É a seção que engloba conteúdos relacionados ao conteúdo principal da página. Um bom exemplo são artigos relacionados, informações adicionais sobre o autor ou publicidade. Geralmente são posicionados como barras laterais.

### [**\<footer\>**](#índice)

Representa o rodapé do conteúdo, sendo aceito dentro de vários elementos, como _article_, _section_ e até do _body_. Exemplos de conteúdo dentro do footer são informações sobre o autor ou links relacionados.

### [**\<section\>**](#índice)

Representa uma seção genérica do conteúdo, quando não há nenhuma estrutura específica para ela.

Também podemos usar as tags de **\<h1\>** até **\<h6\>**. Elas não tem tanto valor semântico, sendo portadas de versões anteriores do HTML. Contudo, possuem um valor importante, denotando os títulos e subtítulos da página.

É importante usar apenas um **\<h1\>** por página, pois ele irá representar o objetivo e conteúdo principal dela, sendo usado como referência em pesquisas.