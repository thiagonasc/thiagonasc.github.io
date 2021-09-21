---
layout: post
title: 'Desenvolvendo com Bootstrap 3: um framework front-end que vale a pena!'
date: 2013-10-31 15:17:15.000000000 -02:00
type: post
published: true
status: publish
categories:
- desenvolvimento-web
tags:
- bootstrap
- bootstrap3
- css
- framework
- front-end
- html
- jquery
- xhtml
img:
 url:	bootstrap-logo.jpg
 alt:	Logotipo do bootstrap em fundo roxo
---


É engraçado como temos receio do novo. Me acostumei a desenvolver sites do zero, desde a primeira linha de código. Achava estranho a ideia de utilizar um <em>framework</em> para <em>front-end</em> até surgir a necessidade de criar e editar constantemente páginas e mais páginas de formulários. Neste cenário cresceu meu desejo de utilizar grids padronizados que facilitassem e agilizassem o desenvolvimento.

Após pesquisas e testes, decidi me aventurar com o **Bootstrap** e digo: vale e muito a pena!

## 1. Apresentação

![bootstrap-apresentacao](/assets/imgs/bootstrap-apresentacao.jpg){:.img-fluid.rounded}

Desenvolvido pela equipe do <a title="Visitar site" href="http://twitter.com/" target="_blank">Twitter</a>, o Bootstrap é um <em>framework</em> <em>front-end</em> de código aberto (<em>opensource</em>). Em palavras simples, é um conjunto de ferramentas criadas para facilitar o desenvolvimento de sites e sistemas web.

Compatível com HTML5 e CSS3, o <em>framework</em> possibilita a criação de layouts responsivos e o uso de gris, permitindo que seu conteúdo seja organizado em até 12 colunas e que comporte-se de maneira diferente para cada resolução.

Como qualquer outra ferramenta, possui suas vantagens e desvantagens. É importante conhecer e entender suas funcionalidades para saber os momentos certos de utilizá-lo.
<h3>Vantagens</h3>
<ul>
	<li>Possui documentação detalhada e de fácil entendimento;</li>
	<li>É otimizado para o desenvolvimento de layouts responsivos;</li>
	<li>Possui componentes suficientes para o desenvolvimento de qualquer site ou sistema web com interface simples;</li>
	<li>Facilita a criação e edição de layouts por manter padrões;</li>
	<li>Funciona em todos os navegadores atuais (Chrome, Safari, Firefox, IE, Opera).</li>
</ul>
<h3>Desvantagens</h3>
<ul>
	<li>Seu código terá de seguir os "padrões de desenvolvimento Bootstrap";</li>
	<li>Tema padrão e comum do Bootstrap (caso não faça ajustes visuais, seu projeto se parecerá com outros que também utilizam o Bootstrap).</li>
</ul>

## 2. Como funciona

![bootstrap-estrutura](/assets/imgs/bootstrap-estrutura.jpg){:.img-fluid.rounded}

A estrutura é simples e seu pacote contém três tipos diferentes de arquivos (CSS, JavaScrpipt e Fonts), que vêm devidamente organizados em suas pastas.

Montar um layout é simples e rápido utilizando sua <a title="Acessar documentação" href="http://getbootstrap.com/getting-started/" target="_blank">documentação</a>. Como toda a estrutura do CSS já vem definida, basta procurar o componente necessário e adicionar seu código. Em poucos minutos seu layout toma forma e está pronto para uso! E o mesmo acontece com o JavaScript.
<h3>O sistema de grids</h3>

O uso efetivo dos grids é fundamental para um bom projeto com o Bootstrap e entender sua lógica é simples.

O sistema de grids possibilita a divisão em até 12 colunas de mesma largura:

![bootstrap-grid-1](/assets/imgs/bootstrap-grid-1.jpg){:.img-fluid.rounded}

Se você não deseja dividir seu conteúdo, basta usar uma única coluna de largura 12 (Caso 1).

Se você deseja dividir seu conteúdo em 2 partes iguais, de mesma largura, basta criar 2 colunas de largura 6 cada uma (Caso 2).

Se você deseja dividir seu conteúdo em 4 partes iguais, de mesma largura, basta criar 4 colunas de largura 4 cada uma (Caso 3).

![bootstrap-grid-2](assets/imgs/bootstrap-grid-22.jpg){:.img-fluid.rounded}

A mesma lógica se segue para qualquer divisão. Portanto se você deseja dividir seu conteúdo em 4 partes diferentes, utilizando larguras diferentes para cada coluna, basta criá-las, cada uma com sua largura específica, de modo que o resultado da soma das larguras seja sempre 12 (exemplos abaixo).

![bootstrap-grid-2](/assets/imgs/bootstrap-grid-21.jpg){:.img-fluid.rounded}

O uso de grids possibilita mudar o visual de um site ou sistema de maneira fácil e rápida, alterando apenas o valor da largura das colunas.

E o melhor vem agora: as grids são nativamente responsivas! Você pode definir grids diferentes para cada tipo de resolução. Esses comportamentos são definidos através das classes xs (dispositivos muito pequenos), sm (dispositivos pequenos), md (dispositivos médios) e lg (dispositivos grandes).

![bootstrap-grid-responsive](/assets/imgs/bootstrap-grid-responsive.jpg){:.img-fluid.rounded}

## 3. Criando o primeiro projeto

![bootstrap-projeto](/assets/imgs/bootstrap-projeto.jpg){:.img-fluid.rounded}

Faça o download da versão compilada do **Bootstrap** no <a title="Visitar site oficial" href="http://getbootstrap.com/" target="_blank">site oficial</a> e descompacte os arquivos para iniciar seu projeto.

Crie um arquivo HTML (na raíz da pasta) utilizando a estrutura básica abaixo:

{% highlight html linenos %}
<meta charset="utf-8" />
Bootstrap Template
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- Carregando o CSS do Bootstrap -->
        <link href="css/bootstrap.min.css" rel="stylesheet" media="screen" /></pre>
<h1>Olá, mundo!</h1>
<pre>
    <!-- jQuery (plugins em JavaScript) -->
<script type="text/javascript" src="https://code.jquery.com/jquery.js"></script><script type="text/javascript" src="js/bootstrap.min.js"></script>
{% endhighlight %}

O código declara o HTML5, carrega os arquivos necessários (CSS + JavaScript) e define uma estrutura básica para o projeto.

Concluído! O **Bootstrap** está configurado e pronto para receber suas linhas!

O site oficial disponibiliza alguns <a title="Visitar templates de exemplo" href="http://getbootstrap.com/getting-started/#examples" target="_blank">templates de exemplo</a> que são bastante úteis, principalmente para quem começa a se aventurar agora.

## 4. Conclusão

![bootstrap-produtividade](/assets/imgs/bootstrap-produtividade.jpg){:.img-fluid.rounded}

Altamente recomendado para desenvolvedores inciantes com conhecimento básico em HTML e CSS, desenvolvedores avançados que buscam o aumento da produtividade (utilizando recursos como o sistema de grids) e programadores back-end, o Bootstrap possui recursos e componentes suficientes para desenvolver um site ou sistema web por completo.

Como já dito, há vantagens e desvantagens, indicações e contra-indicações de seu uso, assim como qualquer outro <em>framework</em>. O importante é entender seu funcionamento para saber o momento certo de usá-lo.

Por fim, uma coisa é inegável: **Bootstrap** aumenta sua produtividade de desenvolvimento, tornando fácil a criação e edição de páginas responsivas.
