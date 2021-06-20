---
layout: post
title: A importância dos protótipos no desenvolvimento de sistemas
date: 2013-11-13 21:17:43.000000000 -02:00
type: post
published: true
status: publish
categories:
- desenvolvimento-web
# Usabilidade
tags:
- interface
- prototipação
- ui
- ux
img:
 url:	prototipo-wireframe.jpg
 alt:	Papel com protótipo feito à mão, desenho de um calendário
---

#### O protótipo é a forma mais rápida e econômica de se definir e experimentar um projeto. Esses dois motivos por si só já garantem sua importância, porém, ainda assim é comum vermos sistemas tomando forma antes de qualquer rascunho.

Por mais que o levantamento de requisitos por si só levante uma infinidade de informações que deverão estar dispostas na interface, é durante a interação real do usuário com o sistema que os detalhes realmente são percebidos. Para projetar a experiência perfeita, a utilização de protótipos se faz a forma mais eficaz de simular essa interação, devendo ser feita ainda no período de concepção do sistema, evitando gastos dispendiosos de tempo e monetários.

![wireframe exemplo](/assets/imgs/wireframe-example.jpg){:.img-fluid.rounded}

Muitos desenvolvedores indagam a questão de começar o projeto pela parte visual e não a funcional. Pois bem, temos a interface como o principal canal de comunicação entre o sistema e o usuário, e é sua função oferecer a melhor experiência. Em outras linhas, a interface deve entregar ao usuário uma mensagem clara e objetiva a fim de atender suas necessidades sem criar dúvidas (cenário ideal). A interface portanto deve ser tratada desde o primeiro minuto de concepção de um software. Será ela quem define e exprime a interação do sistema com o usuário ou vice-versa, portanto a programação deve seguir o visual e não o visual seguir a programação.

"As maiores melhorias na interface de um produto são obtidas através da recolha de dados de usabilidade nas fases inicias de seu desenvolvimento." <em>Jakob Nielsen, 2013</em>

Quanto mais avançado o projeto está, maiores são os impactos para se realizar correções ou alterações em seu código. É fácil imaginar: alterar a programação de uma determinada funcionalidade em um sistema demanda mais tempo que refazer seu rascunho várias vezes. O tempo gasto portanto na prototipação é inversamente proporcional ao tempo necessário para a programação, em outras linhas, quanto mais se dedicar na fase de prototipação, menor será o gasto de sua implementação.

## Vantagens:

* baixa demanda de tempo para desenvolvimento e consequentemente, baixo custo
* não requer conhecimentos avançados em softwares de edição gráfica
* facilita a visualização do produto para o cliente desde a fase inicial
* possibilita receber o feedback do cliente em tempo ágil
* facilita o levantamento de requisitos e funcionalidades
* possibilita estimar de forma mais precisa a complexidade e tempo de desenvolvimento
* possibilita a realização testes de interações
* reduz os esforços de desenvolvimento

## Classificações

### Protótipos de Baixa Fidelidade:

Os protótipos de baixa fidelidade, também chamados de rascunhos ou sketches, são concebidos ainda na fase inicial, durante a concepção do sistema.

Desenhados geralmente à mão utilizando lápis, borracha e papel, essas representações são feitas de maneira rápida e superficial, apenas margeando a ideia do projeto e definindo superficialmente sua interação com o usuário, não se preocupando ainda com elementos de layout, cores, disposições, etc.

![prototipo de baixa fidelidade](/assets/imgs/prototipo-baixa_fidelidade.jpg){:.img-fluid.rounded}

Essa etapa é fundamental para a definição do produto e levantamento de requisitos.

### Protótipos de Média Fidelidade:

Conhecidos também por wireframes, esse protótipos são desenvolvidos na fase da arquitetura da informação.

Utilizando lápis e papel ou softwares de prototipação, como o Balsamiq ou Axure, esses documentos apresentam a estrutura e o conteúdo da interface, definindo peso, relevância e relação dos elementos, formando o layout básico do projeto.

![prototipo de media fidelidade](/assets/imgs/prototipo-media_fidelidade.jpg){:.img-fluid.rounded}

Os protótipos de média fidelidade ainda não utilizam recursos gráficos avançados como cores ou fotografias.

### Protótipos de Alta Fidelidade:

Os mockups ou protótipos funcionais constituem a representação mais próxima do sistema a ser desenvolvido. Em alguns casos, é possível simular o fluxo completo das funcionalidades, permitindo a interação do usuário como se fosse o produto final.

A aparência visual, as formas de navegação e interatividade já são concebidas e aplicadas aos protótipos de alta fidelidade.

![prototipo-alta_fidelidade](/assets/imgs/prototipo-alta_fidelidade.jpg){:.img-fluid.rounded}

Seu desenvolvimento é realizado na fase final de definição da interface, utilizando programas de design gráfico, como o Photoshop ou Fireworks; ferramentas de codificação front-end, como o Sublime Text ou Dreamweaver; e linguagens de programação front-end, como o HTML + CSS + jQuery.

Obs: não há uma convenção formada sobre os nomes e definições, há quem chame um mockup de wireframe, um wireframe de sketch, ou vice-versa, há também quem diga que um wireframe obrigatoriamente tem de ser feito à mão, há quem diga que não. Enfim, você irá encontrar definições de todo tipo pela internet, mas no final, todos são protótipos e o importante é que desempenhem suas funções e lhe traga benefícios. Então use aqueles que lhe for mais conveniente e os chame como preferir.

## Metodologias

Enquanto desenvolvemos os protótipos é comum surgir a dúvida: devo aprimorá-los até o último momento e ir programando de acordo com sua evolução, ou devo em determinado instante dá-los como finalizados e só então iniciar o desenvolvimento? A resposta é: os dois casos podem ser aplicados com êxito, fica à sua escolha.

**Prototipação Evolucionária:** consiste em produzir um modelo inicial e refiná-lo ao longo das várias fases de desenvolvimento até atingir a forma final.

**Prototipação Descartável:** implementados em cada etapa do projeto, esses modelos abordam os detalhes do ciclo e depois são descartados. Para esse tipo de uso, descartável, é fundamental saber o momento certo de considerar o protótipo como finalizado.

![exemplo prototipo iphone mobile](/assets/imgs/prototipo-iphone.jpg){:.img-fluid.rounded}

## Conclusão

Há diversas metodologias e formas de se iniciar o desenvolvimento de um sistema, independentemente da escolha, a etapa de prototipação se faz fundamental para o sucesso do projeto, otimizando o tempo e reduzindo o esforço de desenvolvimento.

É mais barato alterar um produto na sua fase inicial do que fazer alterações em um produto acabado. Estima-se que seja 100x (cem vezes) mais barato efetuar alterações antes de se começar a programar do que esperar que todo o desenvolvimento tenha sido efetuado." <em>Jakob Nielsen, 2013</em>

## Referências

* PRESSMAN, Roger S. Software Engineering: a Practitioner's Approach. 6. ed. McGraw-Hill, 2005
* <a href="http://en.wikipedia.org/wiki/Software_prototyping" target="_blank">Prototyping, Wikipédia</a>
* <a href="http://pt.wikipedia.org/wiki/Prototipa%C3%A7%C3%A3o" target="_blank">Prototipação, Wikipédia</a>
* <a href="http://disciplinas.lia.ufc.br/es062/arquivos/Captulo_8-Prototipacao.pdf" target="_blank">Prototipação de software - Engenharia de Software (UNESP)</a>
* <a href="http://dinobrasilis.pro.br/mod_inic_1.pdf" target="_blank">Modelos de Desenvolvimento de Software (Dino Brasilis)</a>