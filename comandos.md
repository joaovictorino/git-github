# Comandos Git

## Aula 01

### Git clone
````sh
git clone [url repositório] [pasta (opcional)] # Copia um repositório de um local remoto.
````

### Git log
````sh
git log [--oneline|--stat|--patch] # Mostra o histórico de commits.
git log [commit id|commit tag|main]..[commit id|commit tag|origin/main]
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
````sh
git restore [caminho do arquivo no working directory] # Desfaz mudanças de estados do “staging” e “working directory”.
git restore --staged [caminho do arquivo no staging]
````

### Git diff
````sh
git diff # Mostra a diferença entre arquivos e commits.
git diff --staged
git diff [commit id|commit tag|main] [commit id|commit tag|origin/main]
````

### Git pull
````sh
git pull # Puxa as alterações de um repositório remoto.
git pull --no-ff
````

### Git push
````sh
git push # Empurra alterações para um repositório remoto.
````

### Git fetch
````sh
git fetch # Busca atualizações do repositório remoto, sem alterar o repositório local.
````

### Git stash
````sh
git stash --message=[mensagem descritiva do stash] # Salva suas alterações atuais em um armazenamento temporário.
git stash list
git stash pop
````

## Aula 02
