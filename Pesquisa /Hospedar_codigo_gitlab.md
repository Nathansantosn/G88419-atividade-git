# 1️⃣ Configurar o Git (se ainda não fez)
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"

# 2️⃣ Criar um novo repositório local (se ainda não existir)
cd /caminho/do/seu/projeto
git init

# 3️⃣ Adicionar um arquivo README (opcional)
echo "# Meu Projeto" > README.md
git add README.md
git commit -m "Primeiro commit"

# 4️⃣ Conectar ao repositório remoto no GitLab (substitua pela URL do seu repositório)
git remote add origin https://gitlab.com/seu-usuario/seu-projeto.git

# 5️⃣ Verificar se o repositório remoto foi adicionado corretamente
git remote -v

# 6️⃣ Enviar código para o GitLab (branch principal é 'main' por padrão)
git branch -M main
git push -u origin main

# 🔄 Para atualizar o repositório no futuro:
git add .
git commit -m "Descrição das alterações"
git push origin main
