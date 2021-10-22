Nome: Emanuelle 

git init: Serve para converter um projeto existente e não versionado em um repositório do Git ou inicializar um novo repositório vazio.

Faça commit:
git init -b main


git config--global user.name: Serve para armazenar as informações sobre você no Git, como o e-mail e o seu nome, consegue criar “apelidos” para os seus comandos e até mesmo trocar a cor das ações do Git.

Faça commit:
$ git config user.name > Bolinhos 
$ git config user.name > Bolinhos 


git config--global user.emailS: Serve para você modificar o arquivo de texto de configurações que está localizado no seu pc. Podemos configurar informações globais como e-mail,nome de usuário e o editor de texto padrão.

Faça commit:
$ git config --global user.email "email@example.com"

git remote add origin: Serve para gerenciar repositórios remotos inclui saber como adicionar-los remotamente, removedor que não são mais válidos, gerenciar vários ramos(ramos) e definí-los como rastreados ou não e muito mais. Nesta seção, abordaremos algumas habilidades de gereciamento remoto.

Faça commit: 
$ git remote add origin https://github.com/user/repo.git # Defina um novo remote $ git remote -v # Verifique o novo remote > origin https://github.com/user/repo.git (fetch) > origin https://github.com/user/repo.git (push)

git status: Serve para verifica quais os estados que os arquivos estão. Se existe algum arquivo modificado, adiciona ou removido. Além disso, caso esteja rastreado com uma branch no servidor, verifica se a versão está a frente ou atrás da versão do servidor.

Faça commit: 
# Edit hello.py
git status
# hello.py is listed under "Changes not staged for commit"
git add hello.py
git status
# hello.py is listed under "Changes to be committed"
git commit
git status
# nothing to commit (working directory clean)

git log: Serve para que você liste e filtre o histórico do projeto e pesquise alterações específicas.

Faça commit:
git log --author="Unicornio" -p hello.py

git add: Serve para adicionar o conteúdo atual dos caminhos existentes como um todo, mas com algumas opções também pode ser usado para adicionar o conteúdo com apenas uma parte das alterações aplicadas nos arquivos da árvore de trabalho ou remover os caminhos que não existem mais na árvore de trabalho.

Faça commit:
git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p] 	 [--edit | -e] [- [não-] todos | - [no-] ignorar-remoção | [--update | -você]] 	 [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormalize] 	 [--chmod = (+ | -) x] [--pathspec-from-file = <arquivo> [--pathspec-file-nul]] 	 [-] [<pathspec>…]


git commit: Serve para capturar o estado de um projeto naquele momento.

Faça commit:
git commit
git commit -a
git commit -m "commit message"
git commit -am "commit message"
git commit --amend

git push: Serve para publicar modificações locais a um repositório central. 

Faça commit:
git push <remote> <branch>
git push <remote> --force
git push <remote> --all
git push <remote> --tags
