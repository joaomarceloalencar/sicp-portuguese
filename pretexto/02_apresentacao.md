# Apresentação

Eu tive o prazer de conhecer o espetacular Alan Perlis e conversar com ele algumas vezes, enquanto ainda era um estudante. Ele e eu tínhamos em comum um profundo amor e respeito por duas linguagens de programação bastante diferentes: _Lisp_ e APL. Seguir seus passos é uma tarefa assustadora, apesar dele ter deixado uma trilha excelente. Ainda assim, eu gostaria de examinar novamente um comentário que ele fez na apresentação original deste livro (e, por favor, eu sugiro que leia a apresentação dele, que está logo em seguida, antes de terminar esta). É realmente verdade que é melhor ter 100 funções atuando em única uma estrutura de dados do que ter 10 funções operando em 10 estruturas de dados?

Para responder essa questão com cuidado, primeiro devemos nos perguntar se a tal única estrutura de dados é "universal": pode ela, de maneira conveniente, cumprir o papel das outras 10 estruturas de dados mais especializadas?

No mesmo contexto, também podemos perguntar: realmente precisamos de 100 funções? Há uma única função universal que pode cumprir o papel de todas as outras funções?

A surpreende resposta para a última questão é **sim**; é apenas um pouco complicado construir uma função que receba (1) uma estrutura de dados que serve como descrição de alguma outra função e (2) uma lista de argumentos, e se comporta exatamente como essa outra função ao receber os mesmos argumentos. E também é apenas um pouco complicado projetar uma estrutura de dados capaz de descrever qualquer computação. Uma estrutura como essa (a representação em lista rotulada de expressões e sentenças, unida a um ambiente que associa nomes a valores) e uma função universal (aplicar) são descritas no Capítulo 04 deste livro. Então talvez precisamos apenas de uma função e uma estrutura de dados. _Nota do tradutor: o nome da estrutura em inglês é taggeg\_list e a função é apply. Talvez lá na frente não traduza esses termos._

Esta é a verdade na teoria. Na prática, encontramos conveniência ao delinear distinções que nos ajudam, como seres humanos criando descrições de computações, a organizar o formato de nosso código para facilitar sua compreensão. Eu acredito que Perlis estava fazendo uma afirmação não sobre capacidade computacional, mas sobre habilidades e limitações humanas.

Uma coisa que a mente humana parece fazer bem é nomear coisas; nós temos memórias associativas poderosas. Dado um nome, conseguimos rapidamente se lembrar de alguma coisa associada a ele. É por isso que geralmente achamos mais fácil trabalhar com o cálculo _lambda_ do que com o cálculo combinatório; é muito mais fácil para a maioria das pessoas interpretar a seguinte expressão _Lisp_ 

`(lambda(x)(lambda(y)(+ x y)))`

ou a expressão _JavaScript_

`x => y => x + y`

do que a expressão combinatória

`((S ((S (K S)) ((S ((S (K S)) ((S (K K)) (K +)))) ((S (K K)) I)))) (K I))` 

apesar de existir uma correspondência estrutural direta, facilmente expressa em algumas poucas linhas de código _Lisp_.

Então apesar de a princípio uma única função universal ser suficiente, preferimos modularizar o nosso código, nomear as diferentes partes e mencionar o nome das descrições de funções no lugar de repetidamente fornecer as descrições para uma função universal. 

Na minha palestra de 1998 chamada "Crescendo uma Linguagem", comentei que um bom programado "não apenas escreve programas. Um bom programador constrói um vocabulário funcional." A medida que projetamos e definimos mais e mais partes dos nossos programas, nomeamos essas partes e o resultado é que temos uma linguagem mais rica, na qual escrevemos o resto. 

Mas também achamos natural delinear distinções entre estruturas de dados e nomeá-las. 

Pode ocorrer de que listas aninhadas são uma estrutura de dados universal (e vale notar que muitas estruturas de dados modernas e amplamente utilizadas, como HTML, XML e JSON, são estruturas aninhadas entre parênteses, somente um pouco mais elaboradas do que os parênteses básicos de _Lisp_). Também há várias funções, tal como determinar o tamanho de uma lista ou aplicar uma função a cada elemento de uma lista e recuperar uma lista dos resultados, que são úteis em uma variedade de situações. Mas mesmo, quando estou pensando em uma computação específica, geralmente falo para comigo mesmo, "Esta lista de duas coisas considero como o primeiro nome e o sobrenome, mas aquela lista de duas coisas considero que são a parte real e imaginária de um número complexo, e aquela outra lista de duas coisas considero o numerador e o denominador de uma fração." Em outras palavras, eu descrevo distinções - e pode ser útil representar tais distinções de maneira explícita na estrutura de dados, em parte para prevenir erros como acidentalmente tratar um número complexo como uma fração. (Novamente, este é um comentário sobre habilidades e limitações humanas.)

Desde que a primeira edição deste livro foi escrita, quase quatro décadas atrás, muito mais maneiras de organizar dados se tornaram relativamente padrozinadas, em particular a abordagem "orientada a objetos", e muitas linguagens, incluindo _JavaScript_, suportam estruturas de dados especializadas como objetos, cadeias de caracteres, monte (_heap_), pilhas e mapeamentos com uma variedade de mecanismos embutidos e bibliotecas. Mas ao fazer isso, muitas linguagens abandoram o suporte para noções mais gerais e universais. _Java_, por exemplo, originalmente não suportava funções de primeira classe e as incorporou apenas recentemente, aumentando em muito seu poder de expressão.

APL, da mesma forma, originalmente não suportava funções de primeira classe e sua única estrutura de dados inicial - _arrays_ de qualquer número de dimensões - não era tão útil como uma estrutura universal porque _arrays_ não podiam conter outros _arrays_ como elementos. Versões mais recentes da APL suportam valores de função anônimos e _arrays_ aninhados e estas adições tornaram API dramaticamente mais expressiva. (O projeto inicial da APL tinha sim duas boas decisões a seu favor: um conjunto abrangente de funções aplicáveis para a única estrutura de dados e um conjunto de nomes para essas funções bem definido. Não estou falando dos símbolos engraçados e letras gregas, mas das palavras faladas que programadores APL usam quando os referenciam, palavras como _shape_, _reshape_, _compress_, _expand_ e _laminate_; estes são nomes não para os símbolos, mas para as funções que representam. Ken Iverson tinha um grande talento para escolher nomes cursos, fáceis de lembrar e vívidos para funções em _arrays_.) _Nota do tradutor: preferi por não traduzir as funções do APL, até porque não devem retornar a aparecer no resto do livro._

Enquanto _JavaScript_, como _Java_, foi originalmente projetada com objetos e métodos em mente, também incorporou funções de primeira classe desde o ínicio e agora não é difícil usar seus objetos para definir uma estrutura de dados universal. Como resultado, _JavaScript_ não é tão distante de _Lisp_ quanto você pensa e como esta nova edição demonstra, é um bom _framework_ alternativo para apresentar as ideias chave. Este livro nunca foi pensando como um livro sobre uma linguagem de programação; ele apresenta ideias gerais e poderosas para organização de programas que podem ser úteis em qualquer linguagem.

O que _Lisp_ e _JavaScript_ tem em comum? A habilidade de abstrair uma computação (código mais alguns dados associados) para posterior execução como uma função; a habilidade de embarcar referências a tais funções dentro de estruturas de dados; a habilidade de invocar funções em argumentos; a habilidade de delinear uma distinção (execução condicional); uma estrutura de dados universal conveniente; gestão totalmente automática de armazenamento para os dados (o que parece algo básico, dadas todas características já citadas, até você perceber que várias linguagens de programação amplamente utilizadas não tem essa característica); um grande conjunto de funções úteis para operar na estrutura de dados universal; e estratégias padrão para utilizar a estrutura de dados universal para representar estruturas de dados mais especializadas.

Então talvez a verdade esteja em algum lugar entre os extremos que Perlis apresentou de forma tão eloquente. Talvez o ponto de equilíbrio seja mais algo como 40 funções gerais o suficiente para operar de forma útil em uma estrutura de dados universal como listas, mas também 10 conjuntos de 6 funções que são relevantes quando tomamos uma das 10 visões especializadas daquela estrutura de dados universal. Isto é gerenciável se dermos bons nomes para essas funções e visões especializadas. 

A medida que você ler este livro, preste atenção não apenas para as construções de linguagem de programa e como elas são utilizadas, mas também para os _nomes_ dados para funções, variáveis e estruturas de dados. Eles não são tão curtos e vívidos como os nomes que Iverson escolheu para suas funções APL, mas eles foram escolhidos de forma deliberada e sistemática para aprimorar sua compreensão da estrutura geral do programa.

Primitivas, meios de combinação, abstrações funcionais, nomeação e convenções para utilizar uma estrutura de dados universal de maneira especializada ao delinear distinções: estes são os blocos fundamentais de uma boa linguagem de programação. A partir daí, imaginação e bom julgamento de engenharia baseado em experiência podem fazer o resto.

Guy L. Steel Jr., Lexington, Massachusetts, 2021.  