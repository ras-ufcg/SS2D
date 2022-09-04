<h1 align="center"> Competição SS2D </h1>

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
![GitHub Org's stars](https://img.shields.io/github/stars/ras-ufcg/SS2D?style=for-the-badge&logo=github)


| Nosso Projeto | Primeiros Passos |Aprendendo Mais|
| ---------------- | ---------------- |------------- |
| 🤖[**SS2D**](#-competição-ss2d) |🛠[**Instalação Server+Monitor**](#-instalando-o-servidor-e-monitor) |📖[**Material Extra**](#-aprendendo-mais) |
| 📝[**Descrição**](#-quem-somos) |📼[**Assistir um Jogo Gravado**](#-rodando-um-jogo-gravado) |🗂️ [**Acesso ao Projeto**](#-acesso-ao-projeto) |
| 🧑‍🎓[**Equipe**](#-equipe) |🛠[**Instalação de Equipes**](#-instalando-as-equipes) |💻[**Criando um Binário**](#-criando-um-binário) |
| 📄[**Metodologia**](#-metodologia) |🎮[**Rodando o Primeiro Jogo**](#-primeira-partida) | 🕹️[**Modo de Controle Manual**](#-controlando-um-robô) |
| 🗓[**Planejamento**](#-planejamento) | | |

<!---## Sumário
- Sobre o Projeto
    - 🤖[**SS2D**](#-Competição-SS2D) 
    - 📝[**Descrição**](#-quem-somos)
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
- A SS2D é a modalidade da Robocup que aborda o futebol simulado por computador num espaço 2D. 
- Cada time tem 11 jogadores virtuais que "pensam" separadamente e tomam decisões com base nas informações que conseguem capturar do seu ambiente. 
- Os jogadores têm atributos como velocidade máxima, precisão de chute, tamanho e energia. Esses atributos são escolhidos aleatoriamente pelo servidor em cada partida. 
- Os algoritmos e lógicas que cada jogador usa para decidir o que ele vai fazer devem ser criados pela equipe do time. Porém, é permitido e recomendado que equipes novas utilizem o código de outras equipes como base.
- As regras das partidas do SS2D são extremamente parecidas com as que conhecemos no futebol: Existem faltas, impedimentos, tiros de meta, cartões, entre outros. Ganha a partida o time que fizer mais gols.
## 📝 Quem somos?
- Esse projeto tem como finalidade a contrução de um time de futebol de robôs 2D para competições. 
-
-
## 📄 Metodologia
-
-
-

## 🗓 Planejamento
-
| # | Atividade | Status |
| ---------------- | ---------------- |------------- |
| 1 | Compreender a Competição SS2D - Leitura de TDP's |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 2 | Instalção do Servidor e do Monitor |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 3 | Instalação dos Times Base e Rodar Partidas |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 4 | Realizar o controle Manual de um Dummy |<img alt="Finalizado" src="https://img.shields.io/badge/-Finalizado-brightgreen">|
| 5 | Criação de um Time Com Apenas um Cliente | <img alt="Em Andamento" src="https://img.shields.io/badge/-Em%20andamento-orange">|
| 6 | Criação de uma Estratégia Própria | <img alt="Não Iniciado" src="https://img.shields.io/badge/-Não%20iniciado-red">|


## 🛠 Instalando o Servidor e Monitor
- Recomenda-se usar ubuntu 16.04 ou posterior para rodar os programas pois é possivel instalar todos os requerimentos com os seguintes comandos:
```
sudo apt update
sudo apt install build-essential automake autoconf libtool flex bison libboost-all-dev
sudo apt install build-essential qt5-default libfontconfig1-dev libaudio-dev libxt-dev libglib2.0-dev libxi-dev libxrender-dev
```

- Servidor:

    Antes de continuar é recomendado criar uma pasta /servidor/ onde você salvará tanto o servidor quanto o monitor dentro

    No github do servidor https://github.com/rcsoccersim/rcssserver/releases baixe a versão mais recente do rcssserver-x.x.x.tar.gz substituindo "x" pelo numero da    versão e rode os seguintes códigos substituindo o nome do arquivo para o correto:
    ```
    tar xzvfp rcssserver-x.x.x.tar.gz
    cd rcssserver-x.x.x
    ./configure
    make
    ```

    Agora quando você quiser pode rodar o binario ./rcssserver dentro do /src/ do servidor para fazer o servidor funcionar, porem mesmo rodando, não vai ser possivel ver oque está acontecendo pois o monitor ainda não está instalado

- Monitor:

    Dentro da pasta /servidor/ mencionada a cima baixe a versão mais recente do monitor https://github.com/rcsoccersim/rcssmonitor/releases e rode os seguintes códigos substituindo o nome do arquivo pelo nome correto:
    ```
    tar xzvfp rcssmonitor-x.x.x.tar.gz
    cd rcssmonitor-x.x.x
    ./configure
    make
    ```

    Agora você pode rodar o binario ./rcssmonitor dentro do /src/ do monitor para fazer o monitor funcionar.

    Lembre-se de rodar o servidor sempre antes do monitor. você saberá que tudo está funcionando se os jogadores aparecerem no monitor na parte superior logo fora da quadra como na imagem:



## 📼 Rodando um Jogo Gravado
-
-
-

## 🛠 Instalando as Equipes
- A princípio estão sendo usadas as seguintes equipes como base:
    - [Helios Base 2D](https://github.com/helios-base/helios-base)
    - [Cyrus Base 2D](https://github.com/Cyrus2D/Cyrus2DBase)
- Para a instalação dos times bases será necessário ter as seguintes bibliotecas:
    - Boost 1.38 ou posterior https://www.boost.org/
        ```
        sudo apt update
        sudo apt install build-essential libboost-all-dev
        ```
    - A última librcsc https://github.com/helios-base/librcsc
    - Libeigen3-dev
        ```
        sudo apt-get update
        sudo apt-get install libeigen3-dev
        ```
## 🎮 Primeira Partida
depois que tudo estiver instalado e você quiser assistir a primeira partida você deve seguir essa sequencia de passos para simular seu primeiro jogo:

- abrir 4 janelas de terminal
- no 1° terminal entrar na pasta /servidor/rcssserver-x.x.x/src/ e rodar ./rcssserver
- no 2° terminal entrar na pasta /servidor/rcssmonitor-x.x.x/src/ e rodar ./rcssmonitor
- no 3° terminal rodar o ./start.sh do primeiro time
- no 4° terminal rodar o ./start.sh do segundo time
- dentro da janela que o monitor abriu clicar em referee e depois kickoff (ou ctrl + k)

caso algo der errado lembrese de esperar alguns segundos entre cada passo 

## 📖 Aprendendo Mais
softwares oficiais:
- https://github.com/rcsoccersim/rcssserver
- https://github.com/rcsoccersim/rcssmonitor

wikipedia:
- https://en.wikipedia.org/wiki/RoboCup_2D_Soccer_Simulation_League

Replay:
- https://archive.robocup.info/Soccer/Simulation/2D/replays/

TDP:
- https://tdp.robocup.org/tdp/
- http://archive.robocup.info/Soccer/Simulation/2D/TDPs/RoboCup/

Docs:
- https://rcsoccersim.readthedocs.io/en/latest/
- https://github.com/herodrigues/robocup2d-tutorial
- https://www.youtube.com/watch?v=eQwX2p5CNFI&list=PLFy1-QjBONFL_yjjOOh6brRJgZMfLyBbw

Equipes:
- https://robocin.com.br/publicacoes.html
- https://bitbucket.org/itandroids/itandroids-soccer2d/wiki/_oldHome

Base team:
- https://github.com/helios-base/helios-base
- http://www.prokopenko.net/gliders2d.html

inteligencia artificial:
- https://www.cin.ufpe.br/~tg/2019-2/TG_EC/Evaluating_Reinforcement_Learning_on_Robocup_Soccer_Simulation_2D%20.pdf

## 🗂 Acesso ao Projeto
-
-
-

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
-
-
-

## 🧑‍🎓 Equipe
| [<img src="https://avatars.githubusercontent.com/u/79481939?v=4" width=115><br><sub>Guilherme Toledo</sub>](https://github.com/drawnator) |  [<img src="https://avatars.githubusercontent.com/u/25869603?v=4" width=115><br><sub>Lucas Melo</sub>](https://github.com/TryhardCC) |  [<img src="https://avatars.githubusercontent.com/u/57972059?v=4" width=115><br><sub>Samara Cardoso</sub>](https://github.com/SamaraLimaCardoso) |
| :---: | :---: | :---: |


<h4 align="center"> 
    :construction:  Projeto em construção  :construction:
</h4>
