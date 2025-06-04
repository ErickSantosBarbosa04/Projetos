
# 🧳 P&E VIAGENS — Sistema de Gerenciamento de Agência de Viagens

## 📌 Descrição do Projeto

**P&E Viagens** é um sistema web desenvolvido como projeto acadêmico para simular o gerenciamento de uma agência de viagens. O sistema permite o cadastro de clientes, consulta e reserva de pacotes turísticos, controle de viagens e geração de relatórios. O projeto foi desenvolvido aplicando boas práticas de engenharia de software, arquitetura em camadas e padrões de projeto do catálogo GoF.

## 📁 Estrutura do Projeto

```
viagens/
├── src/
│   ├── controller/
│   ├── model/
│   ├── dao/
│   └── util/
├── web/
│   ├── jsp/
│   ├── css/
│   └── imagens/
├── banco/
│   └── agencia_viagens.sql
├── README.md
└── .gitignore
```

## 🧰 Tecnologias Utilizadas

- **Linguagem:** Java (JDK 11+)
- **Front-end:** JSP + HTML + CSS
- **Back-end:** Servlets + Java
- **Banco de dados:** MySQL
- **IDE recomendada:** IntelliJ IDEA ou Eclipse
- **Padrões aplicados:** Builder, Command, Decorator, Factory, Facade, Liskov Substitution Principle

## ⚙️ Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/usuario/pe-viagens.git
```

### 2. Importe o projeto na IDE (IntelliJ ou Eclipse)

- **File > Open > selecione a pasta `viagens`**
- Verifique se o JDK está configurado corretamente

### 3. Configure o banco de dados MySQL

- Crie um banco de dados com o nome `agencia_viagens`
- Importe o arquivo `banco/agencia_viagens.sql` para criar as tabelas e dados iniciais

```sql
source caminho/para/agencia_viagens.sql;
```

### 4. Configure a conexão com o banco

No arquivo de propriedades ou classe utilitária de conexão (`ConnectionFactory.java`):

```java
String url = "jdbc:mysql://localhost:3306/agencia_viagens";
String usuario = "root";
String senha = "sua_senha";
```

### 5. Execute a aplicação

- Execute o servidor (ex: Tomcat)
- Acesse: [http://localhost:8080/viagens](http://localhost:8080/viagens)

## ✅ Funcionalidades Implementadas

- Cadastro e login de clientes
- Consulta e listagem de pacotes turísticos
- Realização e controle de reservas
- Visualização de viagens disponíveis
- Controle administrativo e geração de relatórios
- Interface clara com feedback para o usuário

## 📌 Padrões de Projeto Utilizados

- **Builder:** construção flexível de objetos `Viagem`
- **Command:** ações encapsuladas em botões de reserva/cancelamento
- **Decorator:** serviços extras adicionados ao pacote de viagem
- **Factory:** criação de instâncias de viagens padrão
- **Facade:** simplificação da lógica de reserva
- **LSP:** classes especializadas substituem corretamente as genéricas

## 📷 Prints do Sistema

Imagens do sistema em funcionamento estão disponíveis na pasta `/web/imagens` e também nos anexos do documento acadêmico.

## 👨‍🏫 Projeto Acadêmico

Este projeto foi desenvolvido para a disciplina de **Padrões de Projeto**, no curso de **Engenharia de Software** da **Universidade de Mogi das Cruzes** — 2025.

> Autores:
> - Erick Santos Barbosa — 11231101277  
> - Pedro Henrique Harada Pecegueiro — 1123110192

## 📄 Licença

Este projeto é apenas para fins acadêmicos e **não possui fins comerciais**. Licença de uso aberta conforme os termos educacionais.
