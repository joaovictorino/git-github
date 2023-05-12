# Comandos Git

### Git clone
````sh
git clone [url repositório] [pasta (opcional)] # Copia um repositório de um local remoto.
git clone [caminho no disco do repositório] # Pode clonar repositórios remotos e locais.
````

### Git log
````sh
git log [--oneline|--stat|--patch] # Mostra o histórico de commits.
git log [commit id|commit tag|main]..[commit id|commit tag|origin/main]
git log --graph # Mostra o histórico de commit e merges com branchs que foram feitos.
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
git restore --source [id commit] [caminho arquivo] # Desfaz mudanças em um arquivo e um commit específico.
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
git push [origem remota] [nome do branch] # Empurra commits e branch para uma origem remota.
git push [origem remota] --delete [nome do branch] # Apaga um branch na origem remota.
git push --tags
git push --all
git push --force
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
git stash drop
````

### Git revert
````sh
git revert [id commit] # Desfaz o commit diretamente no repositório.
````

### Git show
```sh
git show [id commit] # Mostra detalhadamente o commit.
```

### Git checkout
```sh
git checkout [id commit] # Navega pelo histórico do projeto, assim como em branchs e tags.
git checkout [branch]
git checkout [nome da tag]
```

### Git branch
```sh
git branch [nome do branch] # Cria um novo branch a partir do branch atual que estamos.
git branch -d [nome do branch] # Apaga um branch localmente.
```

### Git switch
```sh
git switch [nome branch] # Navega entre branchs assim como o "git checkout".
```

### Git merge
```sh
git merge [nome do branch] # Busca os commits de outro branch mesclando com o branch atual.
```

### Git tag
```sh
git tag [nome da tag] -m [mensagem da tag] # Cria uma marcação no histórico do projeto, uma etiqueta vinculada a um commit.
git tag [nome da tag] [codigo commit] -m [mensagem da tag]
```

### Git init
```sh
git init # Inicializa uma pasta para o git.
git init --bare # Inicializa uma pasta para o git como servidor.
```

### Git remote
```sh
git remote -v # Lista, cadastra e remove as origens remotas.
git remote add [nome da origem] [endereço]
git remote remove [nome da origem]
```

### Git blame
```sh
git blame [caminho do arquivo] # Mostra quem criou ou alterou cada linha do arquivo.
```

### Git rebase
```sh
git rebase [nome do branch] # Busca os commits e mescla com o repositório atual, mexendo no histórico.
git rebase -i [ponteiro HEAD] # Reescreve o histórico do projeto.
```

### Git cherry-pick
```sh
git cherry-pick [id commit] # Busca um commit de qualquer branch e mescla com o atual.
```

### Git reset
```sh
git reset --soft [ponteiro HEAD] # Apaga commit do repositório, trazendo para staging, working directory ou removendo de vez.
git reset --mixed [ponteiro HEAD]
git reset --hard [ponteiro HEAD]
```
