---
layout:		page
title:		Livros
permalink:	/livros/

livro:
 lendo:
  1:
   titulo: "Pipeline de Liderança"
   subtitulo: "O desenvolvimento de líderes como diferencial competitivo."
   autor: "Ram Charan, Stephen Drotter, James Noel"
   url: "https://amzn.to/3BKE9DV"
   img-asin: "8543106052"
  2:
   titulo: "A Startup Enxuta"
   subtitulo: "Como usar a inovação contínua para criar negócios radicalmente bem-sucedidos."
   autor: "Eric Ries"
   url: "https://amzn.to/2ROZg5M"
   img-asin: "8543108624"

 lidos-2021:
  1:
   titulo: "Ikigai"
   subtitulo: "Os cinco passos para encontrar seu propósito de vida e ser mais feliz."
   autor: "Ken Mogi"
   url: "https://amzn.to/3zmQkWi"
   img-asin: "8582467311"
  2:
   titulo: "Simplificando coisas que parecem complicadas"
   subtitulo: "O guia do tipo faça você mesmo para descobrir e consertar problemas de usabilidade."
   autor: "Steve Krug"
   url: "https://amzn.to/3c6JTNZ"
   img-asin: "8576084511"
  3:
   titulo: "Essencialismo"
   subtitulo: "A busca disciplinada por menos."
   autor: "Greg McKeown"
   url: "https://amzn.to/390Fklb"
   img-asin: "8543102146"
 
 lidos-2020:
  1:
   titulo: "Fora da Curva"
   subtitulo: "Os segredos dos grandes investidores do Brasil e o que você pode aprender com eles."
   autor: "Vários atores"
   url: "https://amzn.to/3viGEsz"
   img-asin: "8582850123"
  2:
   titulo: "Trabalhe 4 horas por semana"
   subtitulo: "Fuja da rotina, viva onde quiser e fique rico."
   autor: "Timothy Ferriss"
   url: "https://amzn.to/3wxyIVC"
   img-asin: "8542211561"
   resenha: livro-trabalhe-4-horas-por-semana
  3:
   titulo: "Sprint a Sprint"
   subtitulo: "Erros e acertos na transformação cultural de um time ágil."
   autor: "Mary Provinciatto, Paulo Caroli"
   url: "https://amzn.to/3pMZsiB"
   img-asin: "6586660009"
   resenha: resenha-livro-sprint-a-sprint
  4:
   titulo: "Sprint"
   subtitulo: "O Método Usado no Google Para Testar e Aplicar Novas Ideias em Apenas Cinco Dias."
   autor: "Jake Knapp, John Zeratsky, Braden Kowitz"
   url: "https://amzn.to/3gm40JM"
   img-asin: "8551001523"
   resenha: resenha-livro-sprint
  5:
   titulo: "O poder da inteligência emocional"
   subtitulo: "Como liderar com sensibilidade e eficiência."
   autor: "Daniel Goleman, Annie McKee, Richard Boyatzis"
   url: "https://amzn.to/3pMG9Ws"
   img-asin: "8547000631"

 lidos-outros:
  1:
   titulo: "TED Talks"
   subtitulo: "O guia oficial do TED para falar em público."
   autor: "Chris Anderson"
   url: https://amzn.to/35i2Fxg
   img-asin: 858057935X
   resenha: resenha-ted-talks-livro

  # 1:
  #  titulo: "titulo"
  #  subtitulo: "subtitulo"
  #  autor: "autor"
  #  url: "url"
  #  img-asin: "asin"

---

Acompanhe aqui minhas principais leituras em andamento e finalizadas. Alguns deles contam com uma breve resenha publicada no blog (os links estão abaixo).

Para adquirir qualquer título, basta clicar na capa do livro abaixo:

## Lendo

<div class="row row-cols-1 row-cols-md-4">
	{% for livro in page.livro.lendo %}
	<div class="feature col py-4">
		<div class="feature-icon">
			<a href="{{ livro[1].url }}" target="_blank">
				<img class="img-thumbnail" src="//ws-na.amazon-adsystem.com/widgets/q?_encoding=UTF8&ASIN={{ livro[1].img-asin }}&Format=_SL160_&ID=AsinImage&MarketPlace=BR&ServiceVersion=20070822&WS=1&tag=thiagonasc-20&language=pt_BR" alt="...">
			</a>
		</div><br>
		<h5 class="card-title">
			{{ livro[1].titulo }}<br>
			<small class="text-muted">{{ livro[1].autor }}</small>
		</h5>
		<p>{{ livro[1].subtitulo }}</p>
		{%- if livro[1].resenha -%}<a href="{{ livro[1].resenha }}" class="icon-link">Ler resenha »</a><br>{%- endif -%}
		<a href="{{ livro[1].url }}" class="icon-link" target="_blank">Ver na Amazon »</a>
	</div>
	{% endfor %}
</div>

## Lidos

<br>

### 2021

<div class="row row-cols-1 row-cols-md-4">
	{% for livro in page.livro.lidos-2021 %}
	<div class="feature col py-4">
		<div class="feature-icon">
			<a href="{{ livro[1].url }}" target="_blank">
				<img class="img-thumbnail" src="//ws-na.amazon-adsystem.com/widgets/q?_encoding=UTF8&ASIN={{ livro[1].img-asin }}&Format=_SL160_&ID=AsinImage&MarketPlace=BR&ServiceVersion=20070822&WS=1&tag=thiagonasc-20&language=pt_BR" alt="...">
			</a>
		</div><br>
		<h5 class="card-title">
			{{ livro[1].titulo }}<br>
			<small class="text-muted">{{ livro[1].autor }}</small>
		</h5>
		<p>{{ livro[1].subtitulo }}</p>
		{%- if livro[1].resenha -%}<a href="{{ livro[1].resenha }}" class="icon-link">Ler resenha »</a><br>{%- endif -%}
		<a href="{{ livro[1].url }}" class="icon-link" target="_blank">Ver na Amazon »</a>
	</div>
	{% endfor %}
</div>

### 2020

<div class="row row-cols-1 row-cols-md-4">
	{% for livro in page.livro.lidos-2020 %}
	<div class="feature col py-4">
		<div class="feature-icon">
			<a href="{{ livro[1].url }}" target="_blank">
				<img class="img-thumbnail" src="//ws-na.amazon-adsystem.com/widgets/q?_encoding=UTF8&ASIN={{ livro[1].img-asin }}&Format=_SL160_&ID=AsinImage&MarketPlace=BR&ServiceVersion=20070822&WS=1&tag=thiagonasc-20&language=pt_BR" alt="...">
			</a>
		</div><br>
		<h5 class="card-title">
			{{ livro[1].titulo }}<br>
			<small class="text-muted">{{ livro[1].autor }}</small>
		</h5>
		<p>{{ livro[1].subtitulo }}</p>
		{%- if livro[1].resenha -%}<a href="{{ livro[1].resenha }}" class="icon-link">Ler resenha »</a><br>{%- endif -%}
		<a href="{{ livro[1].url }}" class="icon-link" target="_blank">Ver na Amazon »</a>
	</div>
	{% endfor %}
</div>

### Outros anos

<div class="row row-cols-1 row-cols-md-4">
	{% for livro in page.livro.lidos-outros %}
	<div class="feature col py-4">
		<div class="feature-icon">
			<a href="{{ livro[1].url }}" target="_blank">
				<img class="img-thumbnail" src="//ws-na.amazon-adsystem.com/widgets/q?_encoding=UTF8&ASIN={{ livro[1].img-asin }}&Format=_SL160_&ID=AsinImage&MarketPlace=BR&ServiceVersion=20070822&WS=1&tag=thiagonasc-20&language=pt_BR" alt="...">
			</a>
		</div><br>
		<h5 class="card-title">
			{{ livro[1].titulo }}<br>
			<small class="text-muted">{{ livro[1].autor }}</small>
		</h5>
		<p>{{ livro[1].subtitulo }}</p>
		{%- if livro[1].resenha -%}<a href="{{ livro[1].resenha }}" class="icon-link">Ler resenha »</a><br>{%- endif -%}
		<a href="{{ livro[1].url }}" class="icon-link" target="_blank">Ver na Amazon »</a>
	</div>
	{% endfor %}
</div>