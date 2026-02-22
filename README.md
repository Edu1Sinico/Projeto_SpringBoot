# Projeto SpringBoot - Aprendizagem e Revisão

Projeto dedicado para aprendizagem e revisão de conteúdos de SpringBoot, utilizando vídeos disponibilizados gratuitamente pelo canal do professor Rogério Napoleão Jr.

>**Ordem dos Vídeos**
- [CRIANDO UM SISTEMA BACKEND COM SPRING BOOT](https://www.youtube.com/watch?v=vZx7EvnUwLs)
- [ENTENDENDO A ESTRUTURA PADRÃO DE UM PROJETO EM SPRING BOOT](https://www.youtube.com/watch?v=Nbtzy7o3pPg)
- [CRIANDO SUA ESTRUTURA INICIAL EM PROJETO JAVA SPRING BOOT - PADRÃO DE PROJETO](https://www.youtube.com/watch?v=5dT1hczY_yU)
- [O QUE É JPA E HIBERNATE E COMO FAZER UM MAPEAMENTO COM JPA](https://www.youtube.com/watch?v=8qP06yVj5JU)
- [QUAL O PAPEL DO DTO E DO ENTITY EM UM PROJETO JAVA SPRING BOOT?](https://www.youtube.com/watch?v=ninjPTQjNSI)
- [O QUE SÃO AS OPERAÇÕES CRUD E COMO IMPLEMENTAR NO SPRING BOOT?](https://www.youtube.com/watch?v=kox99rwtwoo)
<br>

>**Estrutura e ferramentas Back-End do Projeto SpringBoot**

Este projeto utilizará a arquitetura SpringBoot 4.0.3 com a versão do Java 17. Além disso, estarei utilizando o banco de dados PostgreSQL e a seguinte estrutura back-end (Layered Architecture):

- **Repository**: Responsável pela comunicação direta com o banco de dados. Essa camada realiza operações como salvar, buscar, atualizar e deletar informações, utilizando o Spring Data JPA para facilitar o acesso aos dados.
- **Service**: Contém a lógica de negócio da aplicação. Essa camada processa as informações recebidas do Controller, aplica regras e utiliza o Repository para acessar ou modificar os dados.
- **Controller**: Responsável por receber as requisições HTTP do cliente (como GET, POST, PUT e DELETE) e retornar as respostas. Atua como ponto de entrada da aplicação, conectando o front-end com o back-end.
- **Entity**: Representa as tabelas do banco de dados. Cada classe Entity corresponde a uma tabela, e seus atributos representam as colunas, permitindo que o Spring gerencie os dados automaticamente.
- **DTO**: Utilizado para transferir dados entre as camadas da aplicação. O DTO ajuda a controlar quais informações serão enviadas ou recebidas, aumentando a segurança e organização do sistema.
