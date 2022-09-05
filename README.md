
<h1 align="center"> Competição SS2D </h1>

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
![GitHub Org's stars](https://img.shields.io/github/stars/ras-ufcg/SS2D?style=for-the-badge&logo=github)
    

| Nosso Projeto | Primeiros Passos |Aprendendo Mais|
| ---------------- | ---------------- |------------- |
| 🤖[**SS2D**](#-competição-ss2d) |🛠[**Instalação Server+Monitor**](#-instalando-o-servidor-e-monitor) |📖[**Material Extra**](#-aprendendo-mais) |
| 🧑‍🎓[**Equipe**](#-equipe) |📼[**Assistir um Jogo Gravado**](#-rodando-um-jogo-gravado) |🗂️ [**Acesso ao Projeto**](#-acesso-ao-projeto) |
| 📄[**Metodologia**](#-metodologia) |🛠[**Instalação de Equipes**](#-instalando-as-equipes) |💻[**Criando um Binário**](#-criando-um-binário) |
| 🗓[**Planejamento**](#-planejamento) |🎮[**Rodando o Primeiro Jogo**](#-primeira-partida) | 🕹️[**Modo de Controle Manual**](#-controlando-um-robô) |


<!---## Sumário
- Sobre o Projeto
    - 🤖[**SS2D**](#-Competição-SS2D) 
    - 🧑‍🎓[**Equipe**](#-equipe)
    - 📄[**Metodologia**](#-metodologia)
    - 🗓[**Planejamento**](#-planejamento) 
- Primeiros Passos
    - 🛠[**Instalação Server+Monitor**](#-instalando-o-servidor-e-monitor)
    - 🛠[**Instalação de Equipes**](#-instalando-as-equipes)
    - 🎮[**Rodando o Primeiro Jogo**](#-primeira-partida) 
- Apredendo Mais
    - 📖[**Material Extra**](#-aprender-mais)
    - 🗂️ [**Acesso ao Projeto**](#-acesso-ao-projeto)
    - 💻[**Criando um Binário**](#-criando-um-binário)
    - 🕹️[**Modo de Controle Manual**](#-controlando-um-robô) -->
## 🤖 Competição SS2D?
- A Robocup é uma competição anual internacional de robótica estabelecida em 1996, que objetiva promover pesquisas de robótica e de inteligência artificial através de torneios de várias modalidades.
- A [SS2D](https://en.wikipedia.org/wiki/RoboCup_2D_Soccer_Simulation_League) é a modalidade da Robocup que aborda o futebol simulado por computador num espaço 2D. 
- Cada time tem 11 jogadores virtuais que "pensam" separadamente e tomam decisões com base nas informações que conseguem capturar do seu ambiente. 
- Os jogadores têm atributos como velocidade máxima, precisão de chute, tamanho e energia. Esses atributos são escolhidos aleatoriamente pelo servidor em cada partida. 
- Os algoritmos e lógicas que cada jogador usa para decidir o que ele vai fazer devem ser criados pela equipe do time. Porém, é permitido e recomendado que equipes novas utilizem o código de outras equipes como base.
- As regras das partidas do SS2D são extremamente parecidas com as que conhecemos no futebol: Existem faltas, impedimentos, tiros de meta, cartões, entre outros. Ganha a partida o time que fizer mais gols.

## 📄 Metodologia
Para uma melhor divisão das tarefas, o projeto pode ser dividido em duas áreas de foco:
- Microdinâmica - Responsável por decisões de baixo nível, pelo desenvolvimento das heurísticas, inteligência artificial e tomada de decisões de cada um dos jogadores. Área mais focada em detalhes de controle, como: Dribles, Fazer o robô chutar com a força certa ao fazer o passe, interceptação, ETC.
- Macrodinâmica - Responsável por decisões de alto nível, pelo desenvolvimento de estratégias, formações e modo de jogo geral do time. A área engloba: Comparação e escolha de formações a cada ponto do jogo, jogadas "ensaiadas", economia de energia, ETC.

## 🗓 Planejamento

- No primeiro instante foi realizada uma introdução geral acerca da competição e das equipes. Para isso foi feito o estudo e a leitura dos [TDP's](http://archive.robocup.info/Soccer/Simulation/2D/TDPs/RoboCup/) disponibilizados pelas equipes tanto internacionais como nacionais. Neste estudo foi possível captar aspectos importantes da competição, como por exemplo seu funcionamento, como as equipes e como o jogo funciona. Também com a leitura foi possível perceber estratégias de algumas equipes, como por exemplo o uso de inteligência artificial, o uso de diferentes marcações e etc. Além dos TDP’s disponibilizados pelas equipes, também foi e está sendo utilizado o manual, [The RoboCup Soccer Simulator Users Manual](https://rcsoccersim.readthedocs.io/en/latest/).
- No momento a equipe busca ter os primeiros contatos com os softwares, as equipes bases e criar um time com apenas um jogador, para assim poder compreender a dinâmica do jogo na prática e poder criar um time que possa participar de competiçoẽs.


**Status do projeto**

| # | Atividade | Status |
| ---------------- | ---------------- |------------- |
| 1 | Compreender a Competição SS2D - Leitura de TDP's |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 2 | Instalação do Servidor e do Monitor |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 3 | Instalação dos Times Base e Rodar Partidas |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 4 | Realizar o controle Manual de um Dummy |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 5 | Criação de um Time Com Apenas um Cliente | <img alt="Em Andamento" src="https://img.shields.io/badge/-Em%20andamento-orange">|
| 6 | Criação de uma Estratégia Própria | <img alt="Não Iniciado" src="https://img.shields.io/badge/-Não%20iniciado-red">|
    

## 🛠 Instalando o Servidor e Monitor
- Recomenda-se usar o Ubuntu 16.04 ou uma versão posterior para rodar os programas da modalidade. No Ubuntu, é possível instalar todos os requisitos de ambiente com os seguintes comandos:
```
sudo apt update
sudo apt install build-essential automake autoconf libtool flex bison libboost-all-dev
sudo apt install build-essential qt5-default libfontconfig1-dev libaudio-dev libxt-dev libglib2.0-dev libxi-dev libxrender-dev
```

- Servidor:

    Antes de continuar é recomendado criar uma pasta /servidor/ , dentro da qual você salvará tanto o servidor quanto o monitor.

    No [Github do servidor](https://github.com/rcsoccersim/rcssserver/releases), baixe a versão mais recente do _rcssserver-x.x.x.tar.gz_,  substituindo os "x" pelo número da versão. Em seguida, execute os seguintes comandos no terminal, substituindo o nome do arquivo para que fique igual à versão instalada:
    ```
    tar xzvfp rcssserver-x.x.x.tar.gz
    cd rcssserver-x.x.x
    ./configure
    make
    ```

    A partir de agora, você poderá executar o binário ./rcssserver dentro do /src/ do servidor para fazer o servidor funcionar. Porém, mesmo executando esse comando, não será possivel ver o campo nem qualquer jogo que for executado, pois o monitor ainda não está instalado.

- Monitor:

    Dentro da pasta /servidor/ que você criou, baixe [a versão mais recente do monitor](https://github.com/rcsoccersim/rcssmonitor/releases) e execute os seguintes códigos, substituindo o nome do arquivo pelo nome correto:
    ```
    tar xzvfp rcssmonitor-x.x.x.tar.gz
    cd rcssmonitor-x.x.x
    ./configure
    make
    ```

    Agora você pode rodar o binário ./rcssmonitor dentro do /src/ do monitor para fazer o monitor funcionar.

    Lembre-se de rodar o servidor sempre antes do monitor. Você saberá que tudo está funcionando se os jogadores aparecerem no monitor na parte superior, logo fora da quadra, como na imagem:



## 📼 Rodando um Jogo Gravado
A execução de um jogo gravado é um processo muito simples que permite testar se o monitor está funcionando corretamente.
- Em primeiro lugar, baixe o replay do jogo gravado. Existe uma coleção de replays de todas as partidas da Robocup desde 2004 no [site de arquivo da competição](http://archive.robocup.info/Soccer/Simulation/2D/replays/RoboCup/). É recomendado que você crie um diretório para salvar os replays do SS2D.
- Depois disso, copie o caminho do replay baixado na sua máquina. Para isso, você pode clicar com o botão direito no arquivo baixado e selecionar "propriedades". Nas propriedades está exibida a "pasta-mãe" do arquivo. Copie essa pasta-mãe para sua área de transferência.
- Na pasta /src/ do rcssmonitor, execute o comando: 
	./rcssmonitor pastacopiada/nomedoreplay
Substituindo o "pastacopiada" pelo endereço que você copiou e "nomedoreplay" pelo nome do arquivo de replay que você baixou. 
- Pronto! Se tudo tiver dado certo, irá aparecer uma janela do rcssmonitor com botões de controle no canto superior da tela, como pausar e iniciar, mudar a velocidade e ir para o próximo frame.


## 🛠 Instalando as Equipes
- A princípio estão sendo usadas as seguintes equipes como base:
    - [Helios Base 2D](https://github.com/helios-base/helios-base)
    - [Cyrus Base 2D](https://github.com/Cyrus2D/Cyrus2DBase)
- Para a instalação dos times bases será necessário ter as seguintes bibliotecas:
    - [Boost 1.38 ou posterior](https://www.boost.org/)
        ```
        sudo apt update
        sudo apt install build-essential libboost-all-dev
        ```
    - A última [librcsc](https://github.com/helios-base/librcsc)
    - [Eigen3](https://eigen.tuxfamily.org/dox/index.html)
        ```
        sudo apt-get update
        sudo apt-get install libeigen3-dev
        ```
- Para finalizar a instalação da equipe [Cyrus Base 2D](https://github.com/Cyrus2D/Cyrus2DBase) se faz necessário a inclusão de uma pasta chamada [CppDNN](https://github.com/Cyrus2D/CppDNN) na pasta clonada do git da equipe. Da seguinte forma:

<p align="center">
  <img src="https://ik.imagekit.io/6774657672/1_oLAH42qxh.jpeg?ik-sdk-version=javascript-1.4.3&updatedAt=1662309728387" width="900" >
</p>

- Dentro da pasta CppDNN deverá ter os seguintes arquivos:

<p align="center">
  <img src="https://ik.imagekit.io/6774657672/2_2VeOa8ytJ.jpeg?ik-sdk-version=javascript-1.4.3&updatedAt=1662309728387" width="900" >
</p>

- Dentro da pasta CppDNN/src deverá ter os seguintes arquivos:

<p align="center">
  <img src="https://ik.imagekit.io/6774657672/3_BbTvKLbga.jpeg?ik-sdk-version=javascript-1.4.3&updatedAt=1662309728386" width="900" >
</p>

- Finalizado as instalações das dependências das equipes, deve-se agora seguir o seguinte procedimento para cada umas das equipes:

    - Para construir binários, execute comandos da raiz do diretório de origem:
        ```
        ./bootstrap
        ./configure
        make
        ```

## 🎮 Primeira Partida
Depois que tudo estiver instalado, você deve seguir essa sequência de passos para simular sua primeira partida:

- Abra 4 janelas de terminal.
- No 1° terminal, entre na pasta /servidor/rcssserver-x.x.x/src/ e rode ./rcssserver
- No 2° terminal, entre na pasta /servidor/rcssmonitor-x.x.x/src/ e rode ./rcssmonitor
- No 3° terminal, rode o ./start.sh do primeiro time;
- No 4° terminal, rode o ./start.sh do segundo time;
- Dentro da janela que o monitor abriu, libere o kickoff com o comando Ctrl-K.

Espere alguns segundos entre cada passo para diminuir a chance de erros.

## 📖 Aprendendo Mais
Softwares oficiais:
- [Servidor](https://github.com/rcsoccersim/rcssserver)
- [Monitor](https://github.com/rcsoccersim/rcssmonitor)

[Site oficial](https://robocup.org/leagues/23)
[Página da Wikipedia](https://en.wikipedia.org/wiki/RoboCup_2D_Soccer_Simulation_League)

[Arquivo dos Replays](https://archive.robocup.info/Soccer/Simulation/2D/replays/)

TDPs:
- [tdp.robocup](https://tdp.robocup.org/tdp/)
- [Arquivo de TDPs](http://archive.robocup.info/Soccer/Simulation/2D/TDPs/RoboCup/)

Tutoriais:
- [Documentação Oficial](https://rcsoccersim.readthedocs.io/en/latest/)
- [Tutorial não-oficial](https://github.com/herodrigues/robocup2d-tutorial)
- [Tutorial de como fazer o binário do time](https://www.youtube.com/watch?v=eQwX2p5CNFI&list=PLFy1-QjBONFL_yjjOOh6brRJgZMfLyBbw)

Equipes:
- [RoboCIn](https://robocin.com.br/publicacoes.html)
- [ITAndroids](https://bitbucket.org/itandroids/itandroids-soccer2d/wiki/_oldHome)

Times base:
- [HELIOS](https://github.com/helios-base/helios-base)
- [CYRUS](https://github.com/Cyrus2D/Cyrus2DBase)
- [Gliders](http://www.prokopenko.net/gliders2d.html)

Leituras sobre Inteligência Artificial:
- [Análise sobre aprendizado de reforço na SS2D](https://www.cin.ufpe.br/~tg/2019-2/TG_EC/Evaluating_Reinforcement_Learning_on_Robocup_Soccer_Simulation_2D%20.pdf)

## 🗂 Acesso ao Projeto
- Para ter acesso ao projeto vá na pasta disponibilizada Equipe-RAS. Caso o que procura não esteja presente neste Git, entre em contato com a equipe. Estamos à sua disposição.

## ‍💻 Criando um Binário
- Para fazer um binário crie, em primeiro lugar, uma cópia da pasta _src_ do seu time. Essa cópia será transformada no "Binário", ou seja, a pasta com o mínimo necessário de arquivos para fazer um time funcionar. 
- Renomeie a pasta cópia que você criou para o nome de seu time. Dentro dela, acesse o arquivo _start.sh_ e mude a variável _teamname_ na linha 26 para o nome desejado do time. Isso fará com que o servidor trate o seu time pelo nome escolhido. 
- Em seguida, você pode deletar todos os arquivos com quaisquer dessas terminações: _.o .h .cpp .in .am_. Para facilitar use o seguinte comando shell no terminal, dentro da pasta:

```
rm *.o *.h *.cpp *.in *.am
```

- Por via de regra, além das pastas, apenas os arquivos _coach.conf, player.conf, sample_coach, sample_player_ e _start.sh_ precisam permanecer no seu binário.
- Com isso, o seu binário está pronto. Para inserir o time no jogo é só usar a função _.\\start.sh_ .

## 🕹 Controlando um Robô
- Para iniciar o simulador (servidor e monitor), digite:

```
rcsoccersim
```
- Para iniciar o cliente de amostra, digite ./rcssclient ou rcssclient. Em seguida, digite (init sample). Isso conectará o cliente de amostra ao servidor. Você pode então digitar o comando do cliente para mover o cliente pelo campo. Você também precisará de um monitor para poder ver o que está acontecendo no campo.

```
./rcssclient
```
ou 

```
rcssclient > /dev/null 2>&1
```

## 🧑‍🎓 Equipe
- Nossa equipe é composta por graduandos do segundo ao quinto período dos cursos de Ciência da Computação e Engenharia Elétrica da Universidade Federal de Campina Grande(UFCG), todos sendo voluntários do Capítulo Estudantil da Sociedade de Robótica e Automação (IEEE RAS UFCG).

| [<img src="https://avatars.githubusercontent.com/u/79481939?v=4" width=115><br><sub>Guilherme Toledo</sub>](https://github.com/drawnator) |  [<img src="https://avatars.githubusercontent.com/u/25869603?v=4" width=115><br><sub>Lucas Melo</sub>](https://github.com/TryhardCC) |  [<img src="https://avatars.githubusercontent.com/u/57972059?v=4" width=115><br><sub>Samara Cardoso</sub>](https://github.com/SamaraLimaCardoso) |
| :---: | :---: | :---: |


<h4 align="center"> 
    :construction:  Projeto em construção  :construction:
</h4>
