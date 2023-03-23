# Committing

O commit basicamente "tira uma foto" do estado atual do seu repositório e salva no histórico do git, isso funciona similarmente a um album de fotos onde a qualquer momento você pode navegar entre os estados do repositório.

## Fazer um commit

Adicionar um "foto" do estado atual do repositório ao histórico.
A tag -m insere uma mensagem que especifica o que foi feito nesse novo estado do repositório (o que mudou em relação ao estado anterior)

```bash
git commit -m "[message]"
```

Atalho -am :  Ele combina os comandos `git add` e `git commit -m` adicionando todos os arquivos no staged e salvando no histórico do git.

```bash
git commit -am "[message]"
```

## Editar um commit

Para editar um commit podemos utilizar o `--amend`, este comando permite editar o último commit feito permitindo modificar a mensagem de commit,  subir novos arquivos e alterações que estejam na stage area.

```bash
  git commit --amend
```

## Desfazer um commit

### Modo safe

revert: cria um novo commit desfazendo modificações de outro commit

```bash
git revert [commit-hash]
```

Caso queira desfazer o último commit feito e não um específico

```bash
git revert HEAD 
```

### Modo vida loca (evite usar na master/main)

reset: volta o histórico do git para um commit específico, deletando todos os outros commits e alterações feitas após o hash especificado.

**--soft**
Deleta todos os commits, porém coloca or arquivos modificados na stage area para você decidir o que quer fazer com eles.

```bash
git reset [commit-hash] --soft 
```

**--mixed**
Deleta todos os commits, porém coloca or arquivos como mudanças locais para  você decidir o que quer fazer com eles. (basicamente igual ao --soft, porém não adiciona na stage area)

```bash
git reset [commit-hash] --mixed 
```

**--hard**
Deleta todos os commits e arquivos (TUDO MESMO CUIDADO)

```bash
git reset [commit-hash] --hard 
```

## Pegar um commit específico

O comando `cherry-pick` permite copiar um commit específico e coloca-lo no branch atual.

```bash
git cherry-pick [commit-hash]  
```
