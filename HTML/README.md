# HTML

## Índice

1. [Introdução](#introdução)
    1. [Tags](#tags)
    2. [Estrutura](#estrutura)
    3. [Comentários](#comentários)

## [Introdução](#índice)

HTML significa _**H**yper**T**ext **M**arkup **L**anguage_, e é a linguagem de marcação mais utilizada para a criação de páginas Web. 

Como seu nome sugere, ela é capaz de "marcar" o texto usando **_tags_**, uma espécie de rótulo paara separar o texto em partes. 

Essa separação é entendida pelos navegadores, formatando diretamente os documentos com extensão **_.html_** utilizando as tags de marcação para configurar os elementos do texto para a visualização.

O HTML foi desenvolvido por **_Tim Berners-Lee_** em 1990 com o propósito de trocar documentos formatados entre pesquisadores de diferentes universidades.

Sua invenção fez tanto sucesso que Tim é reconhecido hoje como _pai da web_.

Em 1996, a World Wide Web Consortium se tornou a autoridade responsável por manter as especificações da linguagem. Mas foi apenas em 2000 que a linguagem se tornou um padrão internacional (_ISO_).

A última versão do HTML é o **HTML5**. Ele garante uma execução mais rápida e mais robusta para o desenvolvimento web, com novos elementos estruturais para aumentar a redabilidade das páginas web, como **\<main\>**, **\<header\>**, **\<article\>** e **\<footer\>**.

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
        <!-- Isso é um comentário-->
    </body>
</html>
~~~

Qualquer conteúdo inserido entre as tags de comentário será completamente _ignorado_ pelo navegador.

