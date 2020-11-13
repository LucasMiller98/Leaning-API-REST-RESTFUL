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
 
- _Layered System_: 








## RESTFUL 

RESTFUL, é cumprir os padões REST. É a aplicação dos padrões REST.