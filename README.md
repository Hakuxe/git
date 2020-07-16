## Iniciando no git 
    git init : iniciar o repositório no git // uma linha do tempo
    git add <nome do arquivo> : adicionar um arquivo no repositório git criado  
    git add . : adicina tudo no git     
    git commit : colocar um arquivo na árvore do git (colocar pontos na história do git)

## Exibindo alterações
    git log; mostra todas as alterações que foram feitas no arquivo 
    git show: mostra a última alteração feita no  git  

## Crinado novas funcionalidades (branchs)
    git branch <nome do novo branch>: gerenciar novas "linhas do tempo"
    git checkout <branch>: mudar para os outros "universos" (mastar, feature/carrinho_de_compras)
    git branch : mostrar tds os branchs criados 
    git merge: unir os arquivos de 2 branch's
    git branch -D <nome branch>: deletar um "galho " existente 
    git checkout -b <nome do branch>: criar uma nova linha do tempo e alterar o repositorio atual para ela

## Passando projeto para o github
    git remote add origin <link do repositrio do git>: colocar os dados do git na nuvem do github 
    git push: enviar alterações locais para o repositório remoto 

## Pegar um projeto que já foi iniciado
    git clone <link do projeto >: clonar o projeto do repositório online  para o local 
    git pull: pegar as atualizações da nuvem e aplicar no projeto local 