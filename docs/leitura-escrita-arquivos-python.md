A leitura e escrita de um arquivo pode ser feita de vários modos, sendo as mais usuais, w (write), r (read) e a (append).

## Modo "w" (write):
- O modo "w" é usado para criar um arquivo novo ou substituir o conteúdo de um arquivo existente. Se o arquivo já existir, o modo "w" irá apagar o conteúdo anterior e começar com um arquivo em branco.
- Se o arquivo especificado não existir, o Python irá criá-lo.
- O uso do **encoding =”utf-8”** é utilizado para que o Python consiga ler corretamente as informações que possuem acento.

````Python
with open ('arquivo.txt', 'w', encoding =”utf-8”) as arquivo:
	arquivo.write('Este é um exemplo de escrita em Python. \n')
````
## Modo "r" (read):
- O modo "r" é usado para abrir um arquivo existente para leitura.
- Se o arquivo especificado não existir, o Python irá gerar um erro.

````Python
with open('arquivo.txt', 'r', encoding =”utf-8”) as arquivo: 
	conteudo = arquivo.read() 
	print(conteudo)
````
## Modo "a" (append)
- O modo "a" é usado para abrir um arquivo existente ou criar um novo arquivo se ele não existir, mas a diferença principal em relação ao modo "w" é que o "a" não apaga o conteúdo existente. Ele permite adicionar novos dados ao final do arquivo.

````Python
with open('arquivo.txt', 'a', encoding =”utf-8”) as arquivo:
	arquivo.write('Este é um conteúdo que será adicionado ao arquivo. \n')
````
Sempre é uma boa prática usar a instrução `with` (gerenciador de contexto) ao lidar com arquivos em Python, pois ela garante que o arquivo seja fechado corretamente após a execução do bloco de código, mesmo se ocorrerem exceções durante o processamento do arquivo. Isso ajuda a evitar problemas como vazamento de recursos.
