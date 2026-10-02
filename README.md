# SmartList

Sistema de gerenciamento de lista de compras desenvolvido em **Java**, como projeto acadêmico da disciplina de Programação Orientada a Objetos.

O projeto tem como objetivo aplicar conceitos de **Programação Orientada a Objetos**, manipulação de arquivos, serialização de objetos, coleções, API Streams e padrões de projeto, utilizando uma aplicação executada via linha de comando.

> Projeto baseado na proposta acadêmica do repositório [SmartList 2026](https://github.com/FranBeal/smartlist-2026).

---

## 📋 Sobre o Projeto

O **SmartList** é um sistema para gerenciamento de listas de compras. A aplicação permite cadastrar, remover e visualizar produtos, além de salvar e carregar os dados utilizando diferentes formatos de armazenamento.

Durante o desenvolvimento, são aplicados conceitos importantes da linguagem Java e da Programação Orientada a Objetos, buscando também manter uma estrutura organizada e separação de responsabilidades entre as diferentes partes da aplicação.

---

## 🎯 Objetivos

O projeto tem como principais objetivos colocar em prática:

* Programação Orientada a Objetos (POO);
* Encapsulamento;
* Abstração;
* Coleções do Java;
* `List`, `Set` e `Map`;
* API Streams;
* Manipulação de arquivos;
* Serialização e desserialização de objetos;
* Manipulação de arquivos JSON;
* Arquivos de texto;
* Arquivos binários;
* Arquitetura MVC;
* Padrão Singleton;
* Padrão Strategy;
* Padrão Command;
* Organização e separação de responsabilidades;
* Boas práticas de desenvolvimento em Java.

---

## ⚙️ Funcionalidades

O SmartList possui funcionalidades para gerenciamento dos produtos da lista de compras.

### Gerenciamento de produtos

* Adicionar produtos;
* Remover produtos;
* Exibir a lista de compras;
* Organizar produtos em ordem alfabética.

### Manipulação de arquivos

A aplicação permite trabalhar com diferentes formatos de armazenamento:

* Salvar lista em arquivo `.txt`;
* Carregar lista a partir de arquivo `.txt`;
* Salvar lista em arquivo binário `.bin`;
* Carregar lista a partir de arquivo binário;
* Salvar lista em arquivo `.json`;
* Carregar lista a partir de arquivo JSON.

### Operações sobre os produtos

* Filtrar produtos por quantidade mínima;
* Calcular o valor total da lista;
* Utilizar Streams para operações sobre coleções.

---

## 🏗️ Arquitetura

O projeto utiliza uma estrutura baseada no padrão arquitetural **MVC (Model-View-Controller)**.

```text
              ┌───────────────┐
              │     View      │
              │               │
              │ Interface CLI │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │  Controller   │
              │               │
              │ Regras de     │
              │ interação     │
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │     Model     │
              │               │
              │ Produtos e    │
              │ lista de      │
              │ compras       │
              └───────────────┘
```

### Model

Responsável pelos dados e pelas regras relacionadas ao domínio da aplicação.

Exemplos:

* `Produto`
* `ListaDeCompras`

### View

Responsável pela interação com o usuário e pela apresentação das informações.

A aplicação utiliza uma interface baseada em **linha de comando (CLI)**.

### Controller

Responsável por receber as ações do usuário, coordenar as operações e realizar a comunicação entre a View e o Model.

---

## 🧩 Padrões de Projeto

O projeto trabalha com diferentes padrões de projeto:

### Singleton

Utilizado para garantir uma única instância de determinados componentes que precisam ser compartilhados pela aplicação.

### Strategy

Permite encapsular diferentes estratégias de execução, possibilitando alterar o comportamento utilizado sem modificar diretamente o código que o utiliza.

### Command

Encapsula operações como comandos independentes, facilitando a organização das ações disponíveis na aplicação.

### MVC

Utilizado para separar:

* Dados e regras de negócio;
* Interface com o usuário;
* Controle do fluxo da aplicação.

---

## 💾 Persistência de Dados

O SmartList trabalha com diferentes formas de persistência.

### Arquivo de texto

Utilizado para armazenar os dados em formato textual, permitindo que as informações sejam facilmente visualizadas.

```text
lista_compras.txt
```

### Arquivo binário

Utilizado para realizar a persistência dos objetos em formato binário.

```text
lista_compras.bin
```

### JSON

Utilizado para representar os dados de maneira estruturada.

```text
lista_compras.json
```

---

## 🛠️ Tecnologias

| Tecnologia    | Utilização                       |
| ------------- | -------------------------------- |
| Java          | Linguagem principal              |
| JDK 21+       | Ambiente de execução             |
| Maven         | Gerenciamento e build do projeto |
| JSON          | Persistência estruturada         |
| Java Streams  | Manipulação de coleções          |
| IntelliJ IDEA | IDE recomendada                  |

---

## 📦 Pré-requisitos

Antes de executar o projeto, certifique-se de possuir:

* **JDK 21 ou superior**
* **Maven**
* **IntelliJ IDEA** ou outra IDE compatível com projetos Maven
* **Git**, caso queira clonar o projeto

Para verificar a instalação do Java:

```bash
java -version
```

Para verificar o Maven:

```bash
mvn -version
```

---

## 🚀 Como executar

### 1. Clone o repositório

```bash
git clone <URL_DO_SEU_REPOSITORIO>
```

### 2. Acesse a pasta do projeto

```bash
cd Vendas_POO
```

### 3. Compile o projeto

```bash
mvn clean package
```

### 4. Execute a aplicação

A execução pode ser realizada diretamente pela IDE ou através da classe principal configurada no projeto.

---

## 📁 Estrutura do Projeto

A estrutura segue a organização proposta pela arquitetura MVC:

```text
src/
└── main/
    └── java/
        └── br/
            └── com/
                ├── model/
                ├── view/
                └── controller/
```

Além do código-fonte, o projeto pode conter os arquivos utilizados para persistência dos dados:

```text
lista_compras.txt
lista_compras.bin
lista_compras.json
```

---

## 📚 Conceitos Aplicados

Este projeto foi desenvolvido com foco no aprendizado e aplicação prática dos seguintes conceitos:

* Classes e objetos;
* Encapsulamento;
* Construtores;
* Métodos e atributos;
* Interfaces;
* Herança e polimorfismo;
* Coleções;
* Generics;
* Lambda Expressions;
* API Streams;
* Entrada e saída de dados;
* Tratamento de exceções;
* Serialização;
* Desserialização;
* JSON;
* Arquitetura MVC;
* Padrões de projeto.

---

## 👨‍💻 Desenvolvimento

Projeto desenvolvido como atividade acadêmica, tendo como referência a proposta **SmartList 2026** disponibilizada pela disciplina.

Repositório da proposta original:

https://github.com/FranBeal/smartlist-2026

---

## 📄 Licença

Este projeto foi desenvolvido para fins **acadêmicos e educacionais**.
