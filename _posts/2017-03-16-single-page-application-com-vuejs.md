[![VueJS](http://blog.edgardleal.com/wp-content/uploads/sites/3/2017/03/VueJS_Logo-150x150.png)](http://blog.edgardleal.com/wp-content/uploads/sites/3/2017/03/VueJS_Logo.png) 

 VueJS é um framework Javascript reativo e é também conhecido como um framework progressivo, o que significa basicamente que você não vai precisar estudar toda a documentção do framework para começar a usar. Vamos ver um exemplo básico com o mínimo preciso para ter um código VueJS funcionando:  

<script async src="//jsfiddle.net/cohc4xdz/1/embed/js,html,result/"></script>
 
 Declaramos, na aba HTML, uma div simples com o _id_ de nossa aplicação e com o template _{{text}}_ que será substituido pelo valor da variável _text_.

1.  Na aba HTML importamos o código do framework do _cdnjs_
2.  Na aba Javascript criamos a instancia de nossa aplicação
3.  O parâmetro _el_ é onde deve ser inormado um QuerySelector indicando onde a aplicação será renderizada.
4.  E por fim o parâmetro _data_ que irá conter os valores utilizados em nossa aplicação, em nosso exemplo a variável _text_.

## VueJS para usuários de JQuery

O jQuery tem um objetivo diferente do VueJS e por isso não devem ser considerados concorrentes, e por terem paradigmas muito diferentes, é recomendado que não sejam utilizados no mesmo projeto. 

Enquanto o jQuery é uma ferramenta que tem como principal objetivo auxiliar na manipulação dirata do DOM ( HTML ) o VueJS se propoe a encapsular todo a manipulação do DOM. Neste momento surge a pergunta mais importante: 

*E como posso mudar a informação exibida na tela ?* 

O VueJS espera que seu desenvolvimento seja focado em manipular os dados e não o html, sendo assim, sempre que você lterar os valores do campo _data_ definido no setup de nossa aplicação o framework irá alterar automaticamente todos os pontos do html que fazem referencia a este valor. 

O objetivo é que você não precise mais se preocupar com a renderização de seus dados sobrando tempo para se dedicar aos pontos mais importantes de sua aplicação. 

Agora um exemplo demonstrando o framework fazendo este trabalho de "comunicação" dos dados da tela para o seu objeto e de seu objeto para a tela o que é conhecido como **Two Way Data Bind.** 

<script async src="//jsfiddle.net/edgardleal/z45bhc6m/1/embed/js,html,result/"></script>

No exemplo acima, sempre que o _iniput_ for alterado o texto dentro do _span_ será automaticamente alterado, mostrando a "reatividade" do framework.

#### Referencias:

[VueJS no GitHub](https://github.com/vuejs/vue)
