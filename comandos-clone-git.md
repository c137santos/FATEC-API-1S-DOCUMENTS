## Comandos para executar o clone no git

### Passo 1: pegando o link do repositório 
Ir no repositório do GitHub e clicar em "code", depois https e copiar o link.

### Passo 2: criando uma pasta para o repositório
Ir no terminar (Windows Power Shell) e criar uma pasta:

````shell
mkdir Pasta
cd Pasta
```` 

### Passo 3: clonando o repositório e abrindo no VSCode

````shell
git clone copiar-o-link-obtido-do-github
cd nome-do-projeto
git fetch origin
git checkout -b nome-do-projeto origin/nome-do-projeto
git branch -a
git pull
code .
````

### Passo 4: comitando no repositório após as alterações
Após fazer as alterações no código seguir os proximos passos para comitar:

````shell
git add . 
commit -m adicionar-novo-arquivo
git push
````

