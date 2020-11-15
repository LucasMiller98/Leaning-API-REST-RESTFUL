# Leaning-API-REST-RESTFUL
Leaning API, REST and RESTFUL with Rocketseat(NodeJS)

# API, REST and RESTFUL

# API

API -> Aplication programming interface(interface de programação de aplicações). É um conjunto de rotinas e padrões  que uma aplicação disponibiliza para outras aplicações pegam essas informações

Cliente(client) -> APP
garçon(pedidos, levar seus pedidos, para a cozinha) (API)
Cozinha(server)

- Responsável por estabelecer comunicações entre diferentes serviços.
- Meio de campo entre as tecnologias
- Intermiador para trocar informações

## REST

Um acrônimo para representational State Transfer(Transferência de Estado Representativo).

Será feita a transferência de dados de uma maneira simbólica, figurativa, representativa, de maneira didática.

A transferencia de dados, geralmente, é usando o protocolo HTTP.

O Rest, delimita algumas obrigações nessas transferência de dados.

Dados -> Resources seria então, uma entidade, um objeto.

### 6 Necessidades (constraints) para ser RESTFUL

- _Client-server_: Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema, usando o React para WEB e React Native para o smartphone, por exemplo.

- _Stateless_: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST). Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior. Nos nossos cursos, temos por padrão usar o tokens para as comunicações. Os tokens vão dizer se o usuário está autenticado ou não; desde que a API ou o caminho esteja fechado; se for aberto.

- _Cacheable_: As respostas para uma requisição, deverão ser explicitas ao dizer se aquela requisição, pode ou não ser cacheada pelo cliente.
 
- _Layered System_: O cliente acessa a um endpoint, sem precisar saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondida.

- _Code on demand (optional)_: Dá a possibilidade da nossa aplicação pegar códigos, como o JS, por exemplo, executar no cliente.

## RESTFUL 

RESTFUL, é cumprir os padões REST. É a aplicação dos padrões REST.

## Verbos HTTP

- GET -> Recebe dados de um resource
- POST -> Envia dados ou informações para serem processados por um resource
- PUT -> Atualiza os dados de um resource
-  DELETE -> Deleta um resource

=> RESOURCE => CLIENTE. É OS BLOQUINHOS DE NOTA.

## Boas praticas

- Utilizar verbos HTTP para as requisições
- Não utilizar barras no final do endpoint
- Utilizar plural ou singular na criação dos endpoints? _NÃO IMPORTA!_ use um padrão!!
- Nunca deixar o cliente sem resposta

## JSON(Fake users)

- http://jsonplaceholder.typicode.com/users

### STATUS DAS RESPOSTAS

- 1xx: Informação;
- 2xx: Sucesso;
  - 200: OK;
  - 201: Created;
  - 204: Não tem conteúdo PUT, POST, DELETE
- 3xx: Redirection
- 4xx: Client Error
  - 400: Bad request
  - 404: Not Found
- 5xx: Server Error
  - 500: Internal Server Error  