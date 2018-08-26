# Minicurso de Git e GitHub - SEINFO 2018
Minicurso da V Semana de Informática da UTFPR-CM (Git e GitHub). Ministrado por: Giorgio Braz e Lucas Ribeiro

O Git é um sistema de controle de versão distribuído (não centralizado), ou seja, a cópia desenvolvida com o passar do tempo estará em todas as estações de trabalho e não somente no repositório.
￼
## Configuração inicial - aula 1
- git config --global user.name “seuNome”
- git config --global user.email seuEmail

### Comandos mais utilizados
- git status
- git pull
- git add .
- git commit -a -m “first commit”
- git push

## Controle de versão - aula 2
(apenas 1 desenvolvedor)
- git init para criar um novo repositório 
- git status
- git add .
- git commit -m “first commit”
- Não quero controlar essa versão -> crie um arquivo.gitignore e coloque o nome do(s) arquivo(s) desejado(s) -> somente uma informação por linha;

## Visualização de alterações - aula 3
- git diff usado no working directory
- git diff --staged usado na staging area
- git log mostra todos os commits feitos no projeto
- git log -p mostra em ordem cronológica decrescente e as alterações feitas em cada arquivo
- git log -p -1 número do último comia, vai até -n
- git log --pretty=oneline mostra a chave do commit
- gitk usar uma interface gráfica

## Desfazendo algo - aula 4
Editando um commit recente
- git add .
- git commit --amend -m "Novas funcionalidades (edição)"
- Remover arquivo de staged
- git reset HEAD file_name
- Revertendo mudanças em working directory
- git checkout -- file_name
#### Para remover
- gir rm file_name

## Tags e branches - aula 5
- Criar uma tag (no commit atual) git tag -a <v1.0> -m "Versão 1.0"
- Criar uma tag (num commit antigo) git tag -a v0.0 CHAVE -m "Versão 0.0"
- Para listar as tags git tag
- Ver detalhes da tag git show v0.0
- Reverter a versão git checkout v0.0
- Deletar uma tag git tag -d nome_da_tag
- git checkout master
- Criando testes ou novas versões utilizando um branch
- Criar e trocar de uma só vez git checkout -b teste

OU...
- Criar um novo branch git branch teste
- Movendo o working directory para o ambiente de teste git checkout teste
- Para retornar git checkout master
- Transferindo as alterações do ‘teste’ para o ‘master’ git merge teste
- Deletar um branch git branch -d teste
- Listar os branches num repositório git branch

## Git em rede local - aula 6
(Máquina local como servidor - 2º ambiente de desenvolvimento)
- Git e GitHub - aula 7
- Autorizando seu computador ssh-keygen
- git clone endereço...

## Colaborando com um projeto - aula 8
- Fork
- Pull requests
----
### Referências

[Uma Breve História do Git](https://git-scm.com/book/pt-br/v1/Primeiros-passos-Uma-Breve-História-do-Git)

[Git e Github – Hipsters #109](https://pca.st/YB7E)

[Tutorial no YouTube](https://www.youtube.com/playlist?list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)

[Site oficial do Git](https://git-scm.com)

[Guias do GitHub](https://guides.github.com)
