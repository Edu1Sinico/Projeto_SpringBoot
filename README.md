# Projeto SpringBoot- Aprendizagem e Revisão

Projeto dedicado para aprendizagem e revisão de conteúdos de SpringBoot, utilizando vídeos disponibilizados gratuitamente pelo canal do professor Rogério Napoleão Jr.

>**Playlist do Projeto**
- Link: [Projeto utilizando SpringBoot - Prof. Rogério Napoleão Jr](https://www.youtube.com/playlist?list=PL6-iiksdrDYz_Fh_WZxmPORTiQtO0QYMz)
<br>

>**Estrutura e Ferramentas Back-End do Projeto SpringBoot**

Este projeto utilizará a arquitetura SpringBoot 4.0.3 com a versão do Java 17. Além disso, estarei utilizando o banco de dados PostgreSQL e a seguinte estrutura back-end (Layered Architecture):

- **Repository**: Responsável pela comunicação direta com o banco de dados. Essa camada realiza operações como salvar, buscar, atualizar e deletar informações, utilizando o Spring Data JPA para facilitar o acesso aos dados.
- **Service**: Contém a lógica de negócio da aplicação. Essa camada processa as informações recebidas do Controller, aplica regras e utiliza o Repository para acessar ou modificar os dados.
- **Controller**: Responsável por receber as requisições HTTP do cliente (como GET, POST, PUT e DELETE) e retornar as respostas. Atua como ponto de entrada da aplicação, conectando o front-end com o back-end.
- **Entity**: Representa as tabelas do banco de dados. Cada classe Entity corresponde a uma tabela, e seus atributos representam as colunas, permitindo que o Spring gerencie os dados automaticamente.
- **DTO**: Utilizado para transferir dados entre as camadas da aplicação. O DTO ajuda a controlar quais informações serão enviadas ou recebidas, aumentando a segurança e organização do sistema.
