# Basico git

---
Head aponta para qual o commit mais recente

Working directory -> Staged area -> Local repository

---

## Configurando usuário

- git config --global user.email "you@example.com"
- git config --global user.name "Your Name"

### Adicionando arquivos

- git add < nome do arquivo >
  - git add . = adiciona todos os arquivos

### listando as configs

- git config --list

### mostrar a linha do tempo de commits

- git log
  - git log --author=nome listar commits por nome
  - git log --grop=achar um commit filtrando pela msg
  - git log --oneline (exibi o log simplificado)

### Alterações no working directory

- git diff =  mostra um histórico das modifiações feitas no working directory, nos arquivos que não estão na staged area

- git diff --staged = para mostra as que estão no staged

### Recuperando arquivos

- git rm < nome do arquivo >
  - git rm -r --cached < nome do arquivo > remover tudo que está sendo rastreado no git

### Renomear ou movendo arquivos

- git mv < nome do arquivo > < novo nome >
    (esse comando pode ser usado para mover um arquivo de pasta meio que romeando o arquivo pro caminho desejado )

### Desfazendo commit alterações

- git restore < nome do arquivo >
  - git restore --staged < nome do arquivo > (caso já esteja na stage area)
  - git reset HEAD < nome do arquivo > (jeito antigo de fazer)

## Ver alterações no local repository

- git show < começo da hash de um commit >
  - git show < começo da hash de um commit > --color-words (marcar as palavras que mudaram)
  - git show < começo da hash de um commit > -- < caminho arquivo > (mostrar todas a modificações de 1 arquivo específico )



## Exibindo alterações

 mostra a última alteração feita no  git
git show

 exibir todas as alterações que foram feitas no arquivo
git log

    # listar commits por nome
    git log --author=nome

    # exibi o log simplificado
    git log --oneline
```