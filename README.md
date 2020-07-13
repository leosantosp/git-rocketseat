# GIT e GITHUB

Guia prático para iniciantes.

### Instalação  

https://git-scm.com/download

# SCENES

- [add,commit] Você deseja criar pontos na história da produção do seu projeto
- [show,log] Você deseja verificar mudanças feitas no seu projeto

- [branch] Você começa uma nova funcionalidade no seu projeto, sem estragar o que já foi feito
- [checkout,add,commit] Você adiciona novas funcionalidades ao seu projeto em produção
- [branch-d] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto

# COMMANDS

`git init` -> Faz com que a pasta em questão se torne um repositório Git

`git add` -> Adiciona o item para a caixa de commit, você pode adicionar vários itens para esta 'caixa', caso queira que alguns itens tenha um comentário em específico e outros com outro tipo de comentário

`git commit` -m -> Realiza um comentário em cima dos arquivos que você adicionou

`git log` -> Eu posso visualizar o número de identificação deste commit, quem foi o autor do commit e a data e hora do comentário

`git status` -> Visualiza o status atual daquele projeto em relação ao que já está comentado

`Shift + Q` -> Volta a pasta inicial

`git show + serial number` -> Com o git show, nós podemos revisitar um ponto na história da produção do projeto e verificar o que foi alterada naquela versão em especifico, para verificar quais são os seriais da alteração, é possível visualizá-los no git log

// Com isso, notamos que podemos tanto criar arquivos e adicioná-los com comentários ao nosso git, isso cria um ponto na história do projeto e tornando possível revisitar estes projetos, no entanto, além de navegarmos através da história do projeto, podemos ir para mundos paralelos deste projeto, utilizando o 'branch' ou 'ramificação'. O branch é uma espécie de repositório quando queremos criar uma nova funcionalidade sem estragar o que já foi feito. 

`git branch NomeDaRamificacao` -> este comando cria uma nova ramificação no seu projeto

`git checkout NomeDaRamificacao` -> Durante a produção, você estará o tempo todo na 'master' ou seja no Mundo Principal do projeto, o checkout leva você tanto para o mundo paralelo (branch) como leva você de volta ao (master). Para voltar é digitar apenas checkout master

PS: O 'git status' também te informa se você está no 'head' ou na 'branch' 

`git branch` -> Este comando mostra todas as ramificações existentes (inclusive a master)

`ls` -> no terminal, isto lista todos os itens disponíveis naquela pasta git

`git merge NomeDaRamificacao` -> Este comando vai mesclar os arquivos da ramificacao especificada no comando com a atual que você está utilizando

`git branch -D NomeDaRamificacao` -> Este comando exclui uma ramificação que foi criada no histórico do projeto. Obviamente, após adicionar a ramificação ao projeto principal, não existe motivo pra ramificação existir


### COLOCANDO O PROJETO NA NUVEM

Após criar o seu repositório na Nuvem (Site do Git) é necessário copiar um comando que é exibido após a criação do projeto

`git remote add origin https://link.com.br` -> Comando para adicionar o repositório nuvem em questão para o repositório local que estamos inserindo esta linha de comando

`git remote -v` -> Este comando me permite visualizar os meus repositórios remotos

`git push` -> Este comando serve para empurrar os seus arquivos no repositório local para o repositório em nuvem, toda primeira vez que fizer um push em um repositório é necessário que insira o comando `git push -u origin master`, isto serve para criar a branch master no repositório remoto

Caso seja requisitado, é necessário inserir seu username e password da sua conta no GitHub

`git add .` -> Este comando adiciona TODOS os arquivos dentro da pasta