# <center> Relação de entidades:
![Alt text](image-7.png)

```python
{
	"alunos": [
	    {
			"id": 1,
			"nome": "Mateus",
			"cursos_id": [1, 3],
			"notas": [
				{
					"id_curso": 1,
					"id_turma": 1,
					"notas": [5, 6.23, 10],
					"ffe": null
				},
				{
					"id_curso": 3,
					"id_turma": 4,
					"notas": [5, 8],
					"ffe": null

				}
			]
		}
	]
}

```

Nessa relação temos que um **aluno** pode estar matriculado em **diferentes** cursos, o **aluno mateus** tem **duas listas de notas, uma para cada curso matriculado**.

Dessa forma será possível fazer a média e adquirir estatísticas de notas de diferentes cursos e turmas.

## <center> Tabelas de banco de dados:
**1. Dados de Cursos:**

cursos (array): Contém informações sobre os cursos disponíveis.
id (inteiro): ID único do curso.
nome_curso (string): Nome do curso.
professor (string): Nome do professor responsável pelo curso.
qtd_sprint (inteiro): Quantidade de sprints associadas ao curso.
turmas (array de inteiros): IDs das turmas relacionadas ao curso.

**2. Dados de Turmas:**

turmas (array): Contém informações sobre as turmas.
id (int): ID único da turma.
id_curso (inteiro): ID do curso ao qual a turma está associada.
nome_turma (string): Nome da turma.

**3. Dados de Grupos:**

id (int): ID único do grupo.
id_curso (inteiro): ID do curso ao qual o grupo está associado.
id_turma (inteiro): ID da turma à qual o grupo pertence.
nome_grupo (string): Nome descritivo do grupo.
alunos (array de inteiros): Uma lista de IDs de alunos que fazem parte deste grupo.
 
**4. Dados de Alunos:**

alunos (array): Contém informações sobre os alunos matriculados em cursos.
id (int): ID único do aluno.
nome (string): Nome do aluno.
cursos_id (array de inteiros): IDs dos cursos aos quais o aluno está matriculado.
notas (array de objetos): Contém informações sobre as notas do aluno em diferentes cursos e    turmas.
id_curso (inteiro): ID do curso relacionado às notas.
id_turma (inteiro): ID da turma relacionada às notas.
notas (array de números): Lista de notas obtidas pelo aluno no curso e turma específicos.
ffe (nulo ou qualquer outro valor): Média das notas.
 
 
# <center> **BACKLOG API (2 SPRINT):**
 
### **Épico 1: Gerenciamento de curso e turma:**

#### **História de Usuário 1: Como um administrador, eu quero criar um novo curso.**

1. Criar tela inicial que encaminhe para a administração de um curso.

2. Na tela deve aparecer os cursos cadastros e ter a opção de cadastrar novo curso.

3. Para cadastrar um curso será necessário no mínimo adicionar seu nome e o professor responsável.

4. Criar validação para que o nome do curso não seja repetido.

5. Demais opções de curso são: quantidade de sprints e selecionar quantas turmas ele quer criar (**banco de dados = bdd** então bdd1, bdd2, ..., bdd5).

6. Operações CRUD (Create, Read, Update, Delete).

7. Campo para procurar um curso existente.
 
 
#### **História de Usuário 2: Como um administrador, eu quero adicionar uma turma a um curso.**

1. Criar tela de administração de turmas.

2. Na tela deve aparecer turmas cadastrar e ter a opção de cadastrar nova turma.

3. Para cadastrar uma turma é necessário escolher um curso.

4. Operações CRUD (Create, Read, Update, Delete)

5. Campo para procurar uma turma existente.

6. Teste para ver se o relacionamento entre o curso e a turma então corretos.
 
#### **História de Usuário 3: Como um administrador, eu quero adicionar um aluno a uma turma.**
 
1. Criar tela de administração de alunos.
 
#### **História de Usuário 4: Como um administrador, eu quero adicionar um aluno a um grupo.**
 
 
### **Épico 2:  Rotas de API:**

#### **História de Usuário 1: Como administrador eu quero configurar meus cursos**

1. Necessário criar as rotas para que o front end consiga fazer o croud

2. Documentar as rotas e suas funções

3.        

