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

@03-Trabalhando Localmente

@01
Instalando o Git

Nesta aula, vamos trabalhar com Git local!
Vamos instalar o Git para começarmos a controlar as versões dos nossos códigos. Para isso, clique neste link para abrir a página oficial do Git:

https://git-scm.com/

Agora, com base no seu sistema operacional, realize o download da instalação do Git, como ilustra na imagem abaixo:

Insira aqui a descrição dessa imagem para ajudar na acessibilidade

A instalação do Git é simples, porém se precisar de um passo a passo, temos esse vídeo que pode te ajudar!
Recomendamos realizar a instalação antes de dar continuidade no curso. Se precisar de ajuda, conte com o fórum da Alura!

https://git-scm.com

https://cursos.alura.com.br/course/git-github-controle-de-versao/task/57007

@02
Git clone e log

Paulo: Até agora estávamos usando o site do GitHub, cadê o Git? Quando usamos o GitHub estamos sempre usando o Git. Por que essa diferença? Por que essas palavras? GitHub é uma empresa, que inclusive foi comprada pela Microsoft. Mas ela foi criada justamente para facilitar o uso do Git. tudo que usamos aqui via web, antes da existência do GitHub e seus concorrentes era tudo na linha de comando.
Porque quem criou o Git, que é esse sistema que é só via linha de comando foi o Linus Torvalds, que é o criador do Linux. Não bastando ele criar o Linux, ele criou o maior sistema de controle de versão, que inclusive é distribuído.

Estamos sempre centralizando as coisas aqui, mas é engraçado pensar que o Git - aqui são detalhes que você vai aprender com o tempo - faz tudo isso aqui de forma distribuída. tudo que estará na minha máquina é igual ao que está na máquina do Guilherme, inclusive o histórico do projeto. Isso é um mecanismo interessante que você vai entender mais adiante.

O que queremos mostrar agora para você é que dá para você acessar o repositório e baixar todos os arquivos do projeto para a sua máquina, em vez de ficar usando a nuvem. Você pode e deve instalar o Git. Inclusive, tem aqui na Alura instruções para você instalar o Git no Windows, no Mac, no Linux, para poder usá-lo como linha de comando.

Guilherme mostra os passos de como fazer para clonar esse repositório para que esses arquivos finalmente fiquem locais e não somente na nuvem.

Guilherme: Para conseguirmos clonar esse repositório, vou vir no botão "Code" e copiar a URL que ele mostra nesse campo que apareceu. Agora vou abrir o meu terminal. Se eu fizer aqui o comando que utilizamos para clonar, ele vai colocar na pasta em que eu estiver na hora. Não é isso que eu quero, quero colocar todo esse repositório, por exemplo, no meu desktop. Vou usar o comando cd desktop para navegar para o meu desktop.

Agora se eu fizer o comando git clone e der um "Ctrl + V" para colar URL do sistema-de-cadastro.git vai aparecer aqui no nosso desktop a pasta do nosso projeto. Não foi mágica não, gente. Ele fez aqui o clone do nosso projeto.

Agora quero abrir esse projeto no meu VS Code e visualizar todo o código que tem nele. Mas antes vamos acessar a pasta com cd sistema-de-cadastro/, e com ls veremos o nome dos arquivos dentro dessa pasta.

Paulo: Antes de existir o GitHub era só assim que dava para fazer. Tudo que fizemos durante as aulas era na linha de comando. Mostramos primeiro via web para diminuir o trauma. Sem contar que realmente acreditamos que no futuro será cada vez mais na web e um pouco menos na linha de comando no sistema local. Mais no cloud e menos no computador local.

Guilherme: Uma coisa que o Paulo comentou, nós temos aqui os três arquivos e o Paulo falou que podemos trazer também o histórico das alterações que fizemos. Vamos visualizar o histórico antes de abrir o VS Code? O comando para conseguirmos visualizar todo o histórico de alterações é git log. Ele vai mostrar os mais recentes, o autor da mudança e várias outras coisas. Repare que no final aqui ele deixou dois pontos (:), para sair desses dois pontos basta apertar a tecla "Q".

Mas será que conseguimos visualizar todas as alterações que fizemos em uma só linha? Conseguimos com o comando git log --oneline. Olha que interessante, ele vai mostrar todos os commits que fizemos nesse repositório de uma forma bem simples e resumida.

Aqui ele passa um número, que é um código para identificar essa alteração, é a forma como o GitHub trabalha por debaixo dos panos, e vem também a descrição, a mensagem do commit que faz sentido para nós.

Quando fazemos um clone de um determinado repositório do GitHub além dos códigos e todas as alterações que fizemos ele traz também o histórico de tudo que aconteceu naquele projeto.

@@03
Git status, commit e push

Link citado aos 11:45 do vídeo: documentação do GitHub para geração de chave SSH.
Paulo: Nós fizemos muitas das edições lá no site do GitHub, já percebemos vendo o log aqui que no Git, a grande sacada do Linus Torvalds teve quando criou o Git foi que esse repositório não é centralizado, ele está tanto no GitHub quanto agora, depois que você fez o comando git clone, ele está na sua máquina. É um sistema de controle de versão distribuído.

Se um dia deletassem os arquivos no GitHub, você teria todo o repositório na sua máquina e também tem o histórico. Então, é muito comum usarmos via linha de comando no nosso repositório local. Por mais que dê para fazer praticamente tudo via web, precisamos saber alguns comandos principais na linha de comando.

O que vamos aprender a fazer agora é saber se está tudo sincronizado com o nosso repositório, veremos qual é o status, se fizemos alguma mudança do nosso local que ainda não foi enviado para o repositório de origem - não chamamos de "central" chamamos de "origem" - e também vamos aprender a fazer o commit. Veremos que tem dois momentos, tem a hora que você "commita" e tem a hora que você empurra todas as mudanças do nosso repositório aqui da nossa máquina para o GitHub. Vamos ver isso na linha de comando?

Guilherme: Vamos.

Paulo: Tive uma ideia, vamos já ensinar a falar assim: "Pega todas as mudanças que fizeram lá no repositório origem e atualiza o projeto aqui no local". Como fazer isso?

Guilherme: Primeira coisa que vamos fazer é pegar aquele link mais uma vez, clicando em "Code" e copiando a URL do nosso projeto. De volta ao console, vou dar um git pull.

Paulo: O git pull é uma forma de fazer a atualização. Clonar é só a "primeira vez", agora quero puxar tudo que está lá para atualizar aqui.

Guilherme: Exatamente. Vou escrever git pull seguido do link que copiei, pressionei "Enter". E pelo o que ele informou estamos em dia.

Paulo: Então não teve atualização. Se alguém tivesse mexido lá enquanto eu e o Guilherme estamos dando a aula aqui. Seria informado aí que tal arquivo foi atualizado, tal arquivo foi deletado, tal arquivo foi adicionado.

Guilherme: Isso aí. Quem vai fazer essas atualizações somos nós, Paulo. Nós vamos mandar coisas diferentes para o nosso repositório.

Vou abrir o VS Code e vou arrastar a pasta do meu projeto, que está no desktop, para dentro do VS Code, para atualizar alguma parte da nossa aplicação. Temos aqui o nosso app.js, com os nossos console.log, o index.html, que inicialmente só tem o h1, e temos o readme.md.

O que faremos agora? Diferente do CodePen e outras ferramentas onde o HTML já entende o código CSS que já entende o código JavaScript, aqui não. No HTML eu preciso informar que tem um arquivo JavaScript rodando nesse projeto. Então, aqui na linha 10 vou dar um "Enter" e colocar um <script src=""> aqui. Esse script src vai informar que temos arquivos JavaScript a serem lidos: <script src="app.js">.

Agora sim, quando rodarmos essa aplicação o código que colocamos no app.js será executado no HTML. Então, a única coisa que fizemos foi linkar o arquivo JavaScript com o arquivo HTML.

Paulo: Vale lembrar que isso tudo é um projeto de mentira, mas estamos mostrando como as coisas acontecem. Você mexe em um arquivo, às vezes mexe em mais de um arquivo ao mesmo tempo. Nesse aqui só mexemos em um.

Guilherme: Podemos usar o terminal integrado do próprio VS Code para fazer alterações. Ao abrir o terminal do VS Code podemos usar o comando git status para ver o que tem de diferente nesse projeto. Quando dou um "Enter" ele vai falar que tem um arquivo que foi modificado, o arquivo modificado foi o index.html. Agora temos um desafio. Precisamos pegar essas modificações que fizemos aqui nesse arquivo. O VS Code até indica com uma linha verde no início da linha que foi modificada.

Paulo: O VS Code pega as coisas do GitHub que estão no local e percebe que você mudou aquela linha.

Guilherme: Tem duas formas para criarmos um commit com base nas modificações que fizemos agora. Podemos ir por esses ícones que estão aqui em cima no menu explorer ou podemos fazer via código. Como já fizemos no VS Code online lá no GitHub, agora eu vou fazer via código no terminal.

Paulo: Vamos direto no terminal ver o git status. Ele indicou que tem uma modificação sim. Agora vamos falar que queremos commitar esse arquivo. E somos obrigados a dar uma mensagem igual fizemos da outra vez. O comando que usaremos é o git commit.

Guilherme: Isso. Vamos usar o comando git commit para criar um commit assim como fizemos para os anteriores. Essa mensagem de commit é muito importante, aqui vamos passar exatamente qual arquivo queremos commitar.

Paulo: Pode até usar ponto se quiser o diretório inteiro, pode separar os arquivos por espaços, tem várias formas. Aqui só vamos commitar a modificação do index. E logo depois você põe uma mensagem.

Guilherme: Para criar essa mensagem, essa etiqueta desse commit, vou colocar, por exemplo, "linkando o app.js com o html": git commit index.html -m "linkando o app.js com o html". Pressiono "Enter" e pronto, ele fez o commit e adicionou essa alteração.

Vou limpar o terminal e rodar o git status novamente, dessa vez repare que ele não trouxe nenhuma modificação ele até fala aqui "use o push para publicar seus commits locais", ou seja, podemos pegar todas as modificações que fizemos localmente aqui na nossa máquina e mandar essas modificações lá para o nosso código no GitHub. Vamos fazer isso, Paulo?

Paulo: Vamos. Lembrando que "push" em português significa empurrar. Agora vamos empurrar todos os commits, posso ter feito mais de um, e vamos empurrar para o repositório origem.

Guilherme: Vou colocar aqui no terminal o comando git push origin main, porque estamos trabalhando só com a divisão principal, o main.

Paulo: No site do GitHub, já podemos ver essa atualização que foi "empurrada" para o repositório origem. Já começamos a ver alguma diferença: Git é a ferramenta e GitHub é o lugar que te ajuda a ter esse repositório origem para todo mundo poder trabalhar nesse projeto. Podemos ver que o último commit no arquivo index foi há 3 minutos.

Quando entramos no arquivo podemos, inclusive, clicar no botão "History", que está localizado à direita, para ver toda a história desse arquivo.

Estamos vendo tudo sendo amarrado aí. Pode ser que você tenha tomado uma mensagem de erro, porque para empurrar, ter o direito de escrever no repositório além de ter sido adicionado como colaborador no repositório, que foi o que o Guilherme fez comigo na outra aula, você precisa ter configurado corretamente os seus parâmetros de Git no seu computador. São alguns parâmetros que ficam num arquivo de configuração, como a sua chave pública. Inclusive, em algum lugar você terá uma chave primária.

Vamos deixar os links dessa configuração, esse momento tem umas linhas de comando a mais que você tem que fazer, basicamente, só uma vez na vida. Que é gerar sua chave para o GitHub saber, por exemplo, que o Guilherme que está empurrando isso é o Guilherme que tem o login e senha que ele logou no GitHub. Então isso tem aquele mecanismo de chave pública e chave privada de criptografia. Você não precisa entender desse assunto, futuramente no decorrer da sua carreira é importante, mas é uma forma de você saber que quem está conversando é uma pessoa que pode sim escrever no repositório.

Por que não aconteceu isso antes na web? Porque na web já estávamos logados dentro do GitHub, dessa vez fizemos do nosso local para a nuvem. Nessa hora que empurramos da nossa máquina para a nuvem o GitHub verifica se temos as credenciais para editar esse repositório. Ele checa mecanismos de permissão do Git. Através da chave, de assinatura, etc. Provavelmente muitos de vocês já fizeram isso quando instalaram o Git que está lá no nosso manual.

Guilherme: Isso aí. É por questões de segurança da nossa aplicação mesmo. E na sequência, vamos aprender como navegar entre versões diferentes. Por exemplo, subi uma versão mas quero voltar para uma versão anterior. Ou o que acontece geralmente na época da Black Friday, a maioria dos e-commerces alteram o layout e depois voltam para o layout padrão.

Como fazer essa navegação entre projetos? Será que o pessoal tira tudo na mão mesmo ou eles usam um comando no GitHub para mudar a versão do projeto? É isso que vamos descobrir.

https://docs.github.com/pt/enterprise-server@3.2/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

https://docs.github.com/pt/enterprise-server@3.2/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

@@04
O que vimos até aqui

Paulo: No intervalo, eu mexi em um arquivo do nosso sistema. Porque eu quero que você dê o pull e veja as modificações. Inclusive, tem várias formas de darmos pull ou push. O Guilherme fez das maneiras mais explícitas.
Quando nossos arquivos de configuração estão bem configurados, para o git pull basta fazer git pull, não precisa colocar aquela URL gigante. Então, se fizer um git pull agora, ele vai informar que o app.js tem três linhas a mais. Se você abrir o app.js agora vai ver que tem uma modificação lá.

Guilherme: Vamos ver na web também como essa atualização aparece.

Paulo: E se você clicar no commit dá para ver o histórico de edições.

Guilherme: Sim. Antes tínhamos duas linhas, agora temos três linhas adicionadas aqui, assim como ele nos informou no terminal.

Paulo: Ele mostra essa tela de como era antes e como está depois da edição, isso é o que chamamos de "diff". É muito comum falarmos: "Me mostra o diff do seu commit, deixa eu ver o que você modificou". Esse é um jargão muito comum. Você também pode fazer o diff dessa versão com versões mais antigas. Dá para fazer diff tanto via web quanto na linha de comando.

Tem coisas que, para ser sincero, vai ser até mais fácil em linha de comando. E é muito comum usar a linha de comando, é raro um time de desenvolvimento que vá usar apenas a versão web. Esperamos que no futuro seja apenas web, mas hoje você precisa encarar a linha de comando no terminal e praticar bastante.

Guilherme: Como você falou, nesse repositório específico posso fazer só um git pull, sem passar a URL, o mesmo aconteceria para um git push também. Não preciso passar a origem principal.

Vou colocar aqui no app.js mais um console.log(): console.log("Enviando para o GitHub"). Salvei esse arquivo, vou para o terminal e fazer um git commit app.js. Aqui tem um ponto interessante, se eu faço modificações em mais de um arquivo, posso colocar só o ponto: git commit ., isso significa que quero pegar todo o meu projeto. Vou colocar uma mensagem: git commit . -m "adicionando um console log". Vou dar um "Enter" e fazer o git push com esses dois, pressiono "Enter" e ele vai enviar para o repositório origem.

Quando voltarmos para o nosso repositório no site do GitHub já vai estar atualizado. Agora o arquivo app.js tem as edições do Paulo e a minha. Eu fiz o pull, fiz o commit e já fiz o push para enviar o código que eu fiz.

Lembrando, estou trabalhando sem nenhuma ramificação, um nome meio técnico que o pessoal dá para as divisões, existem várias estratégias para dividir o Git, para separar o que é código de teste, código de desenvolvimento e código principal. Quando trabalhamos em uma só raiz, que é o nosso código main, não precisamos especificar exatamente onde estamos trabalhando.

O que eu quero fazer agora é voltar a minha aplicação para um estado anterior. Na página do nosso repositório no GitHub, temos o ícone de um relógio que está com o número 8 do lado dele. Isso significa que temos 8 versões de história, 8 commits feitos.

Paulo: Não é quantos push, é quantos commit, porque às vezes num push tem mais de um commit. Ainda não fizemos isso, mas poderia acontecer. Clicando aí neste ícone do histórico dá para listarmos todos e ver a história inteira da aplicação. Todas as modificações.

Guilherme: Eu quero fazer algo interessante, eu quero voltar para a sua modificação. Não que a modificação que eu fiz esteja ruim, mas eu quero retornar para o estado do projeto que estava naquele momentodo seu commit.

Paulo: Claro que daria para clicar em um desses, ver como era o arquivo antes, copiar e colar, dar um commit e um push. Você passar por cima. Mas o Git tem mecanismos para você falar: "Por favor, volte para como era na época de determinado commit".

Trabalhar com Git e GitHub não é só para fazer o mesmo que um Dropbox, por exemplo, é muito mais. Ele guarda todas as versões, todos os históricos, você pode ir, pode voltar, ver quem fez, qual o tamanho, se isso estava conectado com aquilo. É realmente feito para trabalhar com muito código. E é muito frequente vermos o histórico dos arquivos, porque se você vê como era antes, começa a entender as modificações que foram feitas. Precisamos ganhar esse hábito, não tenham medo de entrar no GitHub e ver esses históricos.

Guilherme: No GitHub local via linha de comando também temos acesso a essas modificações e vou deixar até um "Para saber mais" explicando como conseguimos visualizar o log, saber a hora, de quem é a autoria daquele commit, etc.

Eu quero visualizar essas mensagens do histórico e voltar o meu projeto para o estado desse commit que o Paulo fez. Então, na linha de comando, para visualizar o log das modificações vou colocar: git log --oneline. Eu quero voltar para o commit "a0c893b console log indicando modificações do Paulo". Então, vou copiar essa sequência de caracteres "a0c893b" que identifica esse commit como sendo único e vou colocar o seguinte comando: git restore.

O git restore vai fazer a gente voltar para um determinado momento da aplicação. Mas preciso indicar para ele qual hash vamos utilizar. Para indicar qual hash vamos utilizar vou colocar --source e vou passar o hash com aqueles caracteres que copiei do commit que o Paulo fez:

git restore --source a0c893bCOPIAR CÓDIGO
Mas ainda tem uma coisa interessante, se eu escrever, por exemplo, app.js, vou pegar esse commit que o Paulo fez naquele momento e vou deixar todo o app.js naquele estado. Mas se o Paulo tivesse feito modificações em diversas partes da minha aplicação e quero voltar a minha aplicação para aquele determinado momento, eu coloco só o ponto(.), esse é o comando que vamos utilizar, vamos inserir o ponto:

git restore --source a0c893b .COPIAR CÓDIGO
Agora sim vou pressionar "Enter" e não recebi nenhuma mensagem diferente. Se eu der um git log --oneline, olha que interessante. Ele vai continuar da mesma forma.

Paulo: Ele restaurou, mas só localmente, ainda não commitamos as mudanças. Agora podemos falar que vamos commitar o arquivo tal, voltando atrás de acordo com determinado commit.

git commit app.js -m "voltando para o estado do paulo"COPIAR CÓDIGO
Agora o git status vai falar que só falta o push. Vamos dar um git status para vermos como está. Está tudo commitado, não tem nada sujo. Nosso repositório local está preparado, mas ele está na frente do original por 1 commit, então você tem que empurrar esse commit para lá. Ou dá até para cancelar o commit se tiver feito algo errado, tem vários comandos, muitas opções para trabalhar com os commits que fizermos. Agora nós queremos empurrar, queremos fazer o push.

Guilherme: Podemos ver no navegador que as modificações que eu havia feito não saíram porque eu voltei ao estado anterior, mas não havia feito um commit. Agora sim fiz o commit, e vou fazer o comando git push.

Agora no navegador, quando atualizamos a página, aquela linha que eu havia feito sumiu, voltamos para o commit que o Paulo havia criado.

@@05
Para saber mais: Git log

Se você deseja verificar o histórico de alterações, as mensagens de commits, o nome do autor daquele commit e outras informações sobre o projeto, existe um comando do git que pode te ajudar. Este comando é o git log.
Como já sabemos, os commits possuem hashs que os identificam de uma forma única, isto é, não existem dois commits com o mesmo hash. Com o git log podemos ver o hash e várias outras informações do commit.

Podemos visualizar todos os commits, um em cada linha com o comando:

git log --onelineCOPIAR CÓDIGO
Se, em vez de menos informações, quisermos ver mais como as alterações do commit, podemos usar:

git log -pCOPIAR CÓDIGO
Também podemos pesquisar as informações do autor daquele commit com o comando:

git log --author="user_name"COPIAR CÓDIGO
E pesquisar informações por data:

git log --since=1.month.ago --until=1.day.agoCOPIAR CÓDIGO
No comando acima, estamos buscando as informações do commit desde um mês atrás até um dia atrás.

Você também pode formatar a visualização das informações de commit com o comando:

git log --pretty="format:%h %s"COPIAR CÓDIGO
Este traz o hash seguido da mensagem de commit. Para saber mais formas de exibir as informações de commit, aqui tem uma lista de maneiras que você pode fazer isso.

Bem legal, não é? E se eu te contar que existem vários outros parâmetros que podemos passar no git log? Se você deseja saber mais sobre como exibir as informações de seus commits, você pode conferir neste link.

https://devhints.io/git-log-format

https://devhints.io/git-log

@@06
Para saber mais: clone do git

Imagine que você esteja trabalhando em um projeto que já está configurado em um repositório de origem, e deseja colaborar com esse projeto. Com o git clone, é possível criar uma cópia de desenvolvimento em um repositório local, e todas as alterações que você fizer serão gerenciadas a partir desse repositório. O comando git clone é usado para selecionar um repositório existente e criar um clone ou uma cópia dele em um repositório local.
O comando git clone cria uma cópia de um repositório git existente, e esse repositório pode ser local ou remoto. Além disso, essa cópia é um repositório git completo, com seu próprio histórico, gerenciamento de seus próprios arquivos e é um ambiente isolado como um todo do repositório original.

Por conveniência, a clonagem cria uma conexão remota apontando para o repositório original. E é essa conexão que facilita muito a interação com o repositório central. Você pode consultar um exemplo demonstrando o git clone aqui!

Com o git clone você também pode clonar o repositório para uma pasta específica:

git clone <repositorio> <meu-projeto-clone>COPIAR CÓDIGO
O repositório localizado em repositorio é clonado para uma pasta chamada meu-projeto-clone.

Você também pode configurar o git clone e clonar o repositório a partir de uma branch específica, diferente da original dessa forma:

git clone -branch new_feature <repositorio>COPIAR CÓDIGO
O exemplo acima clonaria apenas a branch new_feature de repositorio. Outras configurações de opções do git clone você pode consultar neste link.

https://www.atlassian.com/br/git/tutorials/setting-up-a-repository

https://git-scm.com/docs/git-clone

@@07
Faça como eu fiz: comandos do git

Uma pessoa atua como dev front-end e concluiu implementações importantes no desenvolvimento do projeto no qual está trabalhando. Agora, ela precisa verificar as modificações realizadas, adicioná-las ao seu repositório local, salvá-las e depois enviá-las ao repositório remoto utilizando o Git.
Com base nesse contexto, quais comandos do git você pode utilizar para realizar essas ações?

Opinião do instrutor

1 - Para verificar as modificações realizadas:
Utilize o comando git status, ele serve para listar todos os arquivos que foram modificados.
2 - Para adicionar as mudanças ao seu repositório local:

Para adicionar todas as modificações realizadas de uma só vez, é necessário usar git add . (git add e um ponto) e, para adicionar as mudanças em algum arquivo específico, usa-se git add nome-do-arquivo-alterado.
3 - Para salvar as alterações:

Utilize o comando git commit, ele é usado quando queremos capturar e salvar o estado atual do repositório.
4 - Para enviar as modificações ao repositório remoto:

Utilize o comando git push, ele é utilizado para envio das alterações gravadas no diretório local para o repositório remoto.

@@08
O que aprendemos?

Nesta aula:
Entendemos a diferença entre Git e GitHub;
Aprendemos como acessar o histórico de commit de um repositório;
Aplicamos alterações no projeto em um mesmo commit.
Na próxima aula:
Vamos aprender na prática como resolver problemas de issue ao realizar git push!

#### 15/07/2023

@04-Adicionando Arquivos

@@01
Git clone e Git log

Guilherme: Então, essa é a forma que temos para navegar. Vamos fazer uma revisão dos principais comandos?
Começamos com o git clone, clonamos o repositório que tínhamos acesso de colaborador.

Paulo: Público sempre podemos clonar, se fosse privado precisaria estar bem configurado. Além de a pessoa te adicionar no time como o Guilherme fez, você precisa ter aquelas chaves para você configurar.

Guilherme: Depois que fizemos o clone, conseguimos ver o log da nossa aplicação de duas formas, git log mostrando detalhes de quem é o autor, qual a data em que foi feito, ou o git log --oneline, que é o log em apenas uma linha.

Além disso, fizemos o nosso git commit indicando o nome do arquivo que queremos alterar. Podemos até colocar um ponto para pegar o diretório atual e todos de dentro dele: git commit . -m "".

Paulo: Às vezes eu faço. Quem é bom mesmo de Git vai falar para sempre selecionarmos os arquivos exatamente os arquivos que queremos dar commit e suas respectivas mensagens. Geralmente, as pessoas vão acabar usando o ponto e informando qual foi a modificação.

Guilherme: Para enviarmos as nossas modificações: git push. Pegamos tudo o que fizemos e mandamos lá para o repositório.

Paulo: Que pode ser mais de um. Podemos empurrar todos os commits que fizemos lá para o repositório origem.

Guilherme: Esses foram os principais comandos. Meu principal desafio para essa aula é: crie um repositório, crie commits dos seus projetos, coloque seus projetos com versões diferentes, crie mensagens de commits que façam sentido para outras pessoas. Às vezes uma mensagem faz muito sentido para mim, mas outra pessoa pode não entender. As mensagens de commit são importantes. Pratiquem os commits locais. Não vimos muitos comandos até agora, mas vimos os essenciais, você vai utilizar mesmo durante seu dia a dia como pessoa desenvolvedora.

Paulo: Esse é o principal do GitHub, seja web ou via linha de comando do Git. Agora vamos trabalhar com os vários branches, entender melhor o que é esse main, que antigamente até chamava master, quais são as opções de podermos trabalhar em paralelo com duas versões e juntar tudo lá no final, o tal do merge. transformaremos em branches (galhos) e depois fazemos os merges. Isso é muito frequente, na web vai ficar mais visível quando tiver esses caminhos.

Também veremos o comando git add. Se queremos adicionar um arquivo novo não basta fazer commit, temos que informar que o arquivo novo faz parte do diretório. Veremos mais alguns comandos que são muito importantes.

Tem milhares de comando. Neste curso estamos passando aqueles que são vitais para você trabalhar no seu dia a dia. O Guilherme que manja mais é que vai dar essa parte do curso. E eu volto para finalizar e dar dicas e desafios para você. Chegou nesse momento, você precisa fazer exercícios, precisa praticar.

@@02
Navegando no tempo

Você fez quatro commits em seu código HTML: Adicionando Title, Adicionando imagem de fundo, Adicionando tabela e Adicionando footer, mas os três últimos commits não foram aprovados por seu supervisor. Então, você precisa voltar ao ponto inicial do projeto. Qual o comando que você precisa utilizar para navegar no passado?
Com base no que vimos em aula, analise as alternativas abaixo e marque apenas a correta:

Usamos o comando restore para voltar exatamente ao ponto que inicial do projeto.
 
Alternativa correta! Usamos o comando Restore informando o ID do primeiro commit depois da flag --source. Te convido a ler mais sobre Restore nesse artigo da Alura.
Alternativa correta
Não é possível voltar tanto assim em projeto depois de vários commits.
 
Alternativa correta
Usamos o comando checkout para voltarmos ao ponto que queremos.

@@03
Git add

Quando acessamos determinada aplicação, por exemplo, a página da Alura ou página dos filmes mais votados da Netflix, algo desse tipo. Existem diversas páginas dentro desse mesmo projeto. Agora eu quero criar uma página nova, por exemplo, de contato.
Vou criar um novo arquivo chamado contato.html. Para inserir automaticamente a estrutura do HTML vou inserir um sinal de exclamação e pressionar "Enter". O título da página será contato: <title>Contato</title>. Também vou deixar o idioma como português <html lang ="pt-br"> e inserir um h1 no body de <h1>Contato</h1>.

Vamos supor que eu desenvolvi essa página e tudo ficou legal. Agora vamos usar o nosso terminal, se eu dou aqui um git status e dou "Enter", observe o que aconteceu.

Ele falou que existem modificações no app.js e existe aqui uma página de contato. Então, se eu tenho mais de uma modificação para adicionar, geralmente o que eu faço? Faço um git add, e passo o nome do arquivo que quero adicionar: git add app.js.

Agora que já adicionamos o app.js para as modificações dele serem "escutadas", vou usar o commit e passar uma mensagem de commit:

git commit app.js -m "corrigindo o app js"COPIAR CÓDIGO
Vou dar "Enter" e ele colocou essa modificação. Se eu dou um git push para ele enviar essas modificações para o nosso repositório, a partir do momento que eu atualizar, observe que ele vai mostrar a atualização que eu fiz.

Mas aquele nosso contato.html não apareceu, essa página não está sendo vista pelo GitHub. Porque fizemos o commit e adicionamos as modificações apenas do app.js. Vamos supor que criemos várias páginas para um site, será que precisaríamos colocar git add e o nome de todas as páginas? E o mesmo para os outros arquivos JavaScript e arquivos CSS que criarmos?

Não. Nós podemos usar apenas um comando git addadicionando um ponto (.): git add . Assim, como o Paulo falou, e temos que tomar bastante cuidado com isso, todas as modificações que fizermos no nosso repositório, na raíz do nosso projeto e nas outras pastas, elas serão "ouvidas" quando usarmos o ponto.

Vou fazer então, um git git add . e, em seguida, farei um commit: git commit -m "criando a página de contato". Dou um git push, e agora no site do GitHub já temos a atualização com a nossa página de contato

Não podemos esquecer que para que o Git consiga analisar quais arquivos estão sendo criados e as modificações que fizemos nesse arquivo, é importante pensarmos no git add para colocar arquivos novos para serem vistos pelo GitHub.

Vocês viram que eu havia feito modificações no app.js e no arquivo de contato. Mas quando adicionei o commit e fiz o push, só o app.js que foi para o repositório. Se quero que a página de contatos também apareça, é necessário incluir essa página também.

Recapitulando: para incluir só uma página podemos usar git add + nome da página, nesse caso:

git add contato.htmlCOPIAR CÓDIGO
Se tenho diversas páginas e modificações, e quero adicionar todas essas modificações no repositório para versionamento utilizo o ponto:

git add .

@@04
Para saber mais: Open Source

Você sabe o que é Open Source?
Open Source é um código projetado para ser acessado abertamente por qualquer pessoa, que pode ver, modificar e distribuir conforme suas demandas.

Você pode ver mais detalhes nesse artigo do Bruno Divino.

https://www.alura.com.br/artigos/open-source-uma-breve-introducao?_gl=1*1vjz3xf*_ga*MTgwMzIzMjk2Ni4xNjg4ODE5OTcz*_ga_59FP0KYKSM*MTY4OTQ1NjQ5Mi4xNC4xLjE2ODk0NTcxNjguMC4wLjA.*_fplc*eUM3ck9VJTJCJTJGZVNoVUViZmFDMkZQdVc5a0t2JTJGY1lBV3pBNmZkR1h5N0VaSFpaNk9OeCUyRlRjMmNkWHJTJTJCY2I0JTJGdlczJTJGeVhoeEROajM4ZDBHc1A0NEJvb1EwcFNxdm1nNnFWWU80S0QyZnVSNjRuTEJ6VCUyRkpVT3NkV3gyOVQ2ZyUzRCUzRA..

@@05
Faça como eu fiz

Chegou a hora de você seguir todos os passos realizados por mim durante esta aula. Caso já tenha feito, excelente. Se ainda não, é importante que você execute o que foi visto nos vídeos para poder continuar com a próxima aula.

Opinião do instrutor
Continue com os seus estudos, e se houver dúvidas, não hesite em recorrer ao nosso fórum!

06
O que aprendemos?

Nesta aula:
git restore
Aprendemos a trabalhar com essa parte de restauração de arquivos e do projeto, voltando para um estado anterior através do git restore;
git add
Aprendemos a adicionar os arquivos que queremos para o próximo commit através do git add.

#### 16/07/2023

@05-Ramificacoes e Merge

@@01
Branch

Durante todo o desenvolvimento desse curso, sempre utilizamos o main, que é o nosso projeto principal, um projeto que buscamos que não tenha erros e falhas.
O que acontece, geralmente, quando vamos trabalhar em um cenário que tem mais de uma pessoa trabalhando no projeto é que existe o código principal, o main, antigamente era chamado de master e existem outras ramificações.

Tem o local que é o código principal e um outro local que é o código de desenvolvimento ou o que estamos trabalhando especificamente. Por exemplo, poderíamos criar aqui duas branches - considere "branches" como ramificações da nossa aplicação - então vamos ter a nossa branch principal, que é a nossa main, e quero criar mais uma branch, uma branch de desenvolvimento.

Nessa branch de desenvolvimento vou criar alguns códigos, fazer algumas coisas e depois quero mostrar para vocês, por exemplo, se isso já estiver validade, já passou em diversos tipos de testes, eu quero mandar isso que estava na branch de desenvolvimento para a branch main.

Assim garantimos que o nosso código main vai funcionar corretamente e, ao mesmo tempo, estaremos trabalhando em versões diferentes da nossa aplicação sem quebrar o nosso código principal.

Vamos lá, como criar uma branch diferente? No terminal, vamos colocar o comando git checkout, -bpara criar a branch e chamarei essa branch de "desenvolvimento":

git checkout -b desenvolvimentoCOPIAR CÓDIGO
Quando pressiono "Enter" ele cria a branch de desenvolvimento e estou nela agora. Se você quiser voltar para a branch principal pode usar o comando git switch main. E para voltar para a branch de desenvolvimento: git switch desenvolvimento.

Agora tenho duas branches. Se eu for no GitHub e atualizar a aplicação, ele vai mostrar só a branch main porque eu ainda não fiz nada com a branch de desenvolvimento. Vamos fazer uma alteração na branch de desenvolvimento?

No VS Code, aqui na minha página contato.html eu vou criar um parágrafo: <p> Entre em contato pelo email gui@alura.com</p>. Agora que terminei de editar a minha página de contatos, quero pegar essas modificações da página de contato, adicionar, criar um novo commit e mandar essas modificações para a branch de desenvolvimento.

Vou abrir o terminal e fazer o comando git add contato.html, ou git add ., ambos os códigos dariam certo. Vou fazer o commit: git commit -m "adicionando email de contato".

Fiz um git add e um git commit, agora falta fazer um push para a nossa branch de desenvolvimento. Eu quero mandar para determinada origem, qual é essa origem? A origem de desenvolvimento:

git push origin desenvolvimentoCOPIAR CÓDIGO
Pressiono "Enter" e ele vai enviar para a branch de desenvolvimento. Ao voltar para o site do GitHub ele informará que temos uma nova branch criada no projeto.

Se eu for na branch principal, a main, a atualização que eu fiz no contato.html com o "Entre em contato pelo email gui@alura.com" não estará presente na main. Então, nós criamos um local específico chamado "desenvolvimento" onde iremos realmente trabalhar no nosso projeto, testar e validar coisas.

Depois que fizemos todo o trabalho na branch de desenvolvimento, o código está ok, tudo funcionando como esperamos, e já podemos subir o código para a branch principal, como fazer para pegar o que está em desenvolvimento e mandar para a nossa branch principal? É isso que aprenderemos no próximo vídeo.

