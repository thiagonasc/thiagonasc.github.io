---
layout: post
title: 'Confirmar senha: necessário ou inútil?'
description: 'Utilizar ou não o campo de confirmação de senha em minhas interfaces? Publicado por Thiago Nascimento.'
date: 2021-01-24 18:50:00
type: post
published: true
status: publish
categories:
- Usabilidade
---

#### O objetivo essencial do campo **confirmar senha**, utilizado massivamente em formulários de cadastro e redefinição de senha, é garantir que o usuário tenha informado a senha correta evitando problemas em seu acesso.

![Livro Trabalhe 4 Horas por semana erguido por uma mão](/assets/imgs/confirmar-senha/form-confirmar-senha.jpg){:.img-fluid.rounded}

Isso acontece principalmente pelo fato do campo **senha** ser mascarado, isto é, mostrar asteriscos (ou bullets) ao invés dos caracteres reais enquanto o usuário digita.

O campo **confirmar senha** serve portanto como um validador, no entanto, há dois aspectos importantes a serem considerados:

### 1. É possível confirmar uma senha diferente da esperada:

O campo **confirmar senha** minimiza porém não extingue a possibilidade do usuário inserir uma senha com caracteres diferentes do esperado, **o que não resolve o problema**.

Parece estranho à primeira vista mas é fácil entender: com sistemas nos pedindo senhas cada vez mais seguras, combinadno letras, números e caracteres especiais, podemos digitar algo seguindo uma lógica e repeti-la sem perceber que algo foi digitado errado. Fato comum principalmente em celulares onde muitas vezes maiúsculas e minúsculas se alternam no teclado sem percebermos ou mesmo alguma alteração feita pelo próprio corretor ortográfico.

![Livro Trabalhe 4 Horas por semana erguido por uma mão](/assets/imgs/confirmar-senha/form-confirmar-senha-maiusculas.jpg){:.img-fluid.rounded}

_Obs: é comum também vermos formulários que permitem o usuário utilizar comandos de colar (ctrl+v) no campo de confirmação de senha. O que o torna <strike>incoerente</strike> ineficiente, visto que submeter o usuário digitar novamente a senha é ação essencial do campo e parte fundamental da validação._

### 2. Quanto mais trabalhoso um formulário, maior as chances de abondono:

Um campo adicional de **confirmar senha** aumenta a complexidade do formulário, o trabalho do usuário e consequentemente suas chances de abandonar o processo.

Sem cadastro, sem senha, sem conversão. **O que não melhora o problema**.

## Solução proposta

A opção mais defendida por especialistas e também oportunamente mais simples é: **remover o campo confirmar senha** e **adicionar a funcionalidade mostrar senha** no campo primário (senha).

![Livro Trabalhe 4 Horas por semana erguido por uma mão](/assets/imgs/confirmar-senha/form-confirmar-senha-solucao.jpg){:.img-fluid.rounded}

Algo curioso neste estudo foi perceber que mascarar senhas mais prejudica a usabilidade que necessariamente aumenta a segurança.

> "Mascarar senhas se tornou comum por nenhuma razão além de ser fácil de fazer e também por ser o padrão no início da web. (...) Vamos limpar as teias de aranha da Web e remover coisas que estão lá apenas porque sempre estiveram lá". (Jakob Nielsen)

Em minha visão, não significa que o campo de senha deva vir originalmente sem máscara mas possibilitar que seja feito. Dessa maneira, a funcionalidade **mostrar senha** atende perfeitamente!

Importante considerar que tratando de interações humanas, sempre teremos exceções e com isso, muitas vezes não há certo ou errado mas sim diferentes opções e contextos. Ainda assim, precisamos manter em mente que sempre haverá uma forma mais efetiva de se utilizar ou no mínimo, mais simples de se desenvolver.

### Exemplo ou exceção?

Lendo sobre o tema e seus comentários me surgiu um pensamento interessante:

Imaginem um usuário que esteja demonstrando seu cadastro à um grande público e após digitar a senha ficou em dúvida se a informou corretamente. A funcionalidade **mostrar senha** não seria considerada visto que exporia seus dados. No entanto a funcionalidade **confirmar senha** lhe seria útil uma vez que informaria novamente e o sistema a validaria com sua primeira inserção.

Surgiria então uma possibilidade híbrida: por que não manter as opções de **confirmar senha** e **mostrar senha**, possibilitando que o usuário escolha o melhor pra si?

Neste caso, por razões de usabilidade, ao escolher **mostrar senha**, a funcionalidade de **confirmar senha** seria ocultada ao passo que ao **ocultar senha**, a funcionalidade **confirmar senha** seria re-exibida. Uma opção aplicável, no entanto, menos convencional e mais complexa em seu desenvolvimento e uso.

Gostaria de repetir o exemplo, no entanto, pedindo que você se coloque na posição do usuário. Imagine portanto você preenchendo um formulário de cadastro com várias pessoas lhe assistindo e ao digitar a senha você se indaga: digitei corretamente? Qual seria sua reação? Apagar o que foi informado e redigitar com mais calma e atenção ou aproveitar do campo de confirmação de senha para validar a primeira inserção? Isso ainda sem considerar que provavelmente o formulário terá diversos outros campos a serem preenchidos antes de avançar.

Sendo assim, desconsideremos o formato híbrido como uma boa opção.

## Conclusão

Podemos dizer que o campo **confirmar senha** não é de todo inútil, no entanto, formulários podem ser mais efetivos sem sua utilização considerando a adição da funcionalidade **mostrar senha** no campo primário (senha).

*Concorda ou discorda de algum ponto do artigo? Contribua!<br>
Ficarei honrado em receber seu comentário!.*

## Referências e leituras complementares

* [Stop Password Masking (Nielsen Norman Group)](https://www.nngroup.com/articles/stop-password-masking/){:target="_blank"}
* [Why the confirm password field must die (UX Movement)](https://uxmovement.com/forms/why-the-confirm-password-field-must-die/){:target="_blank"}
* [How to stop passwords causing users to abandon your form (Zuko)](https://www.zuko.io/blog/password-advice-for-online-forms){:target="_blank"}