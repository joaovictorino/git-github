# Comandos Git

## Aula 01

### Git clone
````sh
git clone [url repositório] [pasta (opcional)] # Copia um repositório de um local remoto.
````

### Git log
````sh
git log [--oneline|--stat|--patch] # Mostra o histórico de commits.
````

### Git config
````sh
git config [--global|--local] [chave] [valor] # Configura vários aspectos do Git.
git config --list
````

### Git add
````sh
git add [caminho do arquivo] # Adiciona alterações à área de “staging”.
git add .
````

### Git commit
````sh
git commit -m [mensagem descritiva do commit] # Confirma as alterações no repositório local.
git commit [caminho do arquivo em staging] -m [mensagem descritiva do commit]
git commit -a -m [mensagem descritiva do commit]
````

### Git status
````sh
git status # Verifica a situação do “staging” e “working directory”.
````

### Git restore

git diff: Show the difference between files.
git pull: Pull changes from a remote repository.
git push: Push changes to a remote repository.
git fetch
git stash

## Aula 02
