Hello World

Fala as coisas para mim ^^

Feramentas que foram aprendidas / a sua função:
$ git config --global user.name "Adriano Serafim" / Serve para indentificar ao programa quem você é. Isso tem como objetivo identificar quem está fazendo as alterações. Isso tem que ser definido todas as vezes que você vai salvar as configurações de um projeto.

$ git config --global user.email "adriano_serafim_1@hotmail.com" / Serve para deixar um e-mail de viculo para caso queira entrar em contato ou sauvar na luvem no nome dessa pessoa. Isso tem que ser definido todas as vezes que você vai salvar as configurações de um projeto.

$ git config --global core.editor (O seu editor) (ex: suble, emacs, vim) / Serve para você definir em qual tipo de linguagem de programação você está falando, pois apesar de ser parrecido as liguagem de programação de cada programa é diferente.

$ git init / Cria um arquivo na pasta onde você está. Vale lembrar que ele vai usar o modelo do arquivo escolhido a cima. Normalmente não é utilizado.

$ git config user.name & $ git config user.email & $ git config --list / Esse dois cód. vão te mostrar qual é o nome e o e-mail que estão sendo utilizados.

$ mkdir (Nome da pasta) / É o comando  de criar pasta em um determinado local.

$ cd (Nome da pasta) (Isso é do sistema Windows) & $ dir (Nome da pasta) (Isso é do sistema MacOS) / Abre a pasta ou arquivo que você quer. Uma pasta ou arquivo por vez.

$ cd (O nome do arquivo) (Não pode esquecer do tipo do arquivo. Como por exemplo esse arquivo é .txt) /  É a mesma coisa do de cima... só escrevi de novo para mostrar mais informações e não deixar mauito confuso.

$ cd .. / Volta uma pasta ou arquivo.

$ vim (Nome do arquivo) / Serve para abrir e editar o arquivo dentro do git. Isso normalmente não é muito utilizado pois como cada liguagem tem a sua peculiaridade é muito fácil que ocorra erro de sintaxe.

	A partir de agora esses comandos é para quando você esta dentro do arquivo o editando.
	Caso você click na letra i você a poder editar o arquivo, caso você click em esc ele sai do modo de edição, caso você click em Stick (Cetinha para cima) e a tecla ; o programa vai entender que você quer incerir um comando, caso você click em w e enter após clicar em Stick e ; o programa vai entender que você quer modificar o arquivo com o que você encreveu, caso você click em q e enter após clicar em Stick e ; o programa vai entender que você quer fechar e sair da edição de arquivo, você pode usar o comando w e q juntos fazendo com que ele salve e saia do arquivo.
	A partir de agora nos voltamos a os comando utilizados fora do editor de arquivos.

Explicação do git: O git tem 4 estados
	Untracked: São arquivos que não estão no git.
	Unmodified: São  arquivos que não tem modificações para salvar
	Modified: São arquivos que tem modificação para salvar
	Staged: Área onde é criada uma versão de modificação do arquivo, após dar um commit no arquivo ele volta ao estatos Unmodified eo git salva o utimo Staged para caso você queira voltar nele algum momento.

$ ls -la / Ele fala o histórico de edção que ocorreu na pasta

$ ls / Vai te falar quais são os arquivos que estão naquela pasta que estão sendo vistos pelo git.

$ git status / Serve para ver os status dos aquivos no git na quela pasta.

$ git add (Nome do arquivo) (Não pode esquecer do tipo do arquivo. Como por exemplo esse arquivo é .txt) / Serve para adicionar o arquivo a o git, tirano ele do estado Untracked e colocando ele no estado Unmodified. Esse comando tambem serve para tirar o arquivo do Modified para Staged, sendo assim ele esta salvando uma cópia de versão desse arquivo sempre que você o faz.

$ git commit -m "(Descrição de edição)" / Você so pode fazer commit nos arquivos que estão no estado Staged e sempre é bom colocar uma descrião, pois assim que você vai identificar em qual versão você quer estar. Após o commit o git te dar a uma chave de versão, para você visualizar que versão você acabou de fazer. Você pode colocar cometarios adicionais no commit acrecentando -m "(Comentario adicional)", porem muitos comando so deixão ser visualizados a descrião e não mostram que há comentario adicional. Caso você vai dar commit em um arquivo que já tinha sido sofrido um commit antes você pode -am "(Descrição de edição)" fazendo isso você não preciza fazer a adição da modificação " no cado seria $ git add"

$ git log / Serve para ver o historico de commit daquala pasta. Esse código pode ser inclementado com algumas configurações a mais que iram nos dar inforamções importantes do arquivo. Tipo --decorate que ira nos dar o estatos de branch do arquivo, --author "(Nome do Autor a ser procurado, ou no minimo as iniciais)", --graph que ira mostrar de forma gráfica como esta os commit's realizados.

$ git shortlog / Mostrar em ordem alfabética os altorer que fizeram commit, quantas vezes eles fizeram o commit e em qual arquivo foi feito o commit, e qual a descrição dos commit's. Você pode colocar no código -sn que ira mostrar um lista de pessoas que fizeram commit e quantos commit aquela pessoa realizou.

$ git show (Chave do commit) / Mostra com detalhes a modificação que causou esse commit no arquivo.

$ git diff / Mostra a diferenças entre os arquivos Unmodified com o arquivos Modified. Você pode colocar no código --name-only que lista para você o nome dos aquivos que estão no estados Modified.

$ git checkout (Nome do arquivo) (Não pode esquecer do tipo do arquivo. Como por exemplo esse arquivo é .txt) / Retorna o arquivo do Modified para Unmodified deletando assim toda a edição feita.

$ git reset HEAD (Nome do arquivo) (Não pode esquecer do tipo do arquivo. Como por exemplo esse arquivo é .txt) / Retorna o arquivo do Staged para Modified possibilitando que você possa adicionar novas mudanças antes do commit que você quer fazer.

$ git reset (Escolha entre os três tipos --soft, --mixed, --hard)
	--soft (Chave do commit) / Ele volta o arquivo para o estado Staged da chave em questão. Sendo assim normalmente você sempre olha para qual arquivo você quer voltar e pega uma chave anterior.
	--mixed (Chave do commit) / Ele volta o arquivo para o estado Modified da chave em questão. Assim facilita para você na hora de fazer as alterções.
	--hard (Chave do commit) / Ele volta o arquivo para o estado Unmodified da chave em questão.
OBS: Tome cuidado com o essa ferramenta, pois a utilizando você mata o histórico dos commit entre o ultimo commit realizado e o commit que esta voltando. E tambem  você pode ter problemas ao subir os arquivos gando já teve pessoas que fizeram alterações na auterações dele, nesse caso você vai ter que utilizar a ferramemta fort.

Exercício pratico de reset - Feito ^^

Apartir de agora nos vamos colocar os aquivos no repositório remoto. Para fazer isso primeiro temos que criar um repositório remoto. Isso é facil de criar é só clicar no botão "New repository" no github e colocar o nome para ele. Lá ira perguntar se você quer deixar o seu repositório publico ou privado e também ira perguntar se você quer deixar os aquivos 100% onlines... apos decidir o que você quer é só clicar em criar repositório "Create repository".

Essa parte tem que fazer um vez por maquina utilizada.
	Agora vamos criar uma chave SSH para o github saber que os aquivos mandados desse computador é você e colocar na sua pasta. A descrição para a criação da chave está no site de ajuda do github (https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent), apos a criação você tem que visualizar a chave no programa e a colocar nas configuração do github na internete.

Feito isso agora irei mostrar alguns comando relacionados ao assunto e irei dar contunuidade ao conteudo.

$ cd ~/.ssh/ (Utilize onde estivar a pasta onde a chave está) / Isso ira abrir a pasta donde está localizado a pasta, essa pasta é oculta. Caso você de o comando "$ ls" apos esse comando, ele ira mostrar as chaves dentro da pasta. 

$ cat (O nome da chave que você quer utilizar).pub & $ more (O nome da chave que você quer utilizar).pub & $ vi (O nome da chave que você quer utilizar).pub (Lembrando que a chave que deve ser utilizada é o arquivo com o dominio .pub) / Isso abre o arquivo e mostra o código da chave que você que copiar para incerir na configuração do github.

$ git remote add (Nome do repositorio que ira ser enviado) / Serve para definir em qual repositório você está enviando os arquivos.

$ git remote / Ira mostrar qual são os repositórios linkados. Caso você coloque  na frente do código "-v" ele ira mostrar mais informações sobre o repositório.

$ git branch -M main / Não sei ao serto o que faz, mas acredito eu que ele define o branch que eu estou como o branch main

$ git push -u (Nome do repositório) (Nome do branch) / Ira mandar os arquivos que sofrerão commit para o repositório. O "-u" no código é uma criação de atalho, assim na proxima vez que você for colocar no repositório remoto não precisara digitar o nome do repositorio, isso quer dizer que esse parte pode ser tirada do código (exemplo: $ git push origin main).

$ git clone (Chave de clonagem que o github fornece) (nome da pasta que sera baixado os arquivos) / Ira clonar para você os arquivos do repositório que você deseja no github.


$ git checkout -b (Nome do branch) / Cria um novo branch (Ponto de referência do arquivos), o branch padrão sempre anda junto com o commit, mas é possivel criar vairos pontos de referencia e juntar eles no final. Há duas maneiras de juntar os branch, elas são Merge e Rebase:
	Merge une os branch criando um novo commit na linha de histórico, além de deixar visivel a derivação do branch no histórico.
	Rebase une o branch colocando o seu último commit na frente da linha de histórica do arquivo. Isso faz com que o historico do branch sejá apagado, mas deixa o histórico linear, tornando assim o histórico menos poluído

$ git branch / Mostras os branch e mostra com um asterisco na frente o branch que você está.

$ git checkout (Nome do branch) / Moda para o branch que você quer.

$ git branch -D (Nome do branch) / Exclui branch criados.

