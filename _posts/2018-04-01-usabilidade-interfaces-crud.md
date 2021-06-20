---
layout: post
title: "Usabilidade em interfaces CRUD: o guia completo"
date: 2018-04-01 14:00:00.000000000 -03:00
type: post
published: true
status: publish
categories:
- Usabilidade
tags: [usabilidade]
img:
 url:	usabilidade-interfaces-crud.jpg
 alt:	"Imagem ilustrativa do título Usabilidade em interfaces CRUD"
---

Quem trabalha com desenvolvimento de sistemas está acostumado a lidar com **CRUD**! E por mais que esse acrônimo seja uma constante em nossas vidas, é comum vermos interfaces mal desenvolvidas por aí, comprometendo a experiência do usuário (UX) e consequentemente, o sucesso dos projetos.

## O que é CRUD?

Para quem não está familiarizado com o termo, segue sua definição:

> CRUD (acrônimo de Create, Read, Update e Delete na língua Inglesa) para as quatro operações básicas utilizadas em bases de dados relacionais (RDBMS) ou em interface para utilizadores para criação, consulta, atualização e destruição de dados. 

Fonte: [Wikipédia][1]{:target"_blank"}

Em linhas simples, as interfaces **CRUD** que lhe permitem cadastrar (create), visualizar (read), editar (update) e excluir (delete) registros de um sistema. Simples, não?

Seguem algumas dicas preciosas para o sucesso de sua interface:

## Cadastrar *(Create)*

### 1. Fácil acesso

Podemos considerar a funcionalidade 'Cadastrar' como a mais importante em uma interface CRUD, afinal, sem ela as demais não teriam utilidade.

**Botão de acesso à funcionalidade:** deve estar facilmente visível e acessível, sem a necessidade de usar a barra de rolagem.

![Exemplo de interface não recomendada, com a necessidade de rolar a página para acessar o botão cadastrar e exemplo de interface recomendada, onde o botão fica disponível sem rolar a página](/assets/imgs/usabilidade-interfaces-crud/crud-1.jpg){:.img-fluid.rounded}

**Interfaces/telas longas:** aproveite-se de recursos como (1) disponibilizar um botão no início e outro ao final da página, (2) utilizar botão fixo ao rolar a página e/ou (3) utilizar atalho 'voltar ao topo' para facilitar o uso;

### 2. Página ou modal: qual utilizar?

Entende-se como **página** quando a interface por inteira é alterada e **modal** quando uma janela sobrepõe a página já aberta, na maioria das vezes preenchendo parcialmente a tela do usuário.

Formulários complexos e com muitos campos demandam uma alta concentração do usuário, isto implica que sua atenção não deva ser desviada e a utilização de páginas se mostram mais eficazes.

Formulários simples e com poucos campos demandam menos concentração e tem seu uso de forma rápida, tornando a utilização de janelas (modal) mais recomenda, visto sua melhor fluidez e intuitividade.

Importante salientar que não existe uma regra ou fórmula que defina a melhor utilização. Aproveite-se de recursos como a prototipação, testes e feedbacks dos usuários a fim de entender e aplicar a melhor estratégia ao seu cenário!

* **Formulários grandes e complexos:** prefira a utilização de páginas;
* **Formulários curtos e simples:** prefira a utilização de modal.

![Exemplo de interface não recomendada onde o formulário simples ocupa somente parte da página e exemplo de interface recomendada, utilizando uma modal](/assets/imgs/usabilidade-interfaces-crud/crud-2.jpg){:.img-fluid.rounded}

### 3. Formulários grandes e/ou muito complexos

Para formulários grandes ou muito complexos a utilização de técnicas que facilitem a experiência do usuário é fundamental para o sucesso do projeto. Afinal, perder os dados depois de preencher um a um com toda a atenção é de rancar os cabelos. Quem nunca?

**Divida o formulário em etapas:** categorize e distribua os campos de forma lógica e compreensível;

**Torne claro seu posicionamento e progressão:** o usuário deve entender onde está e onde precisa chegar para finalizar o processo;

![Exemplo de interface não recomendada, com formulário longo em única página e exemplo de interface recomendada, com várias etapas contendo formulários menores e indicação da progressão através de um indicador de etapas](/assets/imgs/usabilidade-interfaces-crud/crud-3.jpg){:.img-fluid.rounded}

**Permita o usuário salvar sua progressão:** funcionalidades de 'rascunho' permitem o usuário salvar sua progressão e finalizá-la mais tarde, item imprescindível a formulários que demandam muito tempo do usuário (isto pode salvá-lo de diversas situações, inclusive perda de informação por falta de internet);

**Garanta o bom funcionamento das teclas de atalho:** atendendo a heurística flexibilidade e eficiência de uso, devemos prover atalhos - despercebidos a usuários novatos - que podem acelerar e facilitar a interação aos usuários especialistas, de modo que o sistema atenda bem a ambos. Garanta a aplicação dos seguintes recursos:
* Ordenação dos campos através do atributo <code>tabindex</code> (HTML);
* <code>Tab</code> redireciona ao próximo campo;
* <code>Shift + Tab</code> retorna ao campo anterior;
* <code>Enter</code> no botão de submissão executa a ação.

### 4. Permita cancelar a ação a qualquer momento

Atendendo a heurística 'liberdade e controle do usuário', devemos permitir o cancelamento do cadastro com a mesma - ou quase - facilidade de entrada, muitas vezes o usuário entra em determinada ação por engano ou simplesmente desiste no meio do processo.

**Confirmação de cancelamento:** disponha da funcionalidade para evitar cancelamentos indevidos. Sugestão de mensagem: "Você tem certeza que deseja cancelar o cadastro?"

![Exemplo de interface recomendada com funcionalidade de confirmação de cancelamento de cadastro](/assets/imgs/usabilidade-interfaces-crud/crud-4.jpg){:.img-fluid.rounded}

## Visualizar *(Read)*

### 1. Listagem de registros

A mais tradicional 'página de entrada' de um CRUD é sua listagem de registros.

**Título da página:** deve estar visível sem a necessidade de usar a barra de rolagem. Utilize títulos simples e sem redundância. Exemplo: "Listagem de membros" ao invés de "Listagem de membros cadastrados no sistema".

**O vazio nunca deve estar vazio:** caso não haja dado cadastrado, exiba uma mensagem informativa no grid como: "Não há registros a serem exibidos".

![Exemplo de interface não recomendada, onde a página não exibe nenhuma informação após o botão de cadastro e interface recomendada, onde após o botão, há a informação de que não há registros a serem exibidos](/assets/imgs/usabilidade-interfaces-crud/crud-5.jpg){:.img-fluid.rounded}

**Limite-se aos dados mais importantes no grid:** disponha somente os dados relevantes ao usuário e que melhor identifiquem os registros, os demais devem estar disponíveis na visualização dos detalhes. Uma interessante tática é dispor inicialmente o mínimo de dados possível e à medida do uso, verificar a necessidade de mais dados;

**Sintetize os dados presentes no grid:** aproveite-se de ícones, cores, abreviações e outros recursos para dispor informações relevantes;

**Aproveite-se da resolução:** telas maiores permitem a exibição de mais dados. Permita-se utilizar dados que aparecem somente em telas maiores e esconda-os em telas menores (interfaces responsivas).

![Exemplo de interface não recomendada, sem fim e com diversos registros na tela, ao lado do exemplo de interface recomendada, com poucos registros no grid e logo abaixo a paginação.](/assets/imgs/usabilidade-interfaces-crud/crud-6.jpg){:.img-fluid.rounded}

**Ordene os dados:** verifique a melhor aplicabilidade ao tipo de registro e disponibilize-o inicialmente já ordenado, ainda que possa variar dependendo do tipo de dado, podendo ser:
* **Alfabética:** nomes;
* **Numérica:** ids e códigos
* **Cronológica:** data de cadastro e edição.
 
**Divida os registros em páginas:** utilizar recursos de paginação evita páginas extensas, de difícil carregamento e organização. Garanta a aplicação dos seguintes recursos:

* Destacar a página qual o usuário encontra-se;
* Mostrar o quantitativo total de páginas;
* Facilite o acesso à primeira e última página;

![Exemplo de 3 interfaces, a primeira de um tablet, onde o grid exibe 3 colunas, a segunda de um browser de resolução superior ao tablet, exibindo 1 coluna a mais e por fim, um browser com resolução superior à anterior, exibindo 3 colunas a mais que o tablet](/assets/imgs/usabilidade-interfaces-crud/crud-7.jpg){:.img-fluid.rounded}

**Quantitativo total de registros:** dado de extremo valor, simples de ser coletado e muitas vezes esquecido de ser disponibilizado ao usuário. Disponha a informação ao final da listagem. Exemplo: Total de 105 registros. O termo 'registro' é genérico o suficiente para ser utilizado na maioria dos casos.

### 2. Ferramentas de filtro e pesquisa

Filtrar e pesquisar, ainda que similares, tem comportamentos diferentes e é importante termos este conhecimento:

**Filtro:** considera-se no estado inicial todos os registros presentes no sistema e os removem de acordo com os critérios selecionados.

**Pesquisa:** considera-se no estado inicial vazio (nenhum registro) e exibe os registros de acordo com os critérios selecionados.

## Editar *(Update)*

As boas práticas de cadastro devem ser reaproveitadas na edição, portanto, a página pode ser reutilizada, com a diferença que os dados virão inicialmente já preenchidos, permitindo sua edição.

**Campos não-editáveis devem vir bloqueados:** mantenha-os visíveis porém não editáveis (bloquados). Quando necessário, explique ao usuário o motivo da impossibilidade de alteração.

## Excluir *(Delete)*

Conforme visto no artigo [Usabilidade: Usabilidade: excluir, deletar, apagar, remover ou cancelar?][2], podemos dar o nome a esta ação de várias maneiras. Aplique o que considerar mais adequado e lembre-se de seguir o padrão para todas as páginas!

Prefiro e recomendo sempre utilizar o termo: **excluir**.

**Mensagem de alerta e ação de confirmação:** visto a exclusão ser geralmente irreversível, é fundamental que o usuário seja alertado e possua uma ação para confirmação. Exemplo: Tem certeza que deseja exluir o registro definitivamente?

![Exemplo de interface recomendada com funcionalidade de confirmação de exclusão de registro](/assets/imgs/usabilidade-interfaces-crud/crud-8.jpg){:.img-fluid.rounded}

**Mensagens de feedback:** é fundamental informar o usuário após a conclusão da ação. Aproveite-se, quando necessário, da mensagem de feedback para possibilitar ao usuário desfazer a ação, ainda que o sistema tenha informado ser um processo irreversível. Esse recurso 'extra' pode ser extramente útil a vários casos!

![Exemplo de interface recomendada com feedback após a exclusão, informando o usuário que o procedimento foi realizado e uma funcionalidade extra, possibilitando o usuário desfazer o processo](/assets/imgs/usabilidade-interfaces-crud/crud-9.jpg){:.img-fluid.rounded}

*Este artigo é atualizado frequentemente para inserção de novas dicas.*

E você, quais outras boas práticas de usabilidade aplica em sistemas CRUD's?
<br>Compartilhe com a gente!

[1]: https://pt.wikipedia.org/wiki/CRUD
[2]: http://thiagonasc.com/usabilidade/usabilidade-excluir-deletar-apagar-remover-ou-cancelar