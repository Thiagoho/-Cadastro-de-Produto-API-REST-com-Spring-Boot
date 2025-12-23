## Desafio 1 — Cadastro de Produto (API REST com Spring Boot)
### Descrição

Este projeto é o primeiro desafio da minha jornada de estudos em backend com foco no padrão arquitetural MVC (Model-View-Controller) utilizando Spring Boot. A aplicação simula um sistema simples de cadastro de produtos com três atributos principais: nome, preço e quantidade em estoque.
### Funcionalidades
A API permite:<br>
== Cadastrar um novo produto<br>
== Listar todos os produtos cadastrados<br>
== Buscar um produto pelo ID<br>
== Atualizar dados de um produto existente<br>
== Excluir um produto<br>
## Estrutura do Projeto
 src/main/java/com/example/<br>
├── controller/      # Camada responsável por lidar com as requisições HTTPo<br>
├── dto/             # Representações de dados trafegados entre cliente e servidoro<br>
├── model/           # Entidade Produtoo<br>
├── repository/      # Interface com o banco de dadoso<br>
└── service/         # Regras de negócioo<br>
## Entidade
 Produto<br>
├── String nome<br>
├── Double preco<br>
└── Integer quantidade
## Regras de Negócio
Nome do produto não pode ser vazio.<br>
Preço e quantidade devem ser maiores ou iguais a zero.<br>
Ao excluir ou atualizar um produto, o sistema deve verificar se ele existe.
## Tecnologias Utilizadas
Java 17+<br>
Spring Boot<br>
Spring Web<br>
Spring Data JPA<br>
(Opcional) H2 Database ou MySQL<br>
Maven
## Como Executar
Clone o projeto:<br>
git clone https://github.com/seu-usuario/seu-repositorio.git<br>
Abra no Eclipse, IntelliJ ou outro IDE compatível com Spring Boot.<br>
Execute a classe Application.java.<br>
Teste os endpoints usando:<br>
Postman<br>
Insomnia<br>
Ou diretamente via Swagger (se estiver configurado)
## Endpoints REST
Método	Endpoint	       Descrição<br>
GET	   /produtos	     Lista todos os produtos<br>
GET 	/produtos/{id}	 Busca produto por ID<br>
POST	/produtos	       Cadastra novo produto<br>
PUT	  /produtos/{id}	  Atualiza produto<br>
DELETE	/produtos/{id}	Remove produto<br>
### *Autor*
Thiago Henrique de Oliveira Sales <br>
GitHub

