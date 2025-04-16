## 📌 O que é um Container?  

Um container é um **recurso de virtualização que contém um aplicativo ou um serviço**. Ele é executado em um ambiente isolado, como um processo ou um thread, e é gerenciado pelo sistema operacional.

### 🚀 Benefícios dos Containers:

☑️ Isolamento de aplicações  
☑️ Portabilidade entre diferentes ambientes  
☑️ Fácil integração em pipelines de CI/CD  
☑️ Segurança e controle de acesso  

---

## 🐳 Docker

O **Docker** é uma plataforma que permite criar, gerenciar e executar aplicações em containers. 

### 📌 Principais Conceitos:

🔹 **Imagem**: Um pacote de software contendo todos os arquivos e dependências para um aplicativo ou serviço.  
🔹 **Container**: Uma instância de uma imagem, executada em um ambiente isolado.  
🔹 **Docker Hub**: Repositório público de imagens Docker.  
🔹 **Docker Compose**: Ferramenta para gerenciar múltiplos containers.  
🔹 **Redes**: Mecanismo para comunicação entre containers.  

---

## 🛠️ Primeiros Passos com Docker

1️⃣ **Instale o Docker** em seu computador.  
2️⃣ **Teste o Docker** executando o comando:

```sh
$ docker run hello-world
```

3️⃣ **Listar containers:**

🔹 Containers em execução:  
```sh
$ docker ps
```
🔹 Todos os containers:  
```sh
$ docker ps -a
```

4️⃣ **Baixar uma imagem do Docker Hub:**

```sh
$ docker pull nginx
```

5️⃣ **Criar e executar um container do Nginx:**

```sh
$ docker run --name nginx-container -d -p 80:80 nginx
```
🔗 O Nginx estará disponível em: [http://localhost:8080](http://localhost:8080)

6️⃣ **Parar e remover um container:**

```sh
$ docker stop nginx-container
$ docker rm nginx-container
```

---

## ⚡ Comandos Úteis do Docker

| Comando | Descrição |
|---------|-----------|
| `docker --version` | Exibe a versão do Docker instalada |
| `docker pull <imagem>` | Baixa uma imagem do Docker Hub |
| `docker run <imagem>` | Inicia um container a partir de uma imagem |
| `docker ps` | Lista os containers em execução |
| `docker ps -a` | Lista todos os containers |
| `docker stop <container>` | Para um container em execução |
| `docker rm <container>` | Remove um container |
| `docker rmi <imagem>` | Remove uma imagem |
| `docker images` | Lista todas as imagens disponíveis |
| `docker build -t <imagem> .` | Cria uma imagem a partir de um Dockerfile |

---

## 📚 Referências

📌 **Começando com Docker** - [Alura](https://www.alura.com.br/artigos/comecando-com-docker)  
📌 **Curso Docker Completo** - [YouTube](https://www.youtube.com/watch?v=3c-iBn73dDE)  
📌 **Documentação Oficial do Docker** - [Docker Docs](https://docs.docker.com/engine/reference/commandline/cli/)  
📌 **O mínimo que você precisa saber sobre Docker** - [YouTube](https://www.youtube.com/watch?v=ntbpIfS44Gw)  
📌 **O que é Docker?** - [Twitter](https://x.com/programador_who/status/1875609788303716471)  
📌 **Tutorial Docker para Iniciantes** - [YouTube](https://www.youtube.com/watch?v=DdoncfOdru8)  

---