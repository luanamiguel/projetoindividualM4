# projetoindividualM4


Para apoiar nesse sistema recebemos a tarefa de realizar essa modelagem e responder algumas perguntas com nosso modelo:

⇨ Existem outras entidades além dessas três? Sim. Instrutores e disciplinas, por exemplo.

⇨ Quais são os principais campos e tipos? Na tabela curso é o: id_curso, tipo int. Na tabela turma é o: id_turma, tipo int. Na tabela aluno é o: id_aluno, tipo int.

⇨ Como essas entidades estão relacionadas? O curso tem turmas e as turmas têm alunos.

Utilizando o shell do app XAMPP: Criar o banco de dados com o comando: create database projeto_individual;

Verificar o banco de dados criado: show databases;

Acessar o banco de dados criado: use projeto_individual;

Criar tabela curso:
create table curso ( id_curso int primary key, carga_horaria int, matricula varchar(50), disciplina varchar(50));

Criar tabela turma:
create table turma ( id_turma int primary key, id_orientador int, sala varchar(30), turno varchar(30));

Criar tabela aluno:
create table aluno ( id_aluno int primary key, nome varchar(100), cpf int, nota float);
