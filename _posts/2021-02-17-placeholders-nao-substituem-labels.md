---
layout: post
title: 'Usabilidade em formulários: placeholders não substituem labels'
date: 2021-02-20 19:42:00
type: post
published: true
status: publish
categories:
- Usabilidade
---

#### Lançado através do HTML5 em 2014, o atributo *placeholder* veio para facilitar o preenchimento de formulários, no entanto, quando utilizado em substituição ao *label*, pode provocar sérios problemas na experiência do usuário como a redução da acessibilidade e usabilidade.

## Diferenciando o *placeholder* de um *label* em formulários

![Livro Trabalhe 4 Horas por semana erguido por uma mão](/assets/imgs/placeholder/placeholders-e-labels-demonstracao.jpg){:.img-fluid.rounded}

***Label**: [elemento]* representa o rótulo ou etiqueta, como em sua tradução literal, de um determinado campo na interface.

***Placeholder**: [atributo]* representa uma dica rápida (uma palavra ou uma frase curta) com objetivo de auxiliar o usuário no preenchimento do campo enquanto o mesmo ainda está vazio.

Perceba que o ***placeholder*** é um atributo que deixa de aparecer quando o campo é preenchido, diferentemente do ***label*** que permanece visível a todo momento na interface.

Esse detalhe por si só é suficiente para entendermos que **placeholders não substituem labels**. Ainda assim, segue um bom exemplo para consolidarmos o entendimento:

## Sentindo com a ausência de ***labels*** na prática

Imagine você se deparando com a seguinte interface:

![DESCRICAO](/assets/imgs/placeholder/formulario-sem-labels.jpg){:.img-fluid.rounded}

**Pergunta:** o <ins>telefone comercial</ins> a ser atualizado se refere à qual dos campos na imagem acima?

<span style="color:gray; background-color: #eee;">_[ retorne sua atenção à imagem e pense na resposta ]_</span>

Você provavelmente está em dúvida entre os 2 últimos campos, correto?

<span style="color:gray; background-color: #eee;">_[ retorne novamente à imagem e decida ]_</span>

Acredito que a maioria de nós atualizaríamos o 3º ou 4º campo em razão de seus preenchimentos com números no formato de telefones.

Podemos ainda estar mais suscetíveis a atualizar o 3º campo ao invés do 4º em razão de seus números sugerirem mais um telefone fixo (comercial), que um telefone móvel (celular pessoal) como no último campo. Concorda?

No entanto, o mais interessante dessa experiência é perceber que uma interface na ausência de labels, ainda que conte com placeholders, pode nos trazer grandes problemas na experiência do usuário.

Para nos certificarmos disso, temos abaixo o formulário codificado e funcional seguindo a mesma estrutura: sem labels, com placeholders e um preenchimento inicial já realizado, aguardando pela alteração do telefone comercial.

Para que você sinta essa experiência, tente atualizar o telefone comercial e clique em atualizar, quando o preenchimento estiver correto você será alertado:

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>

<script>
$(document).ready(function(){
  $("form").submit(function(){
    alert("Parabéns, sabemos que não foi fácil (rs) mas você conseguiu atualizar os dados! =)");
  });
});
</script>

<style>
input {
	font-size: 14pt;
	width: 98%;
	margin:4px 0;
	border-radius: 4px;
	padding: 4px;
	border: 1px solid #555;
}
</style>

<div markdown="1" style="background-color:#eee;">
<form style="width: 50%; margin-left:auto; margin-right: auto; padding-top:40px; padding-bottom:50px;">
	<p>
		<span style="font-size:24pt; font-weight: bold;">Atualizar dados</span><br>
		<small style="color:red"><b>Atenção:</b> devido à mudanças na política de uso, seu <ins>telefone comercial</ins> precisa ser atualizado:</small>
	</p>
	<input type="tel" placeholder="Telefone comercial" value="Thiago Nascimento" pattern="\([0-9]{2}\) [0-9]{4,6}-[0-9]{3,4}$" required>
	<br>
	<input type="tel" placeholder="Telefone residencial" value="http://www.thiagonasc.com" pattern="\([0-9]{2}\) [0-9]{4,6}-[0-9]{3,4}$" required>
	<br>
	<input type="text" placeholder="CNPJ" value="(35) 3265-5623" pattern="[0-9]{2}\.?[0-9]{3}\.?[0-9]{3}\/?[0-9]{4}\-?[0-9]{2}">
	<br>
	<input type="url" placeholder="Site" value="(35) 9999-1020">
	<br>
	<small style="font-size: 11pt">Telefones deverão seguir o formato: (xx) xxxx-xxxx</small>
	<br>
	<input type="submit" value="Atualizar" style="width: 50%; background-color: #9eb9d4;">
</form>
</div>

<br>

Perceba que somente ao apagar os valores já preenchidos em cada campo você terá acesso ao _placeholder_ (afinal, esta é sua natureza) e por consequência identificará o que cada item realmente representa. Deveria ser bem mais fácil, concorda?

E como no exemplo, podemos encontrar valores já preenchidos que não coincidem com a realidade do campo e ainda assim, passarmos desapercebidos pela situação.

### E o problema vai além...

O uso de ***placeholders*** em substituição aos ***labels*** também reduzem significativamente a acessibilidade e usabilidade de interfaces à uma gama de usuários que dependem de recursos e facilidades para sua interação.

Alguns exemplos clássicos:

* leitores de telas varrerão a interface informando os dados já preenchidos em cada campo sem a orientação real ao que o campo se refere (incorrendo num problema muito similar ao exemplo citado anteriormente);
* ***placeholders*** são exibidos em cinza claro, por padrão, fornecendo contraste insuficiente a muitos usuários com baixa sensibilidade ou acuidade visual;
* a falta de ***labels*** diminui o espaçamento entre os campos, reduz as áreas de clique e por consequência, dificultam os acessos aos campos corretos.

Há um artigo da *Smashing Magazine* que defende a **não utilização** do ***placeholder*** e explica os motivos em detalhes ([acessar artigo](https://www.smashingmagazine.com/2018/06/placeholder-attribute/){:target="_blank"}).

## Quero simplificar e usar somente um!

Atualmente, por razões estéticas e até minimalistas, é muito comum ver interfaces utilizando somente um desses recursos.

No entanto, é importante salientar que se utilizando das boas práticas, você verá majoritariamente o ***label*** na interface, ainda que em certos momentos ele se pareça muito com um ***placeholder***.

O recurso é utilizado de forma que o ***label*** assuma inicialmente a posição do ***placeholder***, isto é, estará posicionado dentro do campo até o momento em que o mesmo esteja em foco ou receba algum valor. Neste caso, o ***label*** sobe à sua posição original.

Veja que o Google utiliza desse recurso em seu Material Design:

<div markdown="1" style="text-align:center">
![DESCRICAO](/assets/imgs/placeholder/placeholder-label-google.gif)
</div>

<br>
É uma forma digamos híbrida de aproveitar a simplicidade em utilizar um único elemento, a facilidade de uso enquanto a orientação vem no mesmo local onde se preenche e a consistência em se manter a identificação do campo visível a todo momento.

## Conclusão

***Placeholders*** e ***labels*** possuem objetivos diferentes mas complementares e portanto, um não substitui o outro. Sempre que possível, aproveite dos benefícios de ambos em sua interface e caso opte em utilizar somente um, dê preferência ao ***label***.

## Referências e leituras complementares

* [W3C Recommendation - HTML 5.2](https://www.w3.org/TR/html52/sec-forms.html#the-placeholder-attribute){:target="_blank"}
* [SmashingMagazine - Don’t Use The Placeholder Attribute](https://www.smashingmagazine.com/2018/06/placeholder-attribute/){:target="_blank"}
* [CSS Tricks - Placeholder Shown](https://css-tricks.com/almanac/selectors/p/placeholder-shown/){:target="_blank"}
