# Branches, ramificações ou galhos

## Criar novas ramificações(branches)

Gerar uma nova ramificação(branch) que deriva da anterior

```bash
git branch [nome-do-novo-branch]
```

Outra forma de criar um novo branch é usar a tag `-b` no comando `checkout`, assim o branch será criado e repositório local e movido para ele.

```bash
    git checkout -b [nome-do-branch]
```

## Navegar entre branches

Para navegar entre os branches pode ser utilizado o `checkout` ou `switch`:

```bash
git checkout [nome-branch]
```

A diferença entre eles é que o `switch` foi implementado nas versões mais novas do git, com o intuito de "diminuir" a quantidade de funcionalidade abrangidas pelo comando `checkout`

```bash
git switch [nome-branch]
```

## Exibir branches

mostrar tds os branchs criados

```bash
git branch
```

[//]: # "adicionar tags "

## Deletar um branch

Deletar um branch/galho existente

```bash
 git branch -D [nome-branch]
```

Deletar um branch existente num repositório remoto

```bash
git push origin --delete [nome-branch]

```

## Manipulando branches

### Git Merge

O comando git merge ser para unir os arquivos de 2 branches. Para realizar o git merge basta dar um `switch` ou `checkout` para o branch que vai **receber** os arquivos e executar o comando:

```bash
git merge [nome-branch]
```
