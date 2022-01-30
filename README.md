## Iniciando no git 

    # Iniciar o repositório no git // uma linha do tempo
    git init 

    # Adicionar um arquivo no repositório git criado
    git add <nome do arquivo> 

    # adicina tudo no git
    git add . 

    # colocar um arquivo na árvore do git (colocar pontos na história do git)    
    git commit 


##  Removendo arquivos 

    # remover arquivos de um repositório do Git. (o inverso do comando git add)
    git rm < nome do arquivo >
    
    # remover um diretório  e tudo que está dentro dele
    git rm -r < nome do arquivo > 


###  Renomear ou movendo arquivos

    # usado para renomear/mover um arquivo de pasta (meio que renomeando o arquivo pro caminho desejado )
    git mv < nome do arquivo > < novo nome >


## Exibindo alterações

    # mostra a última alteração feita no  git
    git show
    
    # exibir todas as alterações que foram feitas no arquivo 
    git log
    
        # listar commits por nome
        git log --author=nome 
     
        # exibi o log simplificado
        git log --oneline 



## Crinado novas funcionalidades (branchs)

    # gerenciar novas "linhas do tempo"
    git branch <nome do novo branch>

    # mudar para os outros "universos" (master, feature/carrinho_de_compras)
    git checkout <branch>

    # criar um novo branch e alterar o repositorio atual para ele
    git checkout -b <nome do branch>

    # mostrar tds os branchs criados
    git branch  
    
    # deletar um "galho " existente
    git branch -D <nome branch> 
    
    # deletar branch remota
    git push origin --delete nome-da-branch  

    

## Manipulando branchs
    # unir os arquivos de 2 branch's
    git merge

