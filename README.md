# Individual4
Trabalho individual módulo 4 do curso Programadores Cariocas.


Proposta do trabalho:
A Resilia está pensando em lançar um novo sistema de acompanhamento e para isso precisa de ajuda para modelar um banco de dados que vai armazenar seus cursos, turmas e alunos.
Para apoiar nesse sistema recebemos a tarefa de realizar essa modelagem
e responder algumas perguntas com nosso modelo:

1. Existem outras entidades além dessas três?
Sim. No modelo criado para a solução deste minimundo, foi criado também a entidade "Resilia".

2. Quais são os principais campos e tipos?
Entidade Resilia(
  id_resilia serial primary key,
  campus varchar(20) not null
);

Entidade Cursos(
  id_curso serial primary key,
  nome varchar(20) not null,
  coordenador
);

Entidade Turmas(
  id_turmas serial primary key,
  qtd_alunos int
);

Entidade Alunos(
  id_alunos serial primary key,
  nome varchar(30) not null,
  idade int not null,
  rg varchar(11) not null
);
  
  

3. Como essas entidades estão relacionadas?

Segue imagem representando o modelo desde BD:

![Imagem do WhatsApp de 2023-02-28 à(s) 13 35 14](https://user-images.githubusercontent.com/83782674/221925982-a9c92575-ba97-451a-9b56-3f39e597f19a.jpg)

Cardinalidade:

Resilia pode ter um ou vários cursos;
Curso pertence a um e somente um resilia;
Curso pode produzir uma ou várias turmas;
Turma pertence a um e somente um curso;
Turma contém um ou vários alunos;
Alunos contém um ou vários cursos.

Registros:

imagem 1
imagem 2
imagem 3
imagem 4

