# Desafio Backend BTG Pactual

Este é um projeto de desafio backend do BTG Pactual. Neste projeto, aprenderemos e implementaremos os seguintes conceitos e tecnologias:

## Objetivos

- Como criar uma API com Spring Boot
- Como criar um microserviço com Spring Boot
- Como configurar o RabbitMQ e MongoDB via Docker
- Como consumir uma fila do RabbitMQ
- Como comunicar com o banco de dados MongoDB via Docker
- Como mapear uma collection do MongoDB dentro do Spring
- Como fazer aggregations no MongoDB com Spring
- Como efetuar logs com o SLF4J

## Tecnologias Utilizadas

- Java
- Spring Boot
- RabbitMQ
- MongoDB
- Docker
- SLF4J

## Estrutura do Projeto

### 1. Criando a API com Spring Boot
Neste projeto, utilizamos o Spring Boot para criar uma API RESTful. A estrutura básica do projeto foi configurada com as dependências necessárias para o desenvolvimento de microserviços.

### 2. Configurando o RabbitMQ e MongoDB via Docker
Para a configuração do RabbitMQ e MongoDB, utilizamos o Docker. Isso facilita a criação de ambientes de desenvolvimento consistentes e portáteis.

- Arquivo `docker-compose.yml` para configurar e iniciar RabbitMQ e MongoDB:
```yaml
version: '3.8'
services:
  rabbitmq:
    image: rabbitmq:3-management
    ports:
      - 5672:5672
      - 15672:15672
  mongodb:
    image: mongo:4.4.3
    ports:
      - 27017:27017
```
###
## 3. Consumindo Fila do RabbitMQ
Utilizamos o Spring AMQP para consumir mensagens de uma fila do RabbitMQ. As mensagens são processadas e os dados são salvos no MongoDB.

## 4. Comunicando com MongoDB via Docker
O Spring Data MongoDB é utilizado para mapear collections do MongoDB em entidades Java e realizar operações CRUD.

## 5. Fazendo Aggregations no MongoDB com Spring
Utilizamos o Spring Data MongoDB Aggregation Framework para realizar consultas complexas e agregações no MongoDB.

## 6. Efetuando Logs com o SLF4J
A biblioteca SLF4J é utilizada para logging. Isso nos permite registrar informações importantes e facilitar a depuração do aplicativo.

### Instruções para Executar o Projeto
Pré-requisitos
- Docker e Docker Compose instalados
- JDK 11 ou superior instalado
- Maven instalado
- Passos para executar
  
## Clone o repositório:
``` bash
Copiar código
git clone https://github.com/Bellacmeireles/Desafio_BackEnd_BTG_Pactual.git
cd Desafio_BackEnd_BTG_Pactual
Inicie os containers do RabbitMQ e MongoDB:
```

bash
Copiar código
```
docker-compose up
Compile e execute o projeto Spring Boot:
```
bash
Copiar código
```
mvn clean install
mvn spring-boot:run
```

### Referências
Este desafio foi realizado com base em um vídeo tutorial no YouTube. Você pode assistir ao vídeo através do link abaixo:

[Desafio Backend BTG Pactual - Vídeo Tutorial](https://youtu.be/e_WgAB0Th_I?si=zOuRHs4MOf3XRbvY)


Se você encontrar algum problema ou tiver alguma dúvida, sinta-se à vontade para abrir uma issue ou entrar em contato.

