# git_testes
Anotações e testes de uso do GIT


# Inicio de um projeto

---
git init

Vai criar a pasta .git no diretório. A partir dessa pasta o git vai monitorar as alterações.


---
git config user.name "Meu nome"
git config user.email "email@mail.com"

Configura nesse repositório git usuário e e-mail de identificação de quem vai fazer os commits


---
git config --global user.name "Meu nome"
git config --global user.email "Meu nome"

Configura nome e e-mail de todos os repositórios naquela máquina


---
git add arquivo.txt
git add .

Adiciona arquivos para STAGED, preparados para o commit.


---
git commit -m "Comentários do commit"

É criado uma fotografia do projeto na linha do tempo.


---
git push

Envia os commits locais para branch remota.


---
git diff
git diff 2fd21b7 c3d6a19

Mostra as diferença entre arquivos ou commits
