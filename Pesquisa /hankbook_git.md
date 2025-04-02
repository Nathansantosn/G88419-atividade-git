# Handbook do GIT - Principais Comandos do GIT

Este documento serve como um guia de referência rápida para os comandos mais utilizados no Git. A seguir, serão descritos os comandos básicos e mais importantes para controlar o versionamento do código.

## 1. Inicializando um Repositório Git

```bash
git init
```

O comando `git init` é usado para inicializar um novo repositório Git em um diretório existente. Esse comando cria um diretório oculto `.git`, onde o Git vai armazenar os dados do repositório.

## 2. Configurando o Git

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@dominio.com"
```

Esses comandos definem o nome e o email do usuário para todos os commits feitos no Git.

Exemplo:

```bash
git config --global user.name "João Silva"
git config --global user.email "joao.silva@dominio.com"
```

## 3. Verificando o Status do Repositório

```bash
git status
```

O comando `git status` permite verificar o status do repositório, mostrando quais arquivos foram modificados, quais estão prontos para o commit e se há arquivos não rastreados.

## 4. Adicionando Arquivos ao Repositório

```bash
git add <arquivo>
git add .
```

O comando `git add` adiciona arquivos ou mudanças ao índice do Git, preparando-os para serem commitados.

Exemplo:

```bash
git add README.md
git add .
```

## 5. Realizando o Commit

```bash
git commit -m "Mensagem do commit"
```

O comando `git commit` grava as alterações feitas no repositório, com uma mensagem que descreve as mudanças realizadas.

Exemplo:

```bash
git commit -m "Corrigindo erro de digitação no README"
```

## 6. Verificando o Histórico de Commits

```bash
git log
git log --oneline
```

O comando `git log` exibe o histórico de commits feitos no repositório. A opção `--oneline` exibe um resumo do histórico, mostrando apenas o hash e a mensagem de cada commit.

## 7. Fazendo o Push para o Repositório Remoto

```bash
git push origin <branch>
```

O comando `git push` envia os commits do seu repositório local para o repositório remoto.

Exemplo:

```bash
git push origin main
```

## 8. Fazendo o Pull de um Repositório Remoto

```bash
git pull origin <branch>
```

O comando `git pull` busca as alterações do repositório remoto e as integra no seu repositório local.

Exemplo:

```bash
git pull origin main
```

## 9. Criando um Novo Branch

```bash
git branch <nome-do-branch>
git checkout <nome-do-branch>
git checkout -b <nome-do-branch>
```

O comando `git branch` cria um novo branch. O `git checkout` muda para o branch especificado, e a opção `-b` cria e muda para um novo branch ao mesmo tempo.

Exemplo:

```bash
git branch nova-feature
git checkout nova-feature
git checkout -b nova-feature
```

## 10. Mesclando Branches (Merge)

```bash
git merge <nome-do-branch>
```

O comando `git merge` integra as alterações de um branch no branch atual.

Exemplo:

```bash
git merge nova-feature
```

## 11. Visualizando Diferenças no Código

```bash
git diff
```

O comando `git diff` mostra as diferenças entre o estado atual do seu código e a versão do commit mais recente.

## 12. Desfazendo Mudanças

```bash
git checkout -- <arquivo>
git reset <arquivo>
```

O `git checkout -- <arquivo>` restaura o arquivo para o estado do último commit, e o `git reset <arquivo>` desfaz a adição do arquivo ao índice sem excluir suas alterações.

Exemplo:

```bash
git checkout -- README.md
git reset README.md
```

## 13. Removendo Arquivos

```bash
git rm <arquivo>
```

O comando `git rm` remove um arquivo do repositório e o marca para ser excluído no próximo commit.

Exemplo:

```bash
git rm arquivo_desnecessario.txt
```
