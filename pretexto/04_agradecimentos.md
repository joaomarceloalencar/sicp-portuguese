# Agradecimentos

A adaptação de "Estrutura de Interpretação de Programas de Computadores" (_Structure and Interpretation of Computer Programs_ - SICP JS) foi desenvolvido na Universidade Nacional de Cingapura (_National University of Singapore_ - NUS) para a disciplina CS1101S. Essa cadeira foi ministrada em conjunto com Low Kok Lim por mais de seis anos, cujo julgamento pedagógico sensato foi crucial para o sucesso da disciplina e deste projeto. O time de docentes da CS1101S incluiu vários colegas da NUS e mais de 300 alunos de graduação atuando como monitores. O retorno contínuo fornecido por essa equipe nos últimos nove anos nos permitiu resolver inúmeros problemas específicos da _JavaScript_ e remover complicações desnecessárias e mesmo assim manter as características essenciais tanto do texto original quanto da linguagem _JavaScript_.

SICP JS é também um projeto de _software_. Nós obtivemos o código fonte em _Latex_ do livro original em 2008. Um conjunto de ferramentas para compilação do livro foi desenvolvida por Liu Hang e aprimorada por Feng Piaopiao. Chan Ger Hean desenvolveu as primeiras ferramentas para a versão impressa, que serviram de base para Jolyn Tan desenvolver as ferramentas para a primeira edição eletrônica e por último He Xinyue e Wang Qian reajustaram essas ferramentas para a versão atual de comparação. Samuel Fang projetou e desenvolveu a versão _online_ de SICP JS. 

A versão _online_ de SICP JA e da disciplina CS1101S se baseiam fortemente em um sistema de _software_ chamado _Source Academy_ e as sublinguagens _JavaScripts_ suportadas são chamadas _Source_. Várias dúzias de alunos contribuíram para a _Source Academy_ durante a preparação da SICP JA e o sistema os lista de forma proeminente como "Contribuidores". Desde 2020, os alunos do curso CS4215 na NUS, Implementação de Linguagens de Programação, contribuíram com várias implementações de linguagens que são utilizadas no SICP JS: a versão concorrente da _Source_ utilizada na seção 3.4 foi desenvolvida por Zhengqun Koo e Jonathan Chan, a implementação da avaliação preguiçosa usada na seção 4.2 foi desenvolvida por Jellouli Ahmed, Ian Kendall Dunca, Cruz Jomari Evangelista e Alden Tan; a implementação não determinística usada na seção 4.3 foi desenvolvida por Arsalan Cheema e Anubhav; e Daryl Tan ajudou a integrar essas implementações na _Academy_.

Somos gratos à Fundação Sueca para Cooperação Internacional em Pesquisa e Educação de Nível Superior (_The Swedish Foundation for International Cooperation in Research and Higher Education_ - STINT), cujo programa sabático conectou Martin e Tobias e permitiu ao último trabalhar como professor auxiliar na disciplina CS1101S e participar do projeto SICP JS.

Gostaríamos de reconhecer o corajoso trabalho do comitê ECMAScript 2015, liberado por Allen Wirfs-Brock. SICP JS depende fortemente nas declarações _constant_ e _let_, além das expressões _lambda_, todas funcionalidades adicionadas a _JavaScript_ no padrão ECMAScript 2015. Essas adições nos permitiram ficar próximos em termos de apresentação das ideias mais importantes do SICP. Guy Lewis Steele Jr., que liderou a primeira padronização ECMAScript forneceu retorno detalhado e útil em alguns exercícios do capítulo 04.

[Martin Henz](https://www.comp.nus.edu.sg/~henz/) e [Tobias Wrigstad](http://wrigstad.com/)

## Agradecimentos da Segunda Edição de SICP, 1996

Gostaríamos de agradecer as várias pessoas que nos ajudaram a desenvolver este livro e ementa. 

Nossa disciplina é uma clara descendente intelectual da "6.231", uma maravilhosa disciplina em linguísticas de programação e cálculo _lambda_ ensinada no MIT no final dos anos 1960 por Jack Wozencraft e Arthur Evans Jr.

Temos uma grande dívida a Roberto Fano, que reorganizou o currículo introdutório do MIT em engenharia elétrica e ciência da computação para enfatizar os princípios de projeto na engenharia. Ele nos liderou ao iniciar nosso projeto e escreveu as primeiras notas de disciplinas das quais este livro evoluiu.

Muito do estilo e estética de programação que nós tentamos ensinar aqui foram desenvolvidas em conjunto com Guy Lewis Steele Jr, que colaborou com Gerald Jay Sussman no desenvolvimento inicial da linguagem _Scheme_. Além deles, David Turner, Peter Henderson, Dan Friedman, David Wise e Will Clinger nos ensinaram várias das técnicas da comunidade de programação funcional que aparecem neste livro.

Joel Moses nos ensinou sobre estruturação de grandes sistemas. Sua experiência com o sistema Macsyma para computação simbólica forneceu a visão de que deve-se evitar complexidades de controle se concentrar na organização dos dados para refletir a verdadeira estrutura do mundo sendo modelado.

Marvin Minsky e Seymour Papert formaram várias das nossas atitudes sobre programação e seu lugar nas nossas vidas intelectuais. Para eles devemos a compreensão que computação fornece um meio de expressão para explorar ideias que de outra forma seriam muito complexas para lidar com precisão. Eles enfatizam que a habilidade de um estudante para escrever e modificar programas fornece um meio poderoso no qual exploração se torna uma atividade natural. 

Também concordamos fortemente com Alan Perlis ao afirmar que programação é muito divertida e devemos nos preocupar em manter a diversão ao programar. Parte dessa alegria deriva de observar grandes mestres trabalhando. Somos sortudos por termos sido programadores aprendizes de Bill Gosper e Richard Greenblatt. 

É difícil identificar todas as pessoas que contribuíra para o desenvolvimento do nosso currículo. Agradecemos a todos professores, instrutores e tutores que trabalharam conosco nos últimos quinze anos e trabalharam várias horas extra na nossa disciplina, especialmente Bill Siebert, Albert Meyer, Joe Stoy, Randy Davis, Louis Braida, Eric Grimson, Rod Brooks, Lynn Stein e Peter Szolovits. Gostaríamos de reconhecer especialmente as exemplares contribuições pedagógicas de Franklyn Turbak, agora na universidade Weslley; seu trabalho no ensino da graduação definiu um padrão que todos nós podemos almejar. Estamos gratos a Jerry Saltzer e Jim Miller por nos ajudar a entender os mistérios da concorrência e a Peter Szolovits e David McAllester para suas contribuições na explicação de avaliação não determinística no capítulo 04. 

Muitas pessoas empregaram esforço significativo apresentando este material em outras universidades. Alguns dos quais trabalhamos de maneira mais próxima foram Jacob Katzenelson na Technion, Hardy Mayer na Universidade da Califórnia em Irvine, Joe Stoy na Oxford, Elisha Sacks na Purdue e Jan Komorowski na Universidade Norueguesa de Ciência e Tecnologia. Somos excepcionalmente orgulhosos de nossos colegas que receberam importantes prêmios de ensino por suas adaptações dessa disciplina em outras universidades, incluindo Kenneth Yip em Yale, Brian Harvey na Universidade da Califórnia em Berkeley e Dan Huttenlocher na Cornell.

Al Moyé nos permitiu ensinar esse material para engenheiros na Hewlett-Packard e produzir gravações dessas aulas. Gostaríamos de agradecer os talentosos professores - em particular Jim Miller, Bill Siebert e Mike Eisenberg - que projetaram cursos de educação contínua incorporando as gravações e ensinaram o material em universidades e empresas ao redor do mundo. 

Vários professores em outros países empregaram esforço significativo na tradução da primeira edição. Michel Briand, Pierre Chamard e André Pic produziram a edição francesa, Susanne Daniels-Herold produziu uma edição alemã e Fumio Motoyoshi produziu uma edição japonesa. Não sabemos quem produziu a edição chinesa, mas consideramos uma honra ter sido selecionados como objeto de uma tradução "não autorizada".

É difícil listar todas as pessoas que fizeram contribuições técnicas para o desenvolvimentos dos sistemas _Scheme_ que usando para propósitos educacionais. Além de Guy Steele, os magos principais incluem Chris Hanson, Joe Bowbeer, Jim Miller, Guillermo Rozas e Stephen Adams. Outros que fizeram esforço significativo incluem Richard Stallman, Alan Bawden, Kent Pitman, Jon Taft, Neil Mayle, John Lamping, Gwyn Osnos, Tracy Larrabee, George Carrette, Soma Chaudhuri, Bill Chiarchiaro, Steven Kirsch, Leigh Klotz, Wayne Noss, Todd Cass, Patrick O’Donnell, Kevin Theobald, Daniel Weise, Kenneth Sinclair, Anthony Courtemanche, Henry M. Wu, Andrew Berlin e Ruth Shyu.

Além da implementação do MIT, gostaríamos de agradecer a todas as pessoas que trabalharam no padrão IEEE _Scheme_, incluindo William Clinger e Jonathan Rees, que editaram o R4RS e Chris Haynes, Davir Bartley, Chris Hanson e Jim Miller, que preparam o padrão IEEE.

Dan Friedman tem sido o líder da comunidade _Scheme_ há muito tempo. O trabalho amplo da comunidade vai além de tópicos de projeto da linguagem para incorporar significativas inovações pedagógicas, tais como o currículo de ensino médio baseado na EdScheme pela Schemer's Inc., e os maravilhosos livros por Mike Eisenberg, Brian Harvey e Matthew Wright.

Valorizamos o trabalho daqueles que contribuíram para tornar esse livro real, especialmente Terry Ehling, Larry Cohen e Paul Bethge na MIT Press. Ella Mazel achou maravilhosa imagem da capa. Para a segunda edição estamos particularmente agradecidos a Bernard e Ella Mazel pela ajuda no projeto do livro e a David Jones, extraordinário mago do Tex. Também estamos endividados para aqueles leitores que fizeram comentários aprofundados no novo rascunho, Jacob Katzenelson, Hardy Mayer, Jim Miller e especialmente Brian Harvey, que fez neste livro o que Julie fez no seu livro _Simply Scheme_.

Finalmente, gostaríamos de agradecer o apoio das organizações que encorajaram este trabalho através dos anos, incluindo apoio da Hewlett-Packard, possibilitado por Ira Goldstein e Joel Birnbaum e apoio da DARPA, possibilitado por Bob Kahn.

[Harold Abelson](https://en.wikipedia.org/wiki/Hal_Abelson) e [Gerald Jay Sussman](https://en.wikipedia.org/wiki/Gerald_Jay_Sussman) 



