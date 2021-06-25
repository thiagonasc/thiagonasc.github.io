---
layout:		page
title:		Links
permalink:	/links/

categorias:
  - titulo: "Inspirações"
    itens:
      - nome:	"Behance"
        url:	"https://www.behance.net/"
      - nome:	"Dribbble"
        url:	"https://dribbble.com/"
      - nome:	"Awwwards"
        url:	"https://www.awwwards.com/"
      - nome:	"Mobbin (Mobile Design)"
        url:	"https://mobbin.design/"
  - titulo: "Cores"
    itens:
      - nome:	"Adobe Colors"
        url:	"https://color.adobe.com/pt/explore"
      - nome:	"Coolors"
        url:	"https://coolors.co/palettes/trending"
  - titulo: "Fontes"
    itens:
      - nome:	"Google Font"
        url:	"https://fonts.google.com/"
      - nome:	"Adobe Font"
        url:	"https://fonts.adobe.com/"
      - nome:	"Dafont"
        url: 	"http://www.dafont.com"
  - titulo: "Fotografias"
    itens:
      - nome:	"Pexels"
        url:	"https://www.pexels.com/"
      - nome:	"Pixabay"
        url:	"https://pixabay.com/"
      - nome:	"Unsplash"
        url:	"https://unsplash.com/"
      - nome:	"Stockvault"
        url:	"https://www.stockvault.net/"
  - titulo: "Ícones"
    itens:
      - nome:	"Font Awesome"
        url:	"https://fontawesome.com/"
      - nome:	"Icons 8"
        url:	"https://icons8.com.br/icons"
      - nome:	"flaticon"
        url:	"https://www.flaticon.com/br/"
      - nome:	"The Noun Project"
        url:	"https://thenounproject.com/icons/"
  - titulo: "Ilustrações"
    itens:
      - nome:	"O! Ouch"
        url:	"https://icons8.com.br/illustrations"
      - nome:	"Blush Design"
        url:	"https://blush.design/pt/collections"
      - nome:	"Pixabay"
        url:	"https://pixabay.com/"
  - titulo: "Frameworks Front-end"
    itens:
      - nome: "Bootstrap"
        url:  "https://getbootstrap.com/"
      - nome: "Tailwind CSS"
        url:  "https://tailwindcss.com/"
      - nome: "Foundation"
        url:  "https://get.foundation/"
      - nome: "Bulma"
        url:  "https://bulma.io/"
      - nome: "UIkit"
        url:  "https://getuikit.com/"
      - nome: "Materialize"
        url:  "https://materializecss.com/"
      - nome: "Element"
        url:  "https://element.eleme.io/"
  - titulo: "Outros compilados de links"
    itens:
      - nome: "Design Notes"
        url:  "https://www.designnotes.co/"
      - nome: "Design Resources"
        url:  "https://www.designresourc.es/"
        
---

<p>Compartilho aqui links dos sites que mais utilizo para referências e recursos:</p>

{% for categoria in page.categorias %}
<div class="row mb-4">
	<div class="col-sm-3 mr-1">
		<h3 id="{{ categoria.titulo }}">{{ categoria.titulo }}</h3>
	</div>
	<div class="col-sm-9">
		<ul>
			{% for item in categoria.itens %}
			<li><a target="_blank" href="{{ item.url }}">{{ item.nome }} ↗</a></li>
			{% endfor %}
		</ul>
	</div>
</div>
{% endfor %}