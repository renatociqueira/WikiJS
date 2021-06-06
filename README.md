## Documentação Projeto WikiJS

Processo de instalação e implantação do **WikiJS** juntamente com **Docker** e **Postegres**.

## Requisitos

Neste Documento o processo é feito no **Windows 10 Pro X64** caso o processo seja feito em outro SO consultar nas documentações do seu sistema possiveis comandos que vamos precisar utilizar no **Prompt** ou no terminal que seu SO utilizar.

Precisamos ter o **Docker** Instalado na Maquina, caso não tenha consultar a documentação segue um link para estudo.
[instalação do Docker no Windows](https://docs.docker.com/docker-for-windows/install/).

Faz-se necessario ter privilegios de administrador ou permissões para instala e executar os arquivos aqui mencionados que será o **Prompt**,**docker.exe**, e **criação de pasta e arquivos**.

**Opcional**

Caso queira poderá está utilizando o atom para criação dos arquivos ou poderá utilizar algum editor de texto do seu interesse, para criar os arquivos e salva-los com a extensão **yml**, foi utilizado o atom nesta atividade para facilitar a digitação de código e envio para o Github, irei deixar aqui também um link caso queira baixar e utilizar o mesmo.
[Atom](https://atom.io/).

## Documentação do WikiJS

Consultar Documento para Criar Arquivo Docker-compose.
[Documento WikiJS](https://docs.requarks.io/install/docker)

Em Sua maquina crie uma pasta para o projeto e coloque o nome que preferir irei colocar minha pasta com o nome de **WikiJS**, neste processo irei criar no caminho a seguir mais poderá está escolhendo o caminho que tiver permissões e que melhor atenda sua necessidade.
C:\Users\usuariodamaquina\Documents\GitHub\WikiJS

Dentro da pasta WikiJS será criado um arquivo com o nome de **compose.yml** neste arquivo você irá colar o código do docker compose que está na documentação
Link: [Documentação](https://docs.requarks.io/install/docker).

Feito a criação do arquivo e colado o código do docker compose mude no código a porta na qual o http do wiki irá funcionar no meu caso coloquei em **ports** a porta 8080, salve o arquivo.

Após este processo precisamos que abra o Prompt como administrador, para isso entre no menu iniciar do seu sistema windows 10, digite prompt clique com o botão direito do mouse e clique na opção de executar como administrador, caso apareça uma janela pedindo permissões clique em sim, e o prompt será aberto.

Geralmente por padrão o prompt vai abrir no seguinte caminho C:\WINDOWS\system32> para sair dele e ir para a pasta do projeto digite.
cd \Users\usuariodamaquina\Documents\GitHub\WikiJS
e aperte enter você vai entrar na pasta do projeto lembrando que esse caminho foi onde salvei o arquivo compose.yml verifique o seu caminho e utilize ele.

Após entrar no caminho especificado digite dir e aperte o enter para ver se seu arquivo aparece.

caso apareça agora é hora de verificar se o docker está rodando, caso não esteja execute o docker no windows para ele funcionar e podermos subir o conteiner, caso ja esteja funcionando o docker volte para o prompt no caminho especificado do projeto e digite **docker-compose up** este comando vai subir a imagem do postegres e do wiki juntamente com o conteiner.

Acesse localhost:8080 e terá acesso ao WikiJS e poderá finalizar o resto da instalação do mesmo.

## Utilizados

|WINDOWS 10 pro    |X64        |
|------------------|-----------|
|Docker            |v20.10.6   |
|Atom              |v1.57.0    |
|Prompt            |x64        |

## Comandos Usados

|Prompt            |Função                                         |
|------------------|-----------------------------------------------|
|Docker ps         |consulta os conteiners                         |
|Docker ps -a      |consulta os conteiners inclusive os desligados |
|Docker-compose up |sobe o conteiner e imagens                     |  
|Docker start      |inicia o conteiner informando o ID             |
|Docker stop       |para o conteiner informando o ID               |
|cd                |entra nas pastas                               |
|dir               |consulta os arquivos que tem dentro da pasta   |
