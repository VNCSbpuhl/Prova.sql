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

```
INSERT INTO aluno (id_aluno, nome, data_nac, rua, numero, bairro, cidade)
VALUES
(1, 'João Silva', '2000-05-15', 'Rua A', 123, 'Centro', 'Cidade A'),
(2, 'Maria Oliveira', '1999-08-22', 'Rua B', 456, 'Bairro X', 'Cidade B'),
(3, 'Carlos Pereira', '2001-02-10', 'Rua C', 789, 'Bairro Y', 'Cidade C'),
(4, 'Ana Santos', '1998-11-30', 'Rua D', 321, 'Bairro Z', 'Cidade A'),
(5, 'Pedro Souza', '2002-07-05', 'Rua E', 654, 'Bairro X', 'Cidade B'),
(6, 'Lucia Mendes', '1997-04-18', 'Rua F', 987, 'Bairro Y', 'Cidade C'),
(7, 'Fernando Lima', '2003-09-25', 'Rua G', 234, 'Bairro Z', 'Cidade A'),
(8, 'Julia Almeida', '1996-12-12', 'Rua H', 567, 'Bairro X', 'Cidade B'),
(9, 'Marcos Rocha', '2004-01-08', 'Rua I', 876, 'Bairro Y', 'Cidade C'),
(10, 'Camila Costa', '1995-06-20', 'Rua J', 321, 'Bairro Z', 'Cidade A'),
(11, 'Rafaela Nunes', '2000-03-17', 'Rua K', 654, 'Bairro X', 'Cidade B'),
(12, 'Gabriel Oliveira', '1999-10-02', 'Rua L', 987, 'Bairro Y', 'Cidade C'),
(13, 'Sergio Silva', '2001-07-14', 'Rua M', 234, 'Bairro Z', 'Cidade A'),
(14, 'Isabela Pereira', '1998-04-28', 'Rua N', 567, 'Bairro X', 'Cidade B'),
(15, 'Roberto Santos', '2002-11-09', 'Rua O', 876, 'Bairro Y', 'Cidade C'),
(16, 'Cristina Souza', '1997-08-03', 'Rua P', 123, 'Bairro Z', 'Cidade A'),
(17, 'Vinicius Mendes', '2003-05-27', 'Rua Q', 456, 'Bairro X', 'Cidade B'),
(18, 'Tatiane Lima', '1996-02-14', 'Rua R', 789, 'Bairro Y', 'Cidade C'),
(19, 'Eduardo Almeida', '2004-09-01', 'Rua S', 321, 'Bairro Z', 'Cidade A'),
(20, 'Amanda Rocha', '1995-12-24', 'Rua T', 654, 'Bairro X', 'Cidade B');
```

```
INSERT INTO professor (id_profe, nome, data_nac, rua, numero, bairro, cidade)
VALUES
(1, 'Carlos Oliveira', '1975-08-10', 'Rua A', 123, 'Centro', 'Cidade A'),
(2, 'Maria Silva', '1980-04-22', 'Rua B', 456, 'Bairro X', 'Cidade B'),
(3, 'Lucas Pereira', '1978-12-05', 'Rua C', 789, 'Bairro Y', 'Cidade C'),
(4, 'Ana Costa', '1985-06-30', 'Rua D', 321, 'Bairro Z', 'Cidade A'),
(5, 'Roberto Souza', '1973-11-15', 'Rua E', 654, 'Bairro X', 'Cidade B'),
(6, 'Juliana Mendes', '1982-07-18', 'Rua F', 987, 'Bairro Y', 'Cidade C'),
(7, 'Fernando Lima', '1970-03-25', 'Rua G', 234, 'Bairro Z', 'Cidade A'),
(8, 'Mariana Almeida', '1979-12-12', 'Rua H', 567, 'Bairro X', 'Cidade B'),
(9, 'Rafael Rocha', '1988-01-08', 'Rua I', 876, 'Bairro Y', 'Cidade C'),
(10, 'Camila Costa', '1972-06-20', 'Rua J', 321, 'Bairro Z', 'Cidade A'),
(11, 'Gustavo Nunes', '1987-03-17', 'Rua K', 654, 'Bairro X', 'Cidade B'),
(12, 'Carla Oliveira', '1984-10-02', 'Rua L', 987, 'Bairro Y', 'Cidade C'),
(13, 'Sergio Silva', '1976-07-14', 'Rua M', 234, 'Bairro Z', 'Cidade A'),
(14, 'Isabela Pereira', '1983-04-28', 'Rua N', 567, 'Bairro X', 'Cidade B'),
(15, 'Roberto Santos', '1989-11-09', 'Rua O', 876, 'Bairro Y', 'Cidade C'),
(16, 'Cristina Souza', '1977-08-03', 'Rua P', 123, 'Bairro Z', 'Cidade A'),
(17, 'Vinicius Mendes', '1990-05-27', 'Rua Q', 456, 'Bairro X', 'Cidade B'),
(18, 'Tatiane Lima', '1974-02-14', 'Rua R', 789, 'Bairro Y', 'Cidade C'),
(19, 'Eduardo Almeida', '1992-09-01', 'Rua S', 321, 'Bairro Z', 'Cidade A'),
(20, 'Amanda Rocha', '1971-12-24', 'Rua T', 654, 'Bairro X', 'Cidade B');
```

```
INSERT INTO disciplina (id_disciplina, nome, carga_horaria)
VALUES
(1, 'Matemática', 60),
(2, 'Português', 45),
(3, 'História', 30),
(4, 'Geografia', 45),
(5, 'Ciências', 60),
(6, 'Inglês', 30),
(7, 'Artes', 45),
(8, 'Educação Física', 60),
(9, 'Química', 45),
(10, 'Física', 60),
(11, 'Biologia', 45),
(12, 'Filosofia', 30),
(13, 'Sociologia', 30),
(14, 'Programação', 60),
(15, 'Economia', 45),
(16, 'Gestão de Projetos', 45),
(17, 'Psicologia', 30),
(18, 'Comunicação', 45),
(19, 'Marketing', 60),
(20, 'Estatística', 30);
```

```
INSERT INTO nota (id_nota, valor, dt_prova)
VALUES
(1, 7.5, '2023-01-15'),
(2, 8.0, '2023-02-20'),
(3, 6.5, '2023-03-10'),
(4, 9.2, '2023-04-05'),
(5, 5.8, '2023-05-12'),
(6, 7.0, '2023-06-18'),
(7, 8.5, '2023-07-25'),
(8, 6.0, '2023-08-03'),
(9, 9.0, '2023-09-14'),
(10, 7.8, '2023-10-20'),
(11, 8.2, '2023-11-02'),
(12, 6.9, '2023-12-10'),
(13, 9.5, '2024-01-15'),
(14, 7.3, '2024-02-20'),
(15, 8.7, '2024-03-10'),
(16, 6.4, '2024-04-05'),
(17, 9.8, '2024-05-12'),
(18, 7.1, '2024-06-18'),
(19, 8.3, '2024-07-25'),
(20, 6.7, '2024-08-03');
```

```
INSERT INTO turma (id_turma, ano, periodo)
VALUES
(1, 2021, 'diurno'),
(2, 2022, 'noturno'),
(3, 2020, 'diurno'),
(4, 2023, 'noturno'),
(5, 2022, 'diurno'),
(6, 2021, 'noturno'),
(7, 2020, 'diurno'),
(8, 2023, 'noturno'),
(9, 2020, 'diurno'),
(10, 2021, 'noturno'),
(11, 2023, 'diurno'),
(12, 2022, 'noturno'),
(13, 2021, 'diurno'),
(14, 2020, 'noturno'),
(15, 2022, 'diurno'),
(16, 2023, 'noturno'),
(17, 2020, 'diurno'),
(18, 2021, 'noturno'),
(19, 2022, 'diurno'),
(20, 2023, 'noturno');
```




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

























