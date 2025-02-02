# O que é um container?

Um container é um **recurso de virtualização que contém um aplicativo ou um serviço**. Ele é executado em um ambiente isolado, como um processo ou um thread, e é gerenciado pelo sistema operacional.

Os containers são usados para:

- Implementar ambientes isolados e seguros para aplicativos e serviços.
- Permitir a portabilidade de aplicativos e serviços.
- Permitir a reutilização de recursos computacionais.
- Facilitar a manutenção e a atualização de aplicativos e serviços.

# Tipos de containers

Existem vários tipos de containers disponíveis, cada um com suas características e usos específicos.

## Docker

O Docker é um a plataforma que **permite criar, gerenciar e executar aplicações em containers**. Containers são como máquinas virtuais leves que compartilham o kernel do sistema operacional, permitindo que você execute aplicativos e serviços em um ambiente isolado e seguro.

### Principais conceitos

- **Imagem**: Uma imagem é um pacote de software que contém todos os arquivos e dependências necessários para executar um aplicativo ou um serviço.
- **Container**: Um container é uma instância de uma imagem. Ele é executado em um ambiente isolado e separado do sistema operacional.
- **Docker Hub**: O Docker Hub é um repositório público de imagens Docker. Ele permite que você busque, baixe e use imagens de aplicativos e serviços.
- **Docker Compose**: O Docker Compose é uma ferramenta para gerenciar containers Docker. Ele permite que você defina e configure aplicativos e serviços em containers de forma fácil e rápida.
- **Redes**: Mecanismo para comunicação entre containers.

### Por que usar o Docker?

- Isolamento de aplicações;
- Portabilidade entre diferentes ambientes;
- Fácil integração em pipeline de CI/CD;
- Segurança e controle de acesso.

#### Primeiros Passos com Docker

1. Instale o Docker em seu computador.
2. **Testar o Docker**: Eexecute o comando
`docker run hello-world` no terminal.

- Esse comando baixa a imagem `hello-world` do Docker Hub e executa o aplicativo dentro do container.
- Cria e executa um container a partir dela;
- Exibe uma mensagem de boas-vindas.

2 - Listar containers:

- Para ver os containers em execução, execute o comando `docker ps`.

- Para ver todos os containers, execute o comando `docker ps -a`.

3 Baixe uma imagem do Docker Hub:

- Baixe uma imagem do Nginx:
`docker pull nginx`

4 - Criar e executar um container do Nginx:

- Inicie um container do Nginx:
`docker run --name nginx-container -d -p 80:80 nginx`
- O Nginx estará disponível em <http://localhost.8080>

5 - Parar e remover um container:

- Pare o container:
`docker stop nginx-container`

- Remove o container:
`docker rm nginx-container`

## Comandos Úteis do Docker

Comando / Descrição
`Docker --version`: Exibe a versão do Docker instalada.
`docker pull <imagem>`: Baixa uma imagem do Docker Hub.
`docker run <imagem>`: Inicia um container a partir de uma imagem.
`docker ps`: Lista os containers em execução.
`docker ps -a`: Lista todos os containers.
`docker stop <container>`: Para o container em execução.
`docker rm <container>`: Remove o container.
`docker rmi <imagem>`: Remove uma imagem.
`docker images`: Lista todas as imagens disponíveis.
`docker build -t <imagem> .`: Cria uma imagem a partir de um arquivo Dockerfile.

# Referências

- [O que é docker](https://x.com/programador_who/status/1875609788303716471)
