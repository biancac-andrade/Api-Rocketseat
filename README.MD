#API, REST E RESTFUL    -- rocketseat o que é API? Rest e Restful? Mayk Brito


Cliente(Client)
Garçon (pedidos, levar seus pedidos, para cozinha) (API)
Cozinha (Server)

#API 

Restaurante
Limpinho, 
que te atende bem,
te dê aquilo que vc pediu


Cliente
Gritando, 
xingando

Acronico de Application Programming Interface(Interface de Programação de Aplicações)
é basicamente um conjunto de rotinas e padrões estabelecidas por uma aplicação, para que 
outras aplicações possam utilizar as funcionalidades desta aplicação.

- responsavel por estabelecer comunicação entre diferentes serviços
- meio de campo entre as tecnologias
- intermediador para troca de informações

##REST
um acronico para Representational State Transfer (Transferencia de Estado Representativo)
Sera feita a transferencia de dados de uma maneira simbolica, figurativa, representativa, de maneira didática

A transferencia de dados, geralmente, usando o protocolo HTTP

o Rest, delimita algumas  obrigações nessa transferencia de dados.

Resources seria então, uma entidade, um objeto.

### 6 necessidades (constraints) para ser RESTful.

- _Client-Server_: Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade de nosso sistema, usando React para web e React Native para o smartphone, por exemplo.
  
- _Stateless_: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSe) a requisição (REQUEST). Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior. Nos nossos cursos, temos por padrão usar tokens para as comunicações
  
- _Cacheable_: As respostas para uma requisição, deverão ser explicitas ao dizer se aquela resquição, pode ou não ser cacheada pelo cliente.
  
- _Layered System_:  O lciente acessa a um endpoint, sem precisasr saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondido.
- ex https://graph.facebook.com/youtube = explicação o youtube seria uma endpoint, o granph.facebook é uma api, ok, então o url é adicionado como um informação que vc quer,que é informação do youtube
  
- _Code on demand (optional)_: Dá possibilidade da nossa aplicação pegar códigos, como javascript, por exemplo, para executar no cliente;

## RESTful
RESTful, é a aplicação dos padrões REST

## BOAS PRATICAS
- utilizar verbos HTTP para nossas requisições
- utilizar plurarl ou singular na criação dos endpoints? _Não Importa!_ use padrão!!
- Não deixar barra no final do endpoint
- Nunca deixe o cliente sem resposta

## verbos HTTP
//GET: receber dados de um resource.
//POST enviar dados ou informações para ser processados por ser um resource
//PUT atualizar dados de um resource
//DELETE deleter um resource

## STATUS DAS RESPOSTAS

- 1xx: Informação
- 2xx: Sucesso
  - 200: OK
  - 201: created
  - 204: nao tem conteudo PUT POST DELETE
-3xx: Redirection
-4xx: Client Error
    - 400: Bad Request
    - 404: Not Found!
- 5xx: Server Error
  - 500: Internal Server Error
  - 


## LEMBRETE
 
Instalação do yarn npm install --global yarn
executa  yarn init -y e ele criar um packeage.json
instalar servidor   yarn add express e adiciona pasta node_modules

dentro da pasta data.json é resources de clientes, porém é clientes fake, então foi copiado e colado nesse url: https://jsonplaceholder.typicode.com/users