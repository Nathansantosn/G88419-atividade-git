# Passo a Passo para Hospedar o Código no GitHub

## 1. Criar um Repositório no GitHub

### Acessar o GitHub:
- Vá para o site do [GitHub](https://github.com) e faça login com sua conta.

### Criar um Novo Repositório:
1. Clique no ícone de "+" no canto superior direito da página e selecione **New repository**.
2. Escolha um nome para o seu repositório (ex: `meu-repositorio`, `projeto-git`, etc.).
3. **Não** marque a opção *Initialize this repository with a README*, pois vamos adicionar o arquivo README mais tarde.
4. Escolha se o repositório será **público** ou **privado**:
   - Se for privado, lembre-se de adicionar o professor `massilva` como colaborador.
5. Clique em **Create repository** para criar o repositório vazio.

---

## 2. Conectar o Repositório Local ao GitHub

### Copiar o URL do Repositório:
Após criar o repositório no GitHub, copie o link do repositório remoto. O link será algo assim:

```
https://github.com/SEU_USUARIO/MEU_REPOSITORIO.git
```

**Dica**: Substitua `SEU_USUARIO` pelo seu nome de usuário no GitHub e `MEU_REPOSITORIO` pelo nome do seu repositório.

### Adicionar o Repositório Remoto no Terminal:
Abra o **VSCode** ou o terminal no diretório do seu repositório local (onde está o código que você deseja enviar para o GitHub) e execute:

```bash
git remote add origin https://github.com/SEU_USUARIO/MEU_REPOSITORIO.git
```

### Verificar a Conexão Remota:
Para verificar se a conexão foi feita corretamente, execute:

```bash
git remote -v
```

---

## 3. Realizar o Primeiro Commit

### Adicionar os Arquivos ao Git:
Se você já tem os arquivos prontos no diretório do seu projeto, adicione-os ao repositório local:

```bash
git add .
```

### Fazer o Commit das Alterações:
Agora, faça o commit para salvar as alterações localmente:

```bash
git commit -m "Primeiro commit - Adicionando os arquivos iniciais"
```

---

## 4. Subir o Código para o GitHub

### Fazer o Push para o GitHub:
Após o commit, envie suas alterações para o repositório remoto no GitHub com o comando:

```bash
git push -u origin master
```

**Nota**: Se o seu repositório utiliza o branch `main` em vez de `master` (o que é comum para repositórios novos), o comando será:

```bash
git push -u origin main
```

### Verificar no GitHub:
Após o comando *push*, acesse o seu repositório no GitHub e verifique se os arquivos foram carregados corretamente.

---

## 5. Compartilhar o Repositório com os Integrantes e o Professor

- **Repositório Público**: Se o repositório for público, basta compartilhar o link do repositório com os membros da equipe e o professor.
- **Repositório Privado**: Se o repositório for privado, será necessário adicionar os membros da equipe e o professor como colaboradores.

### Para adicionar colaboradores:
1. Acesse as **Configurações** (*Settings*) do repositório.
2. Selecione **Manage access**.
3. Clique em **Invite a collaborator** e adicione o usuário `massilva`.

---

## 6. Confirmar a Atualização e Compartilhar o Link
Após garantir que tudo foi feito corretamente no repositório GitHub, compartilhe o link do repositório no **Classroom** (ou conforme as instruções do professor).
