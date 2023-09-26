# [JSON (JavaScript Object Notation):](https://www.json.org/json-en.html)
O JSON é um formato de dados que é comumente usado para trocar informações estruturadas entre sistemas. Ele é fácil de ler e escrever tanto para humanos quanto para máquinas. Um arquivo JSON possui as seguintes características:

- **Sintaxe**:
    
	 - O JSON é baseado em pares de chave-valor. Os dados são armazenados em um formato semelhante a um dicionário em Python ou um objeto em JavaScript.
	- A chave é sempre uma string, seguida por dois pontos (`:`), e o valor pode ser de qualquer tipo de dado suportado pelo JSON (string, número, booleano, array, objeto, null).

````json
{ 
	"nome": "João",
	"idade": 30, 
	"casado": true, 
	"interesses": ["música", "viagem", "esportes"], 
	"endereço": { 
		"rua": "123 Main Street", 
		"cidade": "São Paulo", 
		"estado": "SP" 
	}
}
````

- Uso:
	- O JSON é frequentemente usado para configurar aplicativos, transmitir dados pela web e armazenar informações estruturadas em arquivos.

- **Vantagens**:
	- Suporta dados aninhados e estruturas complexas.
	- Pode representar diferentes tipos de dados, como strings, números, listas, objetos, etc.
	- É fácil de entender e ler.
	- É usado para configurações de aplicativos e troca de dados entre sistemas.
- **Desvantagens**:
	- Pode ser menos eficiente em termos de espaço quando comparado ao CSV para grandes conjuntos de dados tabulares simples.


# [CSV (Comma-Separated Values):](https://docs.python.org/3/library/csv.html)

O CSV é um formato simples para armazenar dados em formato tabular, onde as colunas são separadas por vírgulas e as linhas são separadas por quebras de linha. Cada linha representa um registro e cada campo (valor) é separado por uma vírgula.

- **Sintaxe**:
    
	- Os valores são separados por vírgulas (daí o nome "Comma-Separated Values").
	- Pode haver uma linha de cabeçalho que define os nomes das colunas.

````plaintext
Nome,Idade,Email
Sara,30,saranahra@hotmail.com 
Caio,33,caiopalma@gmail.com
````

- Uso:
	- O CSV é comumente utilizado para armazenar e compartilhar dados tabulares, como planilhas ou conjuntos de dados estruturados. Ele é amplamente suportado por planilhas e aplicativos de banco de dados.

- **Vantagens**:
	- É eficiente para grandes conjuntos de dados tabulares simples.
	- É fácil de ser lido e editado em qualquer editor de texto.
	- Amplamente suportado por planilhas e bancos de dados.
- **Desvantagens**:
	- Não suporta estruturas de dados complexas diretamente (como objetos aninhados).

**Resumo:**  A escolha entre JSON e CSV dependerá do tipo de dados que você está manipulando e das necessidades específicas do seu aplicativo ou uso. JSON é mais adequado para dados complexos e aninhados, enquanto CSV é excelente para dados tabulares simples e eficiência de armazenamento.


https://docs.python.org/3/library/csv.html

https://www.json.org/json-en.html
