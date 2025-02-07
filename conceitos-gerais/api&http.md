# Conceitos de API e HTTP

## O que é uma API?

> Uma **API (Interface de Programação de Aplicações)** é um conjunto de regras e definições que permite que diferentes softwares se comuniquem entre si. Ela define como as requisições e respostas devem ser feitas, possibilitando que aplicações compartilhem dados e funcionalidades.

As APIs podem ser **RESTful** (baseadas em HTTP) ou seguir outros protocolos como **SOAP**, mas **APIs REST** são as mais comuns atualmente, especialmente para aplicações web.

### Principais Componentes de uma API

- **EndPoint**: URL através da qual a API é acessada.
- **Métodos HTTP**: Regras de como as requisições são feitas (GET, POST, PUT, DELETE, etc.).
- **Headers**: Informações adicionais na requisição, como tipo de conteúdo ou autenticação.
- **Body**: Parte da requisição onde dados podem ser enviados (geralmente em POST ou PUT).

## O que é HTTP?

O **HTTP (HyperText Transfer Protocol)** é o protocolo utilizado para a comunicação entre clientes (como navegadores ou aplicativos) e servidores web. Ele define como as mensagens são enviadas e recebidas pela web.

### Principais métodos HTTP

- **GET**: Recupera dados do servidor (sem modificar nada).
- **POST**: Envia dados ao servidor (usado para criação de recursos).
- **PUT**: Atualiza dados no servidor.
- **DELETE**: Remove um recurso do servidor.
- **PATCH**: Atualiza parcialmente um recurso.

### Exemplo de fluxo HTTP

1. **Cliente envia uma requisição GET**:
   O cliente, como um navegador ou aplicativo, envia uma requisição para um servidor, pedindo um recurso específico.

2. **Servidor processa a requisição**:
   O servidor recebe a requisição e processa a lógica necessária, como acessar um banco de dados ou outro serviço.

3. **Resposta do servidor**:
   O servidor então envia uma resposta com os dados solicitados ou uma mensagem de erro.

## Diferença entre API e HTTP

- **API**: Define um conjunto de regras e funções para a interação entre diferentes softwares.
- **HTTP**: Protocolo de comunicação usado para enviar e receber dados entre clientes e servidores. Muitas **APIs REST** utilizam HTTP como meio de comunicação.

## Principais Conceitos de HTTP/REST

URI (Uniform Resource Identifier): Endereço **único de um recurso na web**.
Métodos HTTP: Como as requisições são feitas (GET, POST, PUT, DELETE).
Status Codes: Códigos que indicam o sucesso ou falha da requisição.

- 200 OK: Requisição bem-sucedida.
- 404 Not Found: Recurso não encontrado.
- 500 Internal Server Error: Erro no servidor.

### Boas Práticas em APIs

- Usar métodos HTTP corretamente: Use GET para leitura, POST para criação, PUT para atualização e DELETE para remoção.
- Consumir APIs de forma segura: Verifique a autenticação e autorização antes de acessar uma API.
- Evitar dependências circulares: Evite depender de outras APIs que você está criando.
- **Documentação clara**: Sempre documente a API, explicando como ela pode ser utilizada, os parâmetros necessários e os tipos de resposta.
- Versionamento: Utilize versionamento na URL para garantir que alterações não quebrem funcionalidades existentes.

## Portas padrão de HTTP

- 80: HTTP (HTTP) e estamos usando o protocolo padrão do HTTP. Geralmente, os servidores HTTP usam a porta 80 para aceitar requisições de clientes.
- 443: HTTPS (HTTPS) é um protocolo de comunicação seguro que é usado para criptografar a comunicação entre o cliente e o servidor.
- De 1023 a 49151: Livres para uso pelos desenvolvedores.
- Portas entre 0 e 1023 são reservadas para serviços padronizados.

## Identificando o protocolo, recurso na URL e método da requisição

- <http://example.com/api/v1/users>

### Protocolo

- http://: Protocolo HTTP
- https://: Protocolo HTTPS

### Recurso (Endpoint)

- /api/v1/users: Recurso que será acessado
- /api/v1/users/:id: Recurso que será acessado e que requer um parâmetro
- /api/v1/users/search: Recurso que será acessado e que requer parâmetros (GET)
- /api/v1/users/create: Recurso que será acessado e que requer parâmetros (POST)
- /api/v1/users/update: Recurso que será acessado e que requer parâmetros (PUT)
- /api/v1/users/delete: Recurso que será acessado e que requer parâmetros (DELETE)
- /api/v1/users/search/:id: Recurso que será acessado e que requer parâmetros (GET)

# Domínios de Serviço

## O que é um domínio de serviço?

- Os servidores DNS transformam requisições de nomes em endereços IP, isso para que a pessoa usuária consiga acessar a página web esperada quando digitar o nome de domínio no navegador web.
- Um domínio de serviço é um nome de domínio que é registrado no DNS (Domain Name System) e que pode ser utilizado para acessar um serviço.
- Um domínio de serviço é uma parte do endereço de um serviço, que é utilizado para acessar o serviço.
- Um domínio de serviço é um nome de domínio que é registrado no DNS (Domain Name System) e que pode ser utilizado para acessar um serviço.

### Sistema de nomes de domínios (DNS)

- O DNS é o sistema responsável por traduzir nomes de domínios para endereços IP.

Por exemplo, se você quiser acessar o site da Google, você digitará o nome de domínio "google.com" no navegador web. **O DNS irá traduzir o nome de domínio para o endereço IP do site da Google.**

## Dominios locais e domínios públicos

#### O domínio é o nome do site na Web. Ele facilita a navegação do usuário, que não precisa lembrar o IP de cada site

- Um domínio local é um nome de domínio que é registrado no DNS local, enquanto que um domínio público é um nome de domínio que é registrado no DNS público.
 Por exemplo, o público seria o nome de domínio "google.com" e o local seria o nome de domínio "localhost".

### Dns é hierarquico

- O DNS é um sistema hierarquico, ou seja, ele é composto por vários nós que estão conectados entre si.
Para simplificar, o DNS é composto por três nós principais:
- O nó de root, que é o **nó raiz** do DNS.
- O nó de domínio, que é onde os **registros de nomes de domínio são armazenados**.
- O nó de host, que é responsável por armazenar as informações de **endereços IP**.

Primeiro é o raiz; (top-level domain, TLD).
Segundo é o domínio; (com, br, org, net, pt, etc.)
Terceiro é o host.

**http:** Protocolo
**//localhost:** Endereço IP ou Nome de domínio.
:3000/: caminho (raiz)

# Formas de lembrar o servidor da sessão

- Cookies
- Tokens
- URLs

## Cookies

[Cookies](https://www.alura.com.br/artigos/o-que-sao-cookies-como-funcionam) são **pequenos arquivos que são enviados pelo navegador do usuário para o servidor**. Geralmente são gravados no disco rígido do usuário, mas também podem ser gravados em memória do navegador.

## Tokens

**
[Tokens](https://www.seudinheiro.com/conteudo-de-marca/o-que-e-token-como-funciona-vantagens-e-desvantagens/) Um token é **uma unidade de dados que representa a autorização de acesso a um recurso ou serviço**. No contexto de segurança de software, os tokens são utilizados para autenticar usuários e garantir que apenas aqueles com as permissões adequadas possam acessar informações sensíveis. Eles podem assumir diversas formas, como tokens de sessão, tokens de acesso e tokens de atualização, cada um com sua função específica dentro do ecossistema de segurança.

## URLs

[URLs](https://developer.mozilla.org/pt-BR/docs/Glossary/URL) **Uniform Resource Locator (URL)** é uma sequência de texto que especifica onde um recurso pode ser encontrado na Internet.

No contexto de HTTP, URLs são chamadas de "Endereços web" ou "link". Seu navegador exibe as URLs na barra de endereços.

# O que é CRUD ?

- Abreviação de CRUD (Create, Read, Update, Delete)
- CRUD é um conjunto de operações que podem ser realizadas em um sistema de banco de dados.
- CRUD é uma maneira de se organizar as operações de um sistema de banco de dados.

## CRUD

- **Create**: Criar um novo registro.
- **Read**: Ler os dados de um registro.
- **Update**: Atualizar os dados de um registro.
- **Delete**: Excluir um registro.

## CRUD vs REST

- **CRUD**: CRUD é um conjunto de operações que podem ser realizadas em um sistema de banco de dados.
- **REST**: REST é uma maneira de se organizar as operações de um sistema de banco de dados.

### O que são APIs?

**APIs** são interfaces entre aplicações. **Podemos pensar em APIs como pontos de contato ou comunicação entre partes de um sistema ou entre sistemas diferentes**, por exemplo:

- O back-end de uma aplicação disponibiliza uma API para que o front-end possa buscar dados para popular uma página (no caso da API da Alura).
- Uma aplicação quer utilizar um sistema de busca de CEPs disponibilizado por terceiros. O serviço de busca disponibiliza uma API para ser usada pela aplicação (um exemplo famoso é o [ViaCEP](https://viacep.com.br/)).
- Grande parte dos serviços em nuvem, como a AWS e o Google Cloud, disponibilizam APIs para que clientes possam utilizar seus serviços.

### APIs e JSON
>
> **API**, ou _application programming interface_ (interface de programação de aplicações), em tradução livre
O formato JSON é o padrão atual para envio de recebimento de dados entre aplicações. Na prática, isso significa que usamos JSON para, por exemplo:

- Um front-end pegar dados de um formulário em uma página e enviar para o back-end criar um cadastro de cliente, como em `{“nome”: “José”, “email”: “jose@email.com”, “telefone”: “551199999999”}`;
- Um back-end consultar dados armazenados em tabelas de um banco de dados e formatá-los em JSON para enviá-los ao front (como a API da Alura).

E como é feito esse envio e recebimento de JSON?

### JSON e requisições

Quando queremos “transitar” um objeto JSON entre computadores na web através do [protocolo HTTP](https://www.alura.com.br/artigos/desmistificando-o-protocolo-http-parte-1) é necessário transformar toda a estrutura em strings, pois nessa comunicação trafegam apenas dados em texto.

Por esse motivo, é bastante comum a operação de transformar um JSON em string e também reconverter um texto em JSON para que o objeto possa ser utilizado pelo programa.

Você vai ter oportunidade de praticar mais com APIs e com o envio e recebimento de JSON nas próximas formações e cursos de Node.js.

# Referências 🔗

📌 **Diferenças entre GET e POST** - [Alura](https://www.alura.com.br/artigos/diferencas-entre-get-e-post)  
📌 **HTTP: um guia completo sobre o que é e como funciona o protocolo da web** - [Alura](https://www.alura.com.br/artigos/http)  
📌 **O que é uma API e como ela funciona? APIs para iniciantes** - [freeCodeCamp](https://www.freecodecamp.org/portuguese/news/o-que-e-uma-api-e-como-ela-funciona-apis-para-iniciantes/)  
📌 **O que são GET, POST, PUT, PATCH e DELETE? Um walkthrough com JavaScript’s Fetch API** - [Medium](https://medium.com/@9cv9official/what-are-get-post-put-patch-delete-a-walkthrough-with-javascripts-fetch-api-17be31755d28)  
📌 **O que são APIs?** - [Alura](https://www.alura.com.br/artigos/api)  
