# Microservices for Email Sending with RabbitMQ (Spring Boot)

Este projeto é composto por dois microserviços criados para estudar **Spring Boot**, **RabbitMQ** e **comunicação entre microserviços**. Projeto utilizado para estudar a integração com RabbitMQ.

## 🚀 Objetivo do Projeto
Demonstrar como dois microserviços podem se comunicar de forma assíncrona utilizando o **RabbitMQ** para enviar e-mails. O projeto simula um fluxo em que:
1. O **serviço User** cria um usuário.
2. O **serviço Email** recebe uma mensagem para enviar um e-mail de boas-vindas.

## 🛠️ Estrutura do Projeto

microservice_envio_email_springboot_rabbit/ 
										├── email/ <- Código do microserviço de e-mails 
												│ ├── src/ │ ├── pom.xml │ └── ... 
										├── user/ <- Código do microserviço de usuários 
												│ ├── src/ │ ├── pom.xml │ └── ... 
										└── README.md <- Documentação do projeto
									


### Microserviços:
- **User**: Responsável por criar usuários e enviar mensagens para o RabbitMQ.
- **Email**: Consome mensagens do RabbitMQ e realiza o envio de e-mails.

## 🧰 Tecnologias Utilizadas
- Java 21
- Spring Boot
- RabbitMQ
- Maven

## 🔧 Como Rodar o Projeto
1. Certifique-se de ter o **RabbitMQ** instalado e em execução.
   - [Guia de instalação do RabbitMQ](https://www.rabbitmq.com/download.html)
2. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/microservice_envio_email_springboot_rabbit.git
3. Abra duas instâncias da sua IDE (por exemplo, IntelliJ):

	Abra a pasta user em uma instância da IDE.
	Abra a pasta email em outra instância da IDE.
	Execute cada microserviço individualmente:

	No microserviço user, execute:
	mvn spring-boot:run

	No microserviço email, execute:
	mvn spring-boot:run

5.	Os dois microserviços devem estar em execução para que a comunicação via RabbitMQ funcione corretamente.

6.	Acesse os endpoints expostos pelos microserviços para testar a aplicação.

7.	Creditos ao canal Michelli Brito (https://www.youtube.com/watch?v=ZnECi2gatMs)

