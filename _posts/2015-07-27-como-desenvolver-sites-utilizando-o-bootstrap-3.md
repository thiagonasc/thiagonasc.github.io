---
layout: post
title: Como desenvolver sites utilizando o Bootstrap 3
date: 2015-07-27 23:15:21.000000000 -03:00
type: post
published: true
status: publish
categories:
- geral
tags: []
img:
 url:	bootstrap-logo-code.jpg
 alt:	Logotipo do Bootstrap sobre fundo de códigos de programação
---

No artigo <a href="http://thiagonasc.com/desenvolvimento-web/desenvolvendo-com-bootstrap-3-um-framework-front-end-que-vale-a-pena" target="_blank" rel="noopener">Desenvolvendo com Bootstrap 3: um framework front-end que vale a pena!</a> fiz uma breve apresentação do <em>framework</em> apontando seus pontos positivos e negativos, explicando o funcionamento do sistema de grids e como se inicia um projeto.

Mas agora chegou a hora de colocar a mão na massa pra valer!

Em 6 etapas, você desenvolverá o seu primeiro site utilizando o <em><strong>Bootstrap</strong></em>.

## 1. Fase de concepção

Antes de sair desenvolvendo qualquer página, é importante demandar tempo em entender a real necessidade e objetivo do que será criado.

Esta é uma das fases mais importantes do ciclo de vida de um projeto e constantemente negligenciadas pelos desenvolvedores, no anseio de se ter um produto a ser usado em pouco tempo.

Mas pare e pense: nada adianta uma página bem desenvolvida se ela não atende o objetivo de seu idealizador ou a real necessidade do usuário.

Portanto se inspire, pense, rabisque, faça <em>brainstorm’s</em>, peça opiniões, enfim, demande tempo... o quanto necessário, pois valerá a pena, pode confiar. ;)

![Homem rascunhando em papel o desenho de um aplicativo](/assets/imgs/site-concepcao-sketch.jpg){:.img-fluid.rounded}

<em>Como <strong>exemplo de caso</strong>, desenvolveremos um site com o objetivo de divulgar informações pessoais e profissionais de um indivíduo. A fase de concepção portanto se dá em descobrir quais serão esses dados e quais suas importâncias (para já se ter uma idéia da organização e disposição do conteúdo).</em>

<em><strong>Dados a serem disponibilizados:</strong> nome, cargo, foto, resumo, telefone, email, localidade, experiências profissionais, habilidades, paixões e hobbies.</em>

## 2. Defina a estrutura do layout pensando em grids

Com a concepção elaborada, chegou a hora de definir o layout, isto é, a estrutura visual de seu site.

Lembre-se de sempre pensar em grids! O <em><strong>Bootstrap</strong></em> trabalha com até 12 colunas e seu layout deve respeitar esses limites. <em>(O sistema de grids foi explicado no artigo citado no início desta postagem - <a href="http://thiagonasc.com/desenvolvimento-web/desenvolvendo-com-bootstrap-3-um-framework-front-end-que-vale-a-pena" target="_blank" rel="noopener">ver artigo</a>).</em>

Através de desenhos bem simples (chamados de <em>wireframes</em>) feitos à mão ou no próprio computador, você definirá onde e como ficará cada componente de seu site como o menu de navegação, rodapé, conteúdo e o que mais tiver.

![Imagem mostrando o layout sobrepondo os grids do bootstra](/assets/imgs/wireframe-bootstrap.gif){:.img-fluid.rounded}

No <em>wireframe</em> acima é possível perceber a distribuição do conteúdo respeitando o sistema de <em>grids</em> (colunas de contorno azul), dividido em 12 porções iguais.

## 3. Preparando o ambiente

Em sua forma mais simples de utilização, preparar um ambiente utilizando <strong><em>Bootstrap</em></strong> é extremamente fácil e rápido.

Acesse a página oficial do <em>framework</em> (<a href="http://www.getbootstrap.com/" target="_blank" rel="noopener">http://www.getbootstrap.com/</a>) e faça o <em>download</em> de sua versão compilada.

![Seta apontando para o botão de download do Bootstrap](/assets/imgs/bootstrap-download.jpg){:.img-fluid.rounded}

Descompacte o arquivo zip no local desejado e seu ambiente está <strong>pronto</strong>! Simples, não? =D

## 4. Criando a estrutura do HTML

Crie o arquivo “<strong>index.html</strong>” no diretório raíz e insira o código ‘padrão’ da estrutura do <em>Bootstrap</em> disponível abaixo:

{% highlight html linenos %}
<!DOCTYPE html>
<html lang="pt-BR">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
        <title>Bootstrap - Template básico</title>
 
        <!-- Bootstrap -->
        <link href="css/bootstrap.min.css" rel="stylesheet">
 
        <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
        <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
        <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
        <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
        <![endif]-->
    </head>
    <body>
        <h1>Olá, mundo!</h1>
 
        <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
        <!-- Include all compiled plugins (below), or include individual files as needed -->
        <script src="js/bootstrap.min.js"></script>
    </body>
</html>
{% endhighlight %}


Estrutura pronta, vamos iniciar a codificação do <em>layout</em>.

## 5. Codificando a estrutura do <em>layout</em> e <em>grids</em>

Para o exemplo, vamos dividir esta etapa em quatro itens:
<h3>5.1. Definindo os componentes principais</h3>

Nosso <em>layout</em> possui 3 componentes horizontais:

<strong>1. cabeçalho: </strong><em>header;<br />
</em><strong>2. seção principal: </strong><em>section;<br />
</em><strong>3. rodapé: </strong><em>footer</em>.

![Divisões estruturais da página em divs horizontais](/assets/imgs/grid-horizontal.gif){:.img-fluid.rounded}

O código a ser inserido dentro do &lt;body&gt;&lt;/body&gt; de nosso arquivo "index.html" para realizar esta separação é bastante simples:

{% highlight html linenos %}
<header>
    <nav>HEADER > NAV</nav>
</header>
 
<section>
    <aside>SECTION > ASIDE</aside>
    <article>SECTION > ARTICLE</article>
</section>
 
<footer>FOOTER</footer>
{% endhighlight %}


Com as estruturas horizontais prontas, partimos para codificação de cada componente e suas divisões em grids, ou seja, as divisões em colunas do <em>layout</em>.
<h3>5.2. Codificando o cabeçalho (header) com a barra de navegação</h3>

O <em><strong>Bootstrap</strong></em> já possui uma barra de navegação (ou <em>navbar</em>) como um componente pronto para uso (e isso significa que você não precisará codificar uma linha sequer para isso). ;)

Basta entrar na documentação disponível no site oficial <a href="http://www.getbootstrap.com" target="_blank" rel="noopener">http://www.getbootstrap.com</a> e procurar pela <em>navbar</em> na página de <a href="http://getbootstrap.com/components/" target="_blank" rel="noopener">componentes</a>.

Copie e cole o código da barra de navegação dentro de sua <em>header</em>.

Perceba que a documentação disponibiliza algumas customizações para cada componente, um exemplo é a possibilidade de tornar a barra de navegação fixa ao topo ou utilizá-la com suas cores invertidas, como é o nosso caso.

Dois pontos importantes a serem observados:

1. Para que os elementos fiquem centralizados na página, basta utilizar a classe "container" nos elementos superiores de cada seção.

2. Quando utiliza-se a barra de navegação fixa no topo, é necessário adicionar um espaçamento<em> (margin-top)</em> ao elemento inferior para evitar que a mesma sobreponha a <em>navbar</em>.

O código para nosso exemplo ficará assim:

{% highlight html linenos %}
<header><!-- Cabeçalho -->
    <nav class="navbar navbar-inverse navbar-fixed-top">
        <div class="container">
            <!-- Brand and toggle get grouped for better mobile display -->
            <div class="navbar-header">
                <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
                    <span class="sr-only">Toggle navigation</span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="#">nome do site</a>
            </div>
 
            <!-- Collect the nav links, forms, and other content for toggling -->
            <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
                <ul class="nav navbar-nav navbar-right">
                    <li><a href="#">Link 1</a></li>
                    <li><a href="#">Link 2</a></li>
                    <li><a href="#">Link 3</a></li>
                    <li><a href="#">Link 4</a></li>
                </ul>
            </div><!-- /.navbar-collapse -->
        </div><!-- /.container -->
    </nav>
</header><!-- Cabeçalho-fim -->
{% endhighlight %}

<h3>5.3. Codificando o componente central (section) e seus grids</h3>

Chegou o momento de trabalhar efetivamente com os <em>grids</em> (visto que não precisamos dele no cabeçalho, uma vez que utilizamos o componente pronto).

Conforme o desenho do <em>layout</em>, o componente central, definido na estrutura do HTML como <em>section,</em> deverá receber duas colunas:

<strong>1.<em> aside</em> (elemento à esquerda):</strong> onde virão os detalhes do profissional como a foto, nome, e-mail, telefone, etc;

<strong>2.<em> article </em>(elemento à direita):</strong> elemento principal, onde virão os textos e descrições mais detalhadas.

![Divisão em grids do layout utilizando o bootstrap](/assets/imgs/aside-article-2.jpg){:.img-fluid.rounded}

<em><strong>Lembrando as regras do sistema de grids:</strong> as colunas devem estar inseridas na &lt;div class="row"&gt;&lt;/div&gt; e a soma das mesmas não podem ultrapassar 12.</em>

Para o exemplo, utilizaremos a seguinte proporção: 'md-3' para o elemento <em>aside</em> e 'md-9' para o <em>article</em> (somando 12 no total, preenchendo assim a largura da página).

<em>Obs: foi adicionado o margin-top à section, evitando que a mesma sobreponha a barra de navegação.</em>

O código de nossa <em>section </em>portanto ficará assim:

{% highlight html linenos %}
<section class="container" style="margin-top:100px;">
    <aside class="col-md-3">
        aside
    </aside>
    <article class="col-md-9">
        article
    </article>
</section>
{% endhighlight %}

<h3>5.4. Codificando o rodapé (footer)</h3>

Nosso rodapé<em> (</em>footer)<em> </em>seguirá a mesma lógica do elemento anterior <em>(section)</em>, porém as proporções serão invertidas. Utilizaremos 'md-9' para a coluna da data de última atualização e 'md-3' para a coluna dos créditos.

Tendo o seguinte código:

{% highlight html linenos %}
<footer class="container">
    <hr>
    <div class="row">
        <div class="col-xs-9">Última atualização</div>
        <div class="col-xs-3 text-right">Créditos</div>
    </div>
</footer>
{% endhighlight %}

<h3>5.5. Código completo</h3>

O resultado é o seguinte código:

{% highlight html linenos %}
<!DOCTYPE html>
<html lang="pt-BR">
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
        <title>Bootstrap - Template básico</title>
 
        <!-- Bootstrap -->
        <link href="css/bootstrap.min.css" rel="stylesheet">
 
        <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
        <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
        <!--[if lt IE 9]>
        <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
        <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
        <![endif]-->
    </head>
    <body>
 
        <header><!-- Cabeçalho -->
            <nav class="navbar navbar-inverse navbar-fixed-top">
                <div class="container">
                    <!-- Brand and toggle get grouped for better mobile display -->
                    <div class="navbar-header">
                        <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
                            <span class="sr-only">Toggle navigation</span>
                            <span class="icon-bar"></span>
                            <span class="icon-bar"></span>
                            <span class="icon-bar"></span>
                        </button>
                        <a class="navbar-brand" href="#">nome do site</a>
                    </div>
 
                    <!-- Collect the nav links, forms, and other content for toggling -->
                    <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
                        <ul class="nav navbar-nav navbar-right">
                            <li><a href="#">Link 1</a></li>
                            <li><a href="#">Link 2</a></li>
                            <li><a href="#">Link 3</a></li>
                            <li><a href="#">Link 4</a></li>
                        </ul>
                    </div><!-- /.navbar-collapse -->
                </div><!-- /.container -->
            </nav>
        </header><!-- Cabeçalho-fim -->
 
        <section class="container" style="margin-top:100px;">
            <aside class="col-md-3">
                aside
            </aside>
            <article class="col-md-9">
                article
            </article>
        </section>
 
        <footer class="container">
            <hr>
            <div class="row">
                <div class="col-xs-9">Última atualização</div>
                <div class="col-xs-3 text-right">Créditos</div>
            </div>
        </footer>
 
        <!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
        <!-- Include all compiled plugins (below), or include individual files as needed -->
        <script src="js/bootstrap.min.js"></script>
    </body>
</html>
{% endhighlight %}

## 6. Insira o conteúdo e publique!

<em>Layout</em> codificado, agora basta inserir os conteúdos e publicar.

<strong>Resultado final:</strong>

![Layout final desenvolvido em bootstrap](/assets/imgs/screenshot-resultado-final.jpg){:.img-fluid.rounded}

<a class="btn btn-lg btn-success" href="https://htmlpreview.github.io/?https://github.com/thiagonasc/bootstrap-3-templates/blob/master/index.html" target="_blank" role="button"><span class="glyphicon glyphicon-eye-open"></span> Ver demo</a>
<a class="btn btn-lg btn-success" href="https://github.com/thiagonasc/bootstrap-3-templates/archive/master.zip" target="_blank" role="button"><span class="glyphicon glyphicon-download-alt"></span> Baixar projeto</a>
<a class="btn btn-lg btn-success" href="https://github.com/thiagonasc/bootstrap-3-templates" target="_blank" role="button"><span class="glyphicon glyphicon-inbox"></span> Repositório no GitHub</a>

O mais legal: seu site está funcional e responsivo para diversos dispositivos com resoluções diferentes, seja smartphones, tablets, notebooks ou desktops.
