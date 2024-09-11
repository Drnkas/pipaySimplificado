# PicPay Simplificado - Desafio Backend

## 💡 Sobre o Projeto

Este projeto foi desenvolvido como parte de um desafio para uma vaga de desenvolvedor backend na PicPay. O **PicPay Simplificado** é uma plataforma de pagamentos que permite o depósito e a realização de transferências de dinheiro entre usuários e lojistas. O sistema foi implementado para seguir as diretrizes e requisitos fornecidos, e simula operações de pagamento e notificações.

## 🚀 Funcionalidades

- **Transferências**: Usuários podem enviar dinheiro para outros usuários e lojistas. Lojistas apenas recebem transferências.
- **Validação de Saldo**: Verificação do saldo do usuário antes da transferência.
- **Consultas Externas**: Simulação de consultas a serviços autorizadores externos para validar transferências.
- **Notificações**: Envio de notificações via e-mail ou SMS após a transferência utilizando um serviço de terceiros.
- **Transações**: Garantia de consistência com rollback em caso de falhas durante as transferências.

- Consultas externas:
  - **Autorizador**: [Mock de Autorizador](https://util.devi.tools/api/v2/authorize) (GET)
  - **Notificações**: [Mock de Notificações](https://util.devi.tools/api/v1/notify) (POST)

## 🛠️ Tecnologias Utilizadas

- [Java](https://www.oracle.com/java/) (Linguagem de programação)
- [Spring Boot](https://spring.io/projects/spring-boot) (Framework para construção de aplicações Java)
- [Maven](https://maven.apache.org/) (Gerenciamento de dependências e construção)
- [H2 Database](https://www.h2database.com/) (Banco de dados em memória para desenvolvimento)

## 🛠️ Como Rodar o Projeto

Para rodar o projeto localmente, siga os seguintes passos:

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/picpay-simplificado.git
2. Acesse a pasta do projeto:
   ```bash
    cd picpay-simplificado
3. Compile o projeto e execute o aplicativo:
   ```bash
   mvn clean install
   mvn spring-boot:run
4. O aplicativo estará disponível em http://localhost:8080.
