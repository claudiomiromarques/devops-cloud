Passo a passo macro

Módulo 2: Solução do Projeto Hands-on

 

# criando uma pasta: mkdir devops-cloud
# acessando a pasta: cd devops-cloud
# criando outra pasta: mkdir src
# acessando a pasta: cd src
# baixando arquivos do Website: curl -k -L --output website.zip https://tcb-bootcamp-devops-cloud.s3.amazonaws.com/tcb-bdc-module2-hop.zip
# descompactando: unzip website.zip
# testando Website: index.html 'open with Live Server' | Instalar VSCode Extesion

# inicializando o Git: git init
# renomenado a Branch:  git branch –m main
# verificando Stauts do Git: git status | "Não precisamos do arquivo 'website.zip' como parte da solução!"
# criando o arquivo Git Ignore: touch .gitignore
# adicionando 'website.zip' no arquivo Git Ignore: vi .gitignore | INSERT Key | website.zip | ESC | :wq!
# adicionando arquvos em 'Stage Area' (aguardando commmit...):

git add .

Removendo arquivos da area de Stage: git rm -r --cached .

git add .

# Configurando Author Name/Email:

git config --global user.name devopscloudbootcamp
git config --global user.email devopscloud@outlook.com
git config --list

# comitando primeira versao do website:

git commit -m 'Website primeira versao!'

# verificando Status do Git:

git status

----------------------------------

▒GitHub▒ 🐱

# criando um repositorio: devops-cloud

# configurando credentiasl para o GitHub (if you used different credentials for Author Name/Email):

git config user.name devopscloudbootcamp
git config user.email devopscloud.bootcamp@outlook.com

# conectando o 'repo' local com o remoto (origin):

git remote add origin [ url repositorio remoto ]

# verificando repositorio remoto:

git remote -v

# uploading repositorio local para o remoto:

git push -u origin main

# Será requisitado 'login' no GitHub: "Sign in with your browser" | Authorize GitCradentialManager

# refresh na página do GitHub!

# Validando 'Short SHA1 Hash' com Git Log!

# Alterando index.html no from GitHub: Edit File | Preview File | Commit Changes

▒ Visualizando as Alterações feitas no GitHub:

https://raw.githack.com/
https://htmlpreview.github.io/

# verificando se o repo Local está atualizado:

git remote show origin

# downloading / atualizando o repositorio Local:

git pull

----------------------------------

# alterando index.html De: 'h1' Para: 'h3'

git commit -am 'alterando h1 para h3'   [adding e commiting]
git log
git show [hash]

# atualizando/uploading repositorio remoto:

git push -u origin main

# revertendo o último commit:

git revert hash

# verificando se o repositorio Remote esta atualizado:

git status uno

# atualizando/uploading repositorio remoto:

git push -u origin main

git status uno
