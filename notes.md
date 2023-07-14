#### 14/07/2023

Curso de 
Git e GitHub: repositório, commit e versões

@01-Conta no GitHub

@@01
Apresentação

Guilherme: Olá! Meu nome é Guilherme Lima, sou instrutor aqui na Alura e quero te convidar a participar desse treinamento de Git e GitHub.
Paulo: E eu sou o Paulo Silveira, CEO da Alura, sou eu que estou sempre atrapalhando o projeto de desenvolvedoras e desenvolvedores aqui e mexendo nos repositórios, fazendo os commits.

Estou aqui para colaborar com o Guilherme, como aluno e dando minhas ideias, meus pitacos, para que você possa entender como você vai criar repositórios e para quê usá-los.

Guilherme: Nesse treinamento você vai aprender muita coisa importante para o seu dia a dia como pessoa que trabalha com código e software.

Paulo: Vamos mostrar tanto na web, lá no site do GitHub, para você criar sua conta, fazer seu setup, preparar seu repositório, e "commitar". Usar essas palavras: commit, push, pull, tanto via web quanto a partir da linha de comando do seu Linux, do seu Windows, do seu Mac, para fazer isso via comando no terminal. Porque ainda hoje isso é muito usado. Apesar de que, muitas vezes, na web conseguimos fazer muita coisa, até abrir um editor tão poderoso quanto o Visual Studio Code.

Guilherme: Além disso, você vai aprender a trabalhar em um repositório chamando outras pessoas que desenvolvem. No curso você vai ver de forma prática eu convidando o Paulo para participar de um projeto que vamos desenvolver ao longo desse treinamento.

Paulo: Vou mexer nos arquivos de um lado, o Guilherme vai mexer do outro, como isso tudo se mistura, quem é dono do quê, como voltamos atrás no arquivo, como criamos o tal do branch, o que é o main ou master. Você vai entender tudo isso e vai ser fundamental, independentemente se você é back-end, front-end, data scientist ou até mesmo gestor de produtos, uma pessoa de agile.

Esse curso está incrível e é fundamental na sua carreira na área de desenvolvimento.

Guilherme: Isso aí. Vamos lá?

@@02
Explicação

Olá!
É muito bom ter você aqui para aprender sobre Git e GitHub. Essas ferramentas desempenham um papel fundamental no desenvolvimento de software colaborativo, permitindo que equipes trabalhem juntas de forma eficiente e organizada. Vamos explorar os conceitos básicos e entender como usar o Git em conjunto com o GitHub para gerenciar projetos de forma eficaz.

Divisão das aulas
Aula	O que vamos aprender nesta aula?
GitHub	Vamos conhecer a plataforma de hospedagem de código colaborativa mais importante do mundo.
Commit, VSCode e equipe	Vamos descobrir como salvar alterações no histórico do projeto Git
Trabalhando localmente	Trabalhemos localmente com Git para melhorar nossa colaboração e eficiência.
Adicionando arquivos	Vamos manter o histórico de alguns arquivos local e como enviá-los para o GitHub
Ramificações e merge	Vamos aprender como navegar entre as versões e no tempo em nossos projetos.
Preciso instalar algum software ou programa para seguir este curso?
Neste primeiro momento não é preciso. Você precisa ter uma conta de email para realizar seu cadastro no GitHub apenas.

Em caso de dúvida na instalação ou durante o curso, conte sempre com o fórum da Alura!
:)

@@03
O ponto central

Guilherme: Vamos iniciar a nossa jornada nos estudos de Git e GitHub? Para isso, temos aqui a ilustre presença do Paulo.
Paulo: Oi, pessoal. Estou muito contente de poder participar desse curso fundamental, porque a primeira dúvida que as pessoas têm é " Para quê eu uso e por que estão usando essas duas palavras: Git e GitHub?".

Então, já queremos avisar para você não se preocupar agora com essa diferença de às vezes falarmos GitHub e em outras vezes falarmos Git. Isso está um pouco misturado, com o tempo vai ficar mais clara a distinção, mas o principal aqui é que possamos criar nossa conta, usar nosso repositório e distribuir nosso código. Não é isso, Guilherme?

Guilherme: Isso mesmo. É até interessante isso, porque a maioria das vagas em programação pedem conhecimento em Git e GitHub, então é algo fundamental para nossa carreira como pessoa desenvolvedora.

Paulo: Independente da área em que você vai trabalhar, ou até mesmo se você vai gerir projetos, é fundamental entender onde está o projeto que foi criado pelo time de desenvolvedores, como posso olhar, como posso editar um arquivo, como posso às vezes até rodar o sistema na minha máquina. Então, não existe mais aquele projeto em que só uma pessoa trabalha, está tudo muito misturado, as equipes são muito grandes, não dá para ficar com o código em um único lugar.

Guilherme: Não dá mesmo, Paulo. Isso me lembrou da época da faculdade, eu estava fazendo o TCC da faculdade junto com três amigos, cada um ficou responsável por uma área específica do nosso projeto. Eu fiquei com back-end, um outro amigo ficou com front-end. E na hora de juntar todos os códigos e falar "o projeto final é esse", era uma dificuldade porque eu fazia a parte do back-end e quando estava funcionando uma determinada funcionalidade que tínhamos combinado, eu copiava o código e mandava esse código para o meu amigo que estava fazendo o front-end.

Paulo: Por e-mail ou um link do Dropbox, algo assim?

Guilherme: Isso mesmo. Eu mandava pra ele e ele quebrava tudo que ele já tinha feito, e quando ele arrumava com o back-end que mandei pra ele, eu já estava codando uma outra parte e outros dois amigos codando outra parte. Nunca conseguíamos juntar as coisas.

Paulo: Esse é um problema real. Quando o Guilherme estava na faculdade já existiam ferramentas como Git e GitHub em que ele podia controlar as versões de software. Por isso tem esse nome de versionamento, para você versionar o seu sistema e falar "essa é a versão 1, essa é a versão 1.2, essa é a versão 2..." E todo mundo trabalha em equipe de forma rápida.

Quando o Guilherme atualiza o back-end, eu, que trabalho no front-end, quero saber dessa mudança o mais rápido possível. E atualizar aqui no meu sistema, para podermos realmente trabalhar em conjunto e não ter problema de trabalhar com versões diferentes e ter falhas na comunicação.

Então, no mundo de hoje em que mesmo em empresas pequenas existem equipes grandes, precisamos de ferramentas que nos ajudam a unificar o que estamos trabalhando. Antes já existiam outras ferramentas, mas Git e GitHub é a principal ferramenta, que todo mundo no universo de tecnologia usa para, de alguma forma, conversar de uma maneira única no sistema. Todo mundo trabalhando no mesmo lugar de forma dinâmica, que dá para usar pela web, pela linha de comando, dá para integrar tudo, criar subversões, dá para fazer mil coisas com Git e GitHub. O principal é que vamos centralizar tudo em um único local, para não ter esses problemas que o Guilherme citou.

Guilherme: Isso aí. Lembrando que na época em que eu fiz o meu TCC eram 4 pessoas de programação juntas, imagina uma equipe de 50 ou 500 devs trabalhando no mesmo projeto utilizando a metodologia que eu usava, que era copiar, colar e enviar o código para as pessoas do grupo. Teria muitos problemas, não seria possível chegar em soluções que conhecemos hoje como a própria Alura, Netflix e outras empresas que possuem muitos desenvolvedores, é muito complexo.

Então, resumindo tudo o que conversamos aqui. O GitHub será um ponto central onde vamos manter o nosso código e manter versões do nosso código.

O que vamos aprender na sequência é o seguinte: Git e GitHub realmente são coisas diferentes e vamos começar a dar nossos primeiros mergulhos no GitHub. Nos encontramos no próximo vídeo.

@@04
Conta no GitHub

Paulo: Olá! O que você vai fazer agora é criar sua conta no GitHub. Não é isso, Guilherme? Você vai entrar no site do GitHub, que pode estar um pouco diferente à medida que eles vão atualizando, normalmente está em inglês. E no canto superior direito tem o botão de "Sign up" para você criar a sua conta.
Você precisa preencher seu cadastro. Inclusive, já que é algo muito importante na vida de uma pessoa desenvolvedora, você vai precisar ativar aquele fator de autenticação no seu celular.

Você vai ver que é simples se cadastrar e ter uma conta de graça no GitHub. Agora o Guilherme vai logar na conta dele, para mostrar que depois de criar seu login, você já pode criar o seu projeto, que podemos chamar de repositório.

Guilherme: Aqui no GitHub, talvez essa parte visual esteja um pouco diferente para você. O que o Paulo falou é uma coisa muito legal, muito importante, vamos precisar armazenar o nosso código na nuvem, essa é a função do GitHub, pegar o nosso código e armazenar o nosso código. Não é colocar só o seu site no ar, é colocar o seu código para que ele fique aqui e se você precisar fazer alterações você pode atualizar esse código.

Onde colocaremos o nosso código? Colocaremos em uma pasta que aqui no GitHub chamaremos de repositório. Para criarmos um repositório no GitHub existem duas formas. A primeira: podemos clicar no ícone de mais que está no canto superior direito e selecionar "New repository". Lembrando que um repositório vai ser uma pasta e você vai colocar o seu projeto dentro dessa pasta.

Após clicarmos em "New repository" ele vai abrir uma página em vou definir o nome desse repositório, colocar uma descrição, informar se ele é público ou privado. E existe uma outra forma mais recente que é digitar na barra de endereços do navegador: repo.new. Quando escrevo repo.new e clico no "Enter", vou cair na mesma página decriação de repositório.

Vou criar um nome bem genérico para esse repositório, pode ser "Primeiro repositório"? Algo assim, Paulo?

Paulo: Vamos colocar um nome mais de projeto mesmo, pode ser "sistema-de-cadastro", por exemplo.

Guilherme: Beleza. Na descrição vamos colocar alguma coisa?

Paulo: Pode pular a descrição.

Guilherme: Vou deixar esse repositório como "público". Se deixo como "privado" só eu vou ter acesso a esse repositório e posso convidar outros colaboradores para trabalhar nesse projeto, se deixo público qualquer pessoa tem acesso a ele.

Paulo: Quais arquivos vamos guardar aí para que eu possa trabalhar com você remotamente?

Guilherme: Inicialmente é só um readme (leia-me).

Paulo: Tá bom. Vamos começar mais simples, com texto de readme. Mas vai ser um sistema de cadastro dos jogos de videogame que nós temos, certo?

Guilherme: Certo, pode ser. Aí depois da definição se o repositório é público ou privado, tem a opção "Add a README file", não vou selecionar essa opção. Eu quero criar esse readme de uma outra forma junto com você.

Paulo: Vale lembrar que se estiver público qualquer pessoa no mundo vai poder acessar e baixar. Agora, se você estiver trabalhando dentro de uma empresa, 99% do tempo vai ser privado. Se você está trabalhando com algo para mostrar o que você está estudando, montar um portfólio, ou algo que vai ser open source que você quer que seus amigos e amigas usem, aí você vai escolher público. Tome cuidado.

Guilherme: Isso aí. E aqui embaixo temos o botão "Create repository" para criar o nosso repositório. Ao clicar nesse botão ele abre essa tela que vocês vão ver muito durante a vida de você como pessoa que trabalha com código. Aparecem alguns código aqui, mas não vamos focar nisso ainda. E aparece algumas opções para criarmos um novo arquivo, fazer upload de arquivos que já existem, ele fala até para incluirmos um readme, um tipo de licença, o gitgnore, vamos ver isso mais adiante.

Eu quero criar um novo arquivo, vou clicar na opção "creating a new file". Vou dar um nome para esse novo arquivo, vou chamá-lo de README.md. Esse .md significa "markdown", que é uma linguagem de estruturação de estilos em que podemos configurar nossas fontes de forma bem simples.

Paulo: E esse arquivo readme (leia-me) é muito comum. Todo mundo que trabalha com projetos de desenvolvimento já viu, na hora que baixar esse repositório na minha máquina, eu já vou querer saber o que fica em cada diretório, como executo, se eu preciso de um banco de dados, etc. Normalmente, as informações principais estarão nesse arquivo readme. É lá que alguém vai ter definido o passo a passo para você poder colaborar nesse projeto.

Guilherme: Para começar, vou colocar aqui uma tag h1 com o título <h1>sistema de cadastro de jogos</h1>. E vou colocar embaixo o texto "status do projeto: em desenvolvimento".

Assim como o Paulo disse, nesse arquivo fazemos um passo a passo do que é preciso fazer para esse projeto funcionar, o que é preciso baixar, quais módulos são necessários, etc. Como é um projeto lúdico para exemplificar, vou deixar só essas duas linhas, mas no geral colocaríamos mais informações sobre esse projeto.

Paulo: Pode até colocar aí, Guilherme, um exemplo: Para rodar esse projeto na sua máquina, por favor digite: npm install react. Sendo que o trecho com o código "npm install react" está entre três crases seguidas que é a sintaxe do markdown para códigos, três crases na linha acima e três crases na linha abaixo do código. Se você clicar na aba "Preview" pode ver como vai ficar esse texto com o markdown aplicado.

Você vai ver por aí em muitos repositórios de GitHub esses arquivos .md, normalmente são arquivos de documentação, arquivos que vão virar documentação ou conteúdo em um site. Então, esse formato markdown é muito comum por aí. Aqui queremos que além de você aprender GitHub e Git, aprenda também o contexto e a cultura que está em volta de desenvolver repositórios em time.

Guilherme: Agora que já temos o readme do nosso projeto, preciso salvar esse arquivo dentro do nosso repositório de sistema de cadastro. Rolando a página para baixo, teremos um botão com o texto "Commit new file". O que seria isso? O que é um commit? Vamos pensar inicialmente que um commit é um rótulo das alterações que estamos fazendo, ele é o momento exato de como está o nosso projeto. Então, vou passar aqui um rótulo, um nome para ele.

O que fizemos criando esse arquivo? Criamos o README.md, então posso inserir no nome desse meu commit: "criando o arquivo readme".

Para que esse arquivo seja armazenado no repositório temos que criar um commit, esse é um passo que vamos lembrar durante todo o nosso treinamento. Depois que eu apertar esse botão "Commit new file", ao acessar novamente o nosso projeto já aparece um campo com esse arquivo README.md que nós criamos.

Mesmo que você esteja trabalhando em um projeto em desenvolvimento, é recomendado que você crie um readme no seu projeto. Porque vai chegar um momento em que você terá muitos repositórios e nem vai lembrar mais o código, por isso você precisa de um readme bem estruturado para entender aquele projeto.

Observe que ele mostra o nome do commit que nós criamos, ele vai mostrar o estado temporal que criamos esse determinado arquivo. Então essa é talvez uma das coisas mais importantes do Git e GitHub. Meu código está na nuvem, e eu consigo armazenar estados do meu código. Fiz uma alteração, vou lá e faço um commit, o Paulo fez uma alteração, ele vai lá e faz um commit. Assim conseguimos ter versões do nosso código. Aqui temos só um readme , mas se fosse um projeto maior o processo seria o mesmo.

@@05
Faça como eu fiz: conta no Github

Agora é a sua vez de criar uma conta no GitHub!

Acesse o site do GitHub. Clique em Sign Up, preencha as informações com seu e-mail, senha e username e depois clique em Continue e em Criar Conta. Será enviado um e-mail para você com um código de 8 dígitos que precisará informar e após isso algumas opções para preencher sobre preferências de uso do site.
E pronto! Parabéns, sua conta está criada.

Site do GitHub mostrando como criar uma conta inserindo e-mail, senha e username

@@06
Para que serve o GitHub?

Uma equipe de pessoas desenvolvedoras está trabalhando em um projeto para realizar mudanças na plataforma de cursos da Alura. Uma pessoa está fazendo uma melhoria no código, outra precisa corrigir um bug no sistema e outra vai alterar as cores do dashboard.
Essas mudanças estão ocorrendo simultaneamente e, para agilizar o desenvolvimento, os devs querem ter acesso ao código atualizado com as mudanças feitas pela equipe em tempo real.

O que você pode fazer para solucionar essa questão?

Alternativa correta
Copiar as implementações no código e enviar para todas as pessoas da equipe; e o mesmo processo seria feito por elas.
 
Alternativa correta
Utilizar o GitHub, pois é uma plataforma de gerenciamento de código que permite gerenciar equipes pequenas e é específica para hospedagem de códigos relacionados ao front-end.
 
Alternativa correta
Utilizar o GitHub, pois ele serve para unificar as mudanças de toda a equipe em um único local, denominado repositório.
 
Alternativa correta! Isso mesmo, com o GitHub, a equipe de devs poderá gerenciar muito mais facilmente as alterações no projeto. Um repositório é basicamente um diretório onde ficarão reunidos todos os arquivos do projeto e poderá ser acessado por todas as pessoas da equipe.

@@07
Para saber mais: Readme

Você já deve ter instalado algum software que continha um arquivo em .txt em uma de suas pastas com o nome Readme. Pois bem, esse arquivo significa literalmente Leiame, e contém instruções que geralmente são para você saber como fazer a instalação do software.
Em projetos do Github, o Readme é um arquivo com extensão .md (Markdown) que contém as informações necessárias para entender o objetivo e status de seu projeto. O markdown é uma linguagem de marcação de texto, assim como html, só que mais simples. Quer saber mais sobre o markdown? O Paulo Silveira te explica neste artigo.

Mas, por que eu preciso de um Readme no repositório do meu projeto?

No readme, você pode dar uma descrição sobre o que é o seu projeto, qual o status atual dele, as tecnologias utilizadas, o time que trabalha no desenvolvimento, como contribuir (se for open source), como usar, etc. Existe uma grande possibilidade de coisas que você pode colocar no seu readme com a finalidade de informar e ser mais atrativo e organizado possível para quem estiver visualizando seu projeto.

E para te ajudar nesta tarefa de personalizar o seu Readme, a Camila Fernanda Alves escreveu um artigo incrível que te mostra como escrever um bom Readme para seu projeto.

Como escrever um README incrível no seu Github

@@08
O que aprendemos?

Nesta aula:
Conhecemos o Github, criamos uma conta e entendemos para o que ele serve;
Criamos um repositório com um Readme;
Fizemos um Commit e aprendemos quando é a hora certa de fazer um.
Na próxima aula:
Vamos mergulhar no mundo do Github, estilizar nosso Readme e conhecer o Github Pages!

@02-Commit, NVScode e equipe

@@01
Commit

Paulo: Guilherme, vamos adicionar mais um arquivo. Um app.js onde fica o nosso sistema rodando. Fazer só um console.log(). Podia ser PHP, podia ser Java, Python, pode ser o que você quiser. Vamos fazer via web no site do GitHub, porque depois vamos aprender que dá para fazer na nossa máquina local e mandar lá para o GitHub.
Veremos que dá para fazer dessas duas formas. Porque por enquanto estamos fazendo tudo no site, tudo via web. Estranho programar na web, não é? Mas é fundamental porque durante muito tempo da sua vida você vai passar navegando no site do GitHub, procurando seus arquivos, vendo o que seus colegas fizeram, e assim por diante.

Guilherme: Vamos lá. Vou criar um novo arquivo, "Add file > Create new file", esse arquivo será um arquivo JavaScript, app.js. E dentro dele vamos escrever: console.log("Rodando o sistema de gerenciamento de jogos").

Em seguida, vou preencher o campo do commit: "criando o arquivo js com o console". Vou fazer um commit direto nessa main, não vou alterar nada, não vamos nos preocuparmos com essas coisas ainda. E vou clicar no botão "Commit new file".

Agora temos dois arquivos. Observe que podemos entrar no arquivo do readme e, ao clicar no ícone do lápis, podemos editá-lo. Isso vai estar habilitado quando eu for o dono do repositório. Vou clicar no ícone do lápis e substituir o "npm install react" por "node app.js" para ele rodar o nosso console.log().

Agora que fizemos essa alteração no readme, vamos precisar dar um nome para essa alteração na área do commit. Vou colocar "alterando o readme do projeto", e vou clicar em "Commit changes".

Observe que agora o nosso arquivo foi atualizado. Mas editar esses arquivos talvez fique um pouco difícil aqui no GitHub com esse esse layout. No próximo vídeo quero te mostrar algo incrível que você pode fazer com o GitHub para continuar editando, não com todos os recursos que temos localmente, mas ainda assim editando de uma forma um pouco mais conhecida por todos nós e ainda na nuvem.

@@02
Realizando um commit

O commit é uma ação muito importante do Git para nos ajudar no controle da versão do nosso projeto. Um commit pode ser considerado como um marco ao longo do cronograma de um projeto.
Sabendo disso, quando realizamos um commit, estamos:

Sabendo disso, quando realizamos um commit, estamos:

Alternativa correta
Adicionando as alterações mais recentes do projeto.
 
Alternativa Correta! Um commit guarda o estado do seu projeto naquele momento.

Alternativa correta
Enviando as alterações do projeto para o repositório remoto.
 
Alternativa correta
Criando um repositório no GitHub.

@@03
VSCode no GitHub

Paulo: Estamos editando tudo na web, nesse editor muito fraco do GitHub que não tem corretor, não executa código, é só um editor de texto básico.
O próximo passo é ter um lugar mais interessante para editar na web. Antes de ser na nossa própria máquina. Então, agora se o Guilherme me convidar para participar desse projeto eu ganho poder de edição e posso editar usando esse mesmo editor que estávamos usando. Mas dá para fazer de um jeito mais interessante e o Guilherme vai explicar para nós como fazer.

Guilherme: Isso aí. Existe quase um "atalho hacker" para conseguirmos editar nosso código do GitHub utilizando uma estrutura do Visual Studio Code.

O objetivo é o seguinte: agora, quero criar uma página HTML para nosso sistema de cadastro e quero criar a estrutura da minha página HTML. Colocar ali o tipo de dicionário, qual a versão do HTML eu quero utilizar. Vamos carregar uma forma mais fácil de conseguir editar o nosso código. Vou pressionar a tecla ponto (.) e esperar ele carregar.

Olha que interessante, carregou um layout do Visual Studio Code. Ele tem algumas limitações, como por exemplo, o uso do terminal, algumas coisas mais avançadas. Mas para criarmos um arquivo HTML, colocar um código JavaScript ou CSS, ele funciona legal. Também conseguimos fazer bastante coisa por aqui.

Então vou clicar no ícone de "new file", criar um arquivo chamado index.html e dentro desse index quero criar toda a estrutura do HTML. Para isso, existe um atalho em que eu insiro no código um ponto de exclamação e aperto "Enter", e ele coloca toda essa estrutura de 12 linhas do HTML automaticamente.

Paulo: Lembrando que isso é algo do VS Code mesmo. Ele tem muitos templates, atalhos, e a maioria deles está disponível dentro desse VS Code da web. Tem gente que não gosta de trabalhar nesse layout na nuvem e vai criticar, mas a tendência é que no futuro mais coisas aconteçam na nuvem mesmo.

Guilherme: Nesse documento, na linha 2, ele fala que a linguagem está em inglês ("en"), eu vou substituir para português brasileiro: <html lang="pt-br">. O título eu vou deixar <title>Meus jogos</title>.

E dentro do body, vou colocar um h1. Quando eu escrevo "h1" e aperto "Enter", note que ele automaticamente completa a sintaxe da tag. Vou escrever <h1>Sistema de cadastro de jogos</h1>. É isso que quero criar na minha index.html.

Mas temos um detalhe importante, se eu voltar no meu repositório observe que ainda não temos esse index.html listado entre os arquivos do meu projeto. Porque precisamos fazer o commit. Voltando ao VS Code do navegador, vemos que no menu da barra lateral esquerda tem um ícone de "Source Control", controle de versão. Tem um pontinho com o número 1 aqui, ele identificou que existem alterações no nosso repositório. Vou clicar nesse ícone do "Source Control". Ele exibe uma mensagem informando um campo em que podemos criar a mensagem do commit.

Ele está vendo todas as mudanças que fazemos em diferentes arquivos. Se, por exemplo, eu alterar alguma coisa no README.md, ele vai indicar que o readme foi alterado. Conseguimos até comparar as alterações que fizemos.

Agora vou fazer de fato um commit, colocar um rótulo indicando que criei um arquivo index.html. Vou escrever na mensagem do commit: "criando o arquivo index do projeto" e para confirmar a criação do commit basta clicar no ícone da setinha aqui em cima.

Agora, ao atualizar a página do nosso GitHub vai aparecer o arquivo index no nosso projeto.

Para finalizar a nossa aula vou clicar no commit "criando o arquivo index do projeto". Olha que interessante, ele vai mostrar todas as alterações que foram feitas nesse estado. Repare que ele mostrou a alteração do readme e também a alteração do index. Então podemos visualizar as edições feitas em cada estado.

Se eu soubesse disso na época do TCC da faculdade, teríamos feito muito mais coisas. Então é isso, queremos que você tenha uma vida mais fácil e mais feliz. O GitHub vai te ajudar muito nos seus projetos tanto pessoais quanto profissionais.

@@04
Adicionando um colaborador

Paulo: Agora vamos colaborar juntos nesse projeto. Eu vou mexer no projeto que você criou porque teremos acesso ao mesmo repositório. Quero mexer no nosso app.js e adicionar mais uma linha de código. Para que isso seja visível tanto para você quanto para mim, você precisa me dar permissão de acesso nesse projeto.
Tem várias formas de fazer isso. O meu usuário no GitHub é "Peas", me adiciona para eu poder acessar e trabalhar nesse projeto.

Guilherme: Vamos clicar nas configurações do repositório, no botão "Settings" que está localizado no canto superior direito. Na página de configurações, clico em "Collaborators" e posso convidar um colaborador. Vou inserir aqui o nome do perfil do Paulo no GitHub e confirmar o convite.

Paulo: Agora vou poder editar. Antes eu já podia ler porque você criou um repositório público. Agora posso "commitar" no projeto e atualizar os arquivos que estão lá.

Guilherme: Paulo, agora eu quero que você compartilhe a sua tela para vermos essa alteração acontecendo.

Paulo: Eu devo ter recebido um e-mail com o seu convite também, mas já aparece aqui na minha tela uma notificação dizendo: "@guilhermeonrails te convidou para colaborar neste repositório". Eu posso clicar nessa notificação para ver o convite e confirmar a minha participação nesse repositório.

Vou aceitar o convite e agora tenho acesso aos mesmos arquivos que editamos antes. Vou clicar no arquivo app.js e depois clicar no ícone de lápis para editá-lo.

Vou editar esse arquivo, colocarei uma segunda linha: console.log("Aplicação está se conectando ao banco de dados"). Claro que é só um exemplo fictício o que estamos criando aqui. Vou rolar a página e lá na área de commit vou escrever: "atualizando o init do projeto".

Vou clicar em "Commit changes" e ao vermos o nosso repositório já atualizado, vai aparecer dois colaboradores nesse projeto, eu e o Guilherme. E todo mundo que está nesse projeto tem acesso a isso instantaneamente. Não tem como uma pessoa ficar desatualizada, está todo mundo na mesma página.

Agora, vai ter lá o histórico de que horas eu modifiquei esse arquivo.

Guilherme: Depois que você fez a atualização eu recebi uma notificação avisando que você fez uma alteração no projeto.

Paulo: Então é assim que você vai colaborar com seus amigos, não se esqueça. Eu acho muito importante você ir lá no Discord da Alura e encontrar pessoas que estão na mesma fase que você para trocar ideias e talvez até criar um projeto juntos. Assim você já vai sentindo como é o verdadeiro ambiente em um ambiente de trabalho.

@@05
Faça como eu fiz

Chegou a hora de você seguir todos os passos realizados por mim durante esta aula. Caso já tenha feito, excelente. Se ainda não, é importante que você execute o que foi visto nos vídeos para poder continuar com a próxima aula.

Opinião do instrutor

Continue com os seus estudos, e se houver dúvidas, não hesite em recorrer ao nosso fórum!

@@06
O que aprendemos?

Nesta aula:
Aprendemos a acessar o VS Code por meio do GitHub;
Convidamos um colaborador em um repositório do GitHub;
Entendemos como verificar o histórico de commits realizados.
Na próxima aula:
Vamos clonar um projeto, entender a diferença entre repositório local e remoto e aprender mais comandos do git!