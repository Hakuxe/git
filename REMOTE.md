## Passando projeto para o github
    # colocar os dados do git na nuvem do github 
    git remote add origin <link do repositrio do git>

    # enviar alterações locais para o repositório remoto 
    git push

## Pegar um projeto que já foi iniciado
    # clonar o projeto do repositório online  para o local 
    git clone <link do projeto >
    
    # pegar as atualizações da nuvem e aplicar no projeto local 
    git pull



## Swapping an HTTPS Repo To SSH Authentication
    # remover a origin atual 
    git remote rm origin

    # trocar pela ssh-key
    git remote add origin < ssh-key do repositório >
    git push --set-upstream origin/< nome da branch principal >