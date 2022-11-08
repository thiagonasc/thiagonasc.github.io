---
layout: post
title: 'Paginação tradicional: como os grandes sites utilizam'
description: ''
date: 2022-11-07 22:20:00 -03:00
type: post
published: true
status: publish
comments: true
categories:
- usabilidade
---

<!-- ---

1. [Apresentação](#apresentacao)
2. [Paginação vs. Rolagem Infinita](#paginacaovsrolageminfinita)
3. Como os grandes projetos utilizam:
	1. AliExpress

--- -->

<a class="anchor" name="apresentacao"></a>

Tempos atrás escrevi o breve artigo [Paginação: boas práticas de uso para uma experiência perfeita][1]{:target="_blank"}. E mesmo passado o tempo, as práticas ali descritas permanecem úteis.

De simples sistemas à produtos robustos, é fácil notar a importância da paginação: onde há diversos registros a serem exibidos - condição presente na quase totalidade dos sistemas - se faz necessário um recurso que permita uma boa experiência ao listá-los.

E ainda que tenhamos inúmeros bons exemplos, é comum encontrar paginações que oferecem uma má experiência ao usuário.

Por fim, analisar como o recurso é aplicado em projetos de referência em nível nacional e até internacional, com certeza é uma prática bastante eficiente!

<a class="anchor" name="paginacaovsrolageminfinita"></a>

<br>

## Paginação vs. Rolagem infinita

Para começo, é importante classificarmos dois dos recursos mais comuns na listagem de diversos registros:

![Recorte da funcionalidade de paginação do Booking](../../assets/imgs/paginacao/paginacao-tradiciona-vs-rolagem-infinita.jpg){:.img-fluid.rounded}

1. **Paginação:** (tradicional) dividem-se os registros em pequenas partes, geralmente denominadas de 'páginas', e o acesso aos mesmos se dá por meio destas porções, listadas individualmente. A medida que uma nova parte é requerida, os antigos registros dão lugar aos novos. Simples como numa página de livro.

2. **Rolagem infinita:** (inifinite-scroll) alguns registros são inicialmente listados, geralmente os mais recentes e à medida que a página é percorrida, novos registros são listados e exibidos, mantendo os anteriores. É comum vermos botões como 'Ver mais' ou somente um 'Carregando...' ao fim dos registros atuais antes que os novos sejam requeridos.

É notório que a maioria das redes sociais utilizam do segundo recurso, a rolagem infinita. O objetivo é evidente: minimizar o esforço e por consequência aumentar a retenção dos usuários.

Quem nunca passou minutos, talvez horas, rolando o dedo na tela para ver mais conteúdos? Chega a ser viciante, não? No entanto, mesmo este recurso possui seus prós e contras. Há inclusive um artigo recém publicado no [Nielsen Norman Group][9], que vale a leitura: [Rolagem infinita - Quando usar, Quando evitar][10] *(artigo em inglês)*.

Exemplos de grandes plataformas que utilizam a rolagem infinita: [Instagram][2], [Tik Tok][3], [Twitter][4], [YouTube][5], [Facebook][6], [LinkedIn][7], [Reddit][8] e outros.

Mas nos concentraremos em analisar, como o próprio título diz, nas **paginações tradicionais**. Vamos lá?

<br>

## Critérios de seleção e análise

Foram selecionados alguns dos principais sites mais acessados no Brasil (segundo [SEM Rush][11]) e que utilizam, é claro, recursos de paginação tradicional.

Para cada site, foram tirados printscreens em 3 momentos distintos de sua utilização: primeira página, página intermediária e última página.

<br>

## Exemplos de usos em grandes sites

![Recorte da funcionalidade de paginação do site AliExpress. ](../../assets/imgs/paginacao/paginacao-aliexpress.jpg){:.img-fluid.rounded.border.border.mt-4}
[AliExpress][12]

_Arrisco-me dizer que a funcionalidade **Ir para a página** é raramente utilizada. Talvez se removida, nem faça falta. Pelo contrário, simplifique a interface e facilite a experiência (menos é mais)._


![Recorte da funcionalidade de paginação da Amazon](../../assets/imgs/paginacao/paginacao-amazon.jpg){:.img-fluid.rounded.border.mt-4}
[Amazon][13]

![Recorte da funcionalidade de paginação do Booking](../../assets/imgs/paginacao/paginacao-booking.jpg){:.img-fluid.rounded.border.mt-4}
[Booking][14]

![Recorte da funcionalidade de paginação do Gmail](../../assets/imgs/paginacao/paginacao-gmail.jpg){:.img-fluid.rounded.border.mt-4}
[Gmail][15]

![Recorte da funcionalidade de paginação do Google](../../assets/imgs/paginacao/paginacao-google.jpg){:.img-fluid.rounded.border.mt-4}
[Google][16]

_Já havia percebido que a letra "O" em vermelho vai percorrendo o logo do Google à medida em que se avançam as páginas? Repare na imagem acima! (é quase um Easter Egg)_

![Recorte da funcionalidade de paginação das Lojas Americanas](../../assets/imgs/paginacao/paginacao-lojas-americanas.jpg){:.img-fluid.rounded.border.mt-4}
[Lojas Americanas][17]

![Recorte da funcionalidade de paginação da Magalu](../../assets/imgs/paginacao/paginacao-magalu.jpg){:.img-fluid.rounded.border.mt-4}
[Magalu][18]

![Recorte da funcionalidade de paginação do Mercado Livre](../../assets/imgs/paginacao/paginacao-mercado-livre.jpg){:.img-fluid.rounded.border.mt-4}
[Mercado Livre][19]

![Recorte da funcionalidade de paginação do OLX](../../assets/imgs/paginacao/paginacao-olx.jpg){:.img-fluid.rounded.border.mt-4}
[OLX][20]

_Considero este um bom exemplo de que mesmo grandes sites podem **não** projetar as interfaces mais amigáveis. Há quebra de layout na página intermediária; e o mais estranho, repare o botão **última página** sendo substituído por **primeira página** no 3º momento._ 🤦🏻‍♂️

_Seria este um loop intencional para retenção do usuário?_ 🤷🏻‍♂️

![Recorte da funcionalidade de paginação da Shopee](../../assets/imgs/paginacao/paginacao-shopee.jpg){:.img-fluid.rounded.border.mt-4}
[Shopee][21]

<br>

## Conclusão

Interessante perceber que não há um consenso visual definido mesmo em grandes sites. Afinal, cada um preza por seguir seu estilo, mantendo uma uniformidade visual da paginação com o layout.

Todavia, analisando a maioria, é possível perceber que há um padrão básico a ser seguido:

* **página atual** (exibição)
* **próxima página** [botão]
* **página anterior** [botão]

_Detalhe: os botões **página anterior** e **próxima página**, ficam indisponíveis quando a página atual (selecionada) é a primeira ou a última, respectivamente._

Há também uma certa recorrência de um modelo mais avançado, onde são acrescidos os seguintes recursos:

* **primeira página** [botão]
* **última página** [botão]

Permitindo que o usuário seja direcionado mais rapidamente à página inicial ou final.

_Detalhe: perceba que os botões podem estar descritos por extenso: **primeira página** e **última página**, como referenciado acima; ou podem estar representados por números: sendo **1** a primeira e o número respectivo à última, exemplo: **17**._

Por último, menos recorrente, no entanto cabível em alguns sistemas, é possível perceber o uso de um recurso que mostra o total de registros em si (não somente as páginas) e onde o usuário está localizado.

* **Exibindo 1-30 de 650 registros**

_Volte nos exemplos do Booking e Gmail caso queira entender melhor._

Agora é com você! <br> Aproveite-se dos bons exemplos.

<br>

## Leituras complementares
---

* [Paginação: boas práticas de uso para uma experiência perfeita (ThiagoNasc.com)][1]{:target="_blank"}
* [Infinite Scrolling: When to Use It, When to Avoid It (NN Group)][10]
* [Alternatives to Pagination on Product-Listing Pages (NN Group)](https://www.nngroup.com/articles/alternatives-pagination-listing-pages/)
* [Infinite Scrolling Is Not for Every Website (NN Group)](https://www.nngroup.com/articles/infinite-scrolling/)
* [Split the Contents of a Website with the Pagination Design Pattern (Interaction Design)](https://www.interaction-design.org/literature/article/split-the-contents-of-a-website-with-the-pagination-design-pattern)

[1]: {% link _posts/2014-05-11-paginacao-boas-praticas-uso-experiencia-perfeita.md %}
[2]: http://instagram.com/
[3]: http://tiktok.com/
[4]: http://twitter.com/
[5]: http://youtube.com/
[6]: http://facebook.com/
[7]: http://linkedin.com/
[8]: http://reddit.com/

[9]: https://www.nngroup.com/
[10]: https://www.nngroup.com/articles/infinite-scrolling-tips/
[11]: https://pt.semrush.com/blog/top-100-sites-mais-visitados/

[12]: http://www.aliexpress.com
[13]: http://www.amazon.com.br
[14]: http://www.booking.com
[15]: http://www.gmail.com
[16]: http://www.google.com
[17]: http://www.americanas.com.br
[18]: http://www.magalu.com.br
[19]: http://www.mercadolivre.com.br
[20]: http://www.olx.com.br
[21]: http://www.shopee.com