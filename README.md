# 🚀 Petfolio API — Arquitetura em Camadas, Regras de Negócio e CRUD Completo com .NET

---

## 🧭 Visão Geral

O **Petfolio API** é um projeto back-end desenvolvido com **.NET**, criado com o objetivo de ensinar, na prática, **organização de projetos profissionais**, **arquitetura em camadas**, **separação de responsabilidades** e a construção de um **CRUD completo** para gerenciamento de pets.

A aplicação evolui passo a passo, abordando conceitos fundamentais utilizados no mercado, desde a organização da solução até a implementação de regras de negócio e endpoints REST bem estruturados.

---

## ⚙️ Etapas do Desenvolvimento

### 🧱 1. Organização de Projetos e Arquitetura em Camadas
* Importância da separação do código em camadas
* Criação das camadas principais:
  - API (camada de entrada)
  - Application (lógica de negócio)
  - Data (acesso a dados)
* Benefícios dessa abordagem:
  - Reutilização de código
  - Facilidade de manutenção
  - Escalabilidade
  - Encapsulamento
  - Melhor colaboração em equipe

---

### 📦 2. Bibliotecas de Classes no .NET
* Conceito de biblioteca de classes
* Biblioteca como uma “caixa de ferramentas”
* Cada classe com um propósito específico
* Uso das bibliotecas por projetos executáveis
* Exemplos de aplicação:
  - Envio de e-mails
  - Conexão com banco de dados
  - Regras de negócio reutilizáveis

---

### 🐾 3. Criação da API Petfolio e Estrutura da Solução
* Criação da API **Petfolio**
* Divisão da solução em múltiplos projetos
* Definição clara das responsabilidades de cada projeto
* Gerenciamento de dependências entre as camadas

---

### 🌐 4. Criação do Primeiro Controller e Endpoint POST
* Criação de um controller na pasta **Controllers**
* Implementação do endpoint do tipo **POST**
* Testes do endpoint utilizando o **Swagger**
* Validação do funcionamento da API

---

### 🧠 5. Projeto Application e Regras de Negócio
* Responsabilidade do projeto **Petfolio.Application**
* Implementação das regras de negócio
* Exemplo prático: cadastro de um pet
* Possíveis ações dentro de um caso de uso:
  - Validações
  - Envio de e-mails
  - Persistência em banco de dados
  - Geração de documentos
* Aplicação do **Princípio da Responsabilidade Única (SOLID)**
* Organização das regras em **Use Cases**
* Criação de subpastas para cada regra de negócio

---

### 🧩 6. Organização com Sync Namespaces
* Uso da funcionalidade **Sync Namespaces** no Visual Studio
* Renomeação de pastas mantendo namespaces atualizados
* Benefícios:
  - Padronização
  - Organização
  - Facilidade de manutenção

---

### ✏️ 7. Atualização de Pets (PUT)
* Criação do endpoint **PUT**
* Recebimento do ID pela rota
* Recebimento das novas informações no corpo da requisição
* Reutilização da mesma classe de request para criação e atualização
* Retorno do status **204 No Content** em caso de sucesso

---

### ⚠️ 8. Tratamento de Erros e Validações
* Retorno de lista de mensagens de erro
* Padronização das respostas de erro
* Uso de sintaxe moderna do C#
* Atualização do Swagger com:
  - Status 400
  - Mensagens de erro descritivas

---

### 📄 9. Listagem de Pets (GET)
* Criação de endpoint **GET** para listagem
* Retorno apenas das informações necessárias:
  - ID
  - Nome
  - Tipo
* Boas práticas para endpoints de listagem
* Estrutura de resposta contendo uma propriedade com a lista de itens

---

### 🔎 10. Busca de Pet por ID (GET)
* Criação do endpoint **GET por ID**
* Retornos possíveis:
  - **200 OK** com dados completos
  - **404 Not Found** se o pet não existir
* Implementação da lógica no *use case*
* Lançamento e tratamento de exceção de *not found*

---

### ❌ 11. Exclusão de Pets (DELETE)
* Criação do endpoint **DELETE**
* Recebimento do ID pela rota
* Implementação da regra de negócio de exclusão
* Retornos possíveis:
  - **204 No Content**
  - **404 Not Found**
* Finalização do CRUD de pets

---

## 🧰 Tecnologias Utilizadas

* C#
* .NET
* Visual Studio
* Swagger / Swashbuckle
* Arquitetura REST
* Princípios SOLID

---

## 🧠 Conceitos Principais Dominados

* Arquitetura em camadas
* Separação de responsabilidades
* Bibliotecas de classes no .NET
* Princípios SOLID
* Organização de projetos profissionais
* Use Cases para regras de negócio
* CRUD completo
* Boas práticas em APIs REST
* Tratamento de erros e status HTTP
* Documentação com Swagger

---

## 🏁 Conclusão

O **Petfolio API** demonstra como construir uma API moderna e profissional com .NET, focando não apenas na funcionalidade, mas principalmente na **qualidade da arquitetura e organização do código**.

Este projeto fornece uma base sólida para desenvolvimento de aplicações escaláveis, bem estruturadas e alinhadas com padrões utilizados no mercado.
