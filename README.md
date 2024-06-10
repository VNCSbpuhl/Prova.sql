# 💻 Prova Modelagem de Banco de Dados

Trabalho final para a disciplina Modelagem de Banco de Dados do 1° Semestre de Desenvolvimento de Software Multiplataforma.

# 💻 Cenário

Uma escola deseja implementar um sistema de gestão escolar para acompanhar informações sobre alunos, professores, disciplinas, notas e turmas. O objetivo é facilitar a administração escolar, fornecendo uma maneira eficiente de gerenciar e organizar dados relacionados ao corpo discente, docente e às atividades acadêmicas. 

#### Entidade: Aluno

Atributos:
ID (PK, int); Nome (varchar); Data de Nascimento (date); Endereço (varchar); E-mail (varchar); Telefone (varchar)

#### Entidade: Professor

Atributos:
ID (PK, int); Nome (varchar); Especialidade (varchar); E-mail (varchar); Telefone (varchar)

#### Entidade: Disciplina

Atributos:
ID (PK, int;) Nome (varchar); Carga Horária (int)

#### Entidade: Nota

Atributos:
ID (PK, int); Valor (decimal); Data da Avaliação (date)
Chaves Estrangeiras:
Aluno_ID (FK referenciando Aluno); Disciplina_ID (FK referenciando Disciplina)

#### Entidade: Turma

Atributos:
ID (PK, int); Ano (int); Período (varchar)
Chave Estrangeira:
Professor_ID (FK referenciando Professor)

# 💻 Modelagem Conceitual



# 💻 Modelagem Lógica




# 💻 Dados

Os dados inseridos nas tabelas estão no arquivo dados.sql



# 💻 CRUD
## Create

## Delete

## Read

## Update





# 💻 Relatórios

#### 1 - Selecione os alunos que começam com C


#### 2 - Selecione as turmas do periodo noturno


#### 3 - Selecione todos os alunos da Cidade B


#### 4 - Selecione todos os alunos que possuem a letra B no nome


#### 5- Selecione todas as disciplinas com mais de 30 de carga horaria


#### 6- Selecione todas as disciplinas


#### 7 - Selecione as disciplinas com 45 de carga horaria


#### 8 - Selecione os alunos nascidos em 1999 e 2001


#### 9 - Selecione os alunos nascidos em 2001 na Cidade A


#### 10 - Selecione os professores que começam com a letra J

























