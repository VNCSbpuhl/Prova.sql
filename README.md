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
![Conceitual](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/8ef3a855-7ea5-4b52-9dc0-681e6e5d6d8e)



# 💻 Modelagem Lógica
![lógico](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/41ee6538-5b03-494e-afb7-ad1254a6ce1d)




# 💻 Dados

Os dados inseridos nas tabelas estão no arquivo dados.sql



# 💻 CRUD
## Create
![Create](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/c26a0783-6b7c-45ab-bfdb-5a17d9dca2a8)

## Delete
![Delete](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/365537d4-096a-4fea-ab9b-6c84f45f6c94)

## Read
![Read](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/289c9d16-738e-4c78-91a0-28adf95e325d)

## Update
![Update](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/f24ca6ee-268b-4268-8831-ab680ef77b7e)





# 💻 Relatórios

#### 1 - Selecione os alunos que começam com C
![Relatórios 1](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/7b8a1d29-27dd-4b8b-9bc8-dede84087b19)


#### 2 - Selecione as turmas do periodo noturno
![Relatórios 2](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/a4145e41-258a-401a-b0bd-35bfa6c2d1da)


#### 3 - Selecione todos os alunos da Cidade B
![Relatórios 3](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/fb9951b8-0ca3-46bb-a203-1ace614c5385)


#### 4 - Selecione todos os alunos que possuem a letra B no nome
![Relatórios 4](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/544aa99a-22e7-4351-beeb-62d3a0985cc7)


#### 5- Selecione todas as disciplinas com mais de 30 de carga horaria
![Relatórios 5](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/4b06fefb-8956-4bd4-80cc-230281865e16)


#### 6- Selecione todas as disciplinas
![Relatórios 6](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/5c5dc41c-bf4a-46e5-96ba-4d2c59892d92)


#### 7 - Selecione as disciplinas com 45 de carga horaria
![Relatórios 7](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/ac92981b-2275-4eb7-8419-199d18159851)


#### 8 - Selecione os alunos nascidos em 1999 e 2001
![Relatórios 8](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/63efc0b1-891e-4a81-8343-b71c1b1e6404)


#### 9 - Selecione os alunos nascidos em 2001 na Cidade A
![Relatórios 9](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/da3dd498-56cb-4268-a929-99b4c0fb566a)


#### 10 - Selecione os professores que começam com a letra J
![Relatórios 10](https://github.com/VNCSbpuhl/Prova.sql/assets/141787258/215535db-eac4-4fff-96ed-065389a01ce2)

























