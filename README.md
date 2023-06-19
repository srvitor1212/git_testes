# git_testes
Anotações e testes de uso do GIT


# Estados de arquivos
Untracked | Tracked | Modified | Staged
------------------|------------------|------------------|------------------
Arquivo não controlado ou rastreado pelo git | Arquivo controlado pelo git | Arquivo que já é rastreado pelo git e que sofre uma alteração | Arquivo pronto para ser enviado pro repositório, ocorre no git add


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


# Comandos básicos
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
git pull

Atualiza o repositório local. Usa-lo na branch develop ou main.


---
git diff

git diff 2fd21b7 c3d6a19

Mostra as diferença entre arquivos ou commits


# Log de commits
---
git log

Mostra o histórico de commits da branch atual

---
git log --all

Mostra o histórico de commits de todos o projeto e suas branches.


---
git log --oneline

Mostra cada commit em uma linha de forma resumida.


---
git log -3

Mostra só os últimos X commits


---
git commit --amend -m "Nova mensagem no commit"

Renomeia a mensagem do último commit. Também adicionar arquivos no staged ao commit.


# Voltar no tempo
---
git checkout 2fd21b7

Volta os arquivos para o commit informado, após esse comando é recomendado criar uma nova branch.

---
git restore

Desfaz as alterações que ainda não foram enviadas para Stage.

--- 
git restore --staged ARQUIVO.TXT

Voltar a alteração de staged (git add) para modificado, permitindo usar o git restore para desfazer as alterações.

---
git checkout ARQUIVO.TXT

Parecido com git restore, volta as alterações do arquivo que não ainda não foi enviado para stage.

---
git reset HEAD --hard

Desfas todas as alterações e volta para o HEAD. Não tem volta...


# Branches
---
git branch

Mostra as branches locais


---
git branch --all

Mostra todas as branches, inclusive as remotas


---
git checkout master

Muda de branch


---
