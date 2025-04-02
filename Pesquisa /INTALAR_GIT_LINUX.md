# Como Instalar o Git no Linux

Este tutorial descreve o processo de instalação do Git em distribuições Linux mais comuns.

## Passo 1: Atualize seu Sistema

Antes de começar a instalação, é uma boa prática atualizar seu sistema. Abra o terminal e execute:

```bash
sudo apt update && sudo apt upgrade -y   # Para distribuições baseadas no Debian/Ubuntu
sudo dnf update -y                      # Para distribuições baseadas no Fedora
sudo pacman -Syu                        # Para distribuições baseadas no Arch
```

## Passo 2: Instalar o Git

### Em Distribuições Baseadas no Debian/Ubuntu

Para instalar o Git em distribuições como Ubuntu, Debian e derivados, use o comando:

```bash
sudo apt install git -y
```

### Em Distribuições Baseadas no Fedora

Para instalar o Git em distribuições baseadas no Fedora, use o comando:

```bash
sudo dnf install git -y
```

### Em Distribuições Baseadas no Arch

Para instalar o Git em distribuições baseadas no Arch, como Manjaro, use o comando:

```bash
sudo pacman -S git
```

## Passo 3: Verificar a Instalação

Após a instalação, verifique se o Git foi instalado corretamente executando o comando:

```bash
git --version
```

Isso deve retornar a versão do Git instalada, por exemplo:

```
git version 2.34.1
```

## Passo 4: Configurar o Git

Agora que o Git está instalado, você pode configurar seu nome de usuário e e-mail, que serão usados nos commits. Execute os seguintes comandos, substituindo "Seu Nome" e "seu-email@exemplo.com" pelos seus dados:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

## Passo 5: Confirmar a Configuração

Você pode verificar as configurações do Git com:

```bash
git config --list
```

Isso mostrará a configuração global do Git, incluindo o nome de usuário e o e-mail.

Pronto! Agora você tem o Git instalado e configurado no seu sistema Linux.
