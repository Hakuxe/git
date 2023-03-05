# Crinado novas funcionalidades (branchs)

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

## Exibindo alterações

    # mostra a última alteração feita no  git
    git show

    # exibir todas as alterações que foram feitas no arquivo
    git log

        # listar commits por nome
        git log --author=nome

        # exibi o log simplificado
        git log --oneline
