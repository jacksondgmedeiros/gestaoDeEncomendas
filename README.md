# 📦 Sistema de Gestão de Encomendas

## 📌 Visão Geral

Sistema para gerenciamento de encomendas em condomínios residenciais, com foco no controle de recebimento, organização, facilidade de localização pela portaria e retirada de pacotes pelos moradores.

O sistema permite registrar encomendas, associá-las a moradores e facilitar a identificação na portaria através de cores.

---

## 🎯 Objetivo do Projeto

Criar uma API REST para:

* Controlar encomendas recebidas na portaria
* Organizar moradores e apartamentos
* Facilitar a localização de encomendas
* Simular um cenário real de uso em condomínios

---

## 🏢 Estrutura do Condomínio

O condomínio é composto por:

* blocos
* andares por bloco
* apartamentos por andar
* moradores por apartamento

---

## 🧱 Modelagem de Dados (3FN)

### Entidades principais:

* Bloco
* Andar
* Apartamento
* Morador
* Encomenda
* Cor (identificação visual)

---

## 🔗 Relacionamentos

* Um bloco possui vários andares
* Um andar possui vários apartamentos
* Um apartamento possui vários moradores
* Um morador pode ter várias encomendas
* Uma encomenda possui uma cor de identificação

---

## 🎨 Identificação por Cor

Cada encomenda recebe uma cor no momento do cadastro de acordo com o seu dia na semana.

### Motivação:

* Facilitar a localização física na portaria
* Melhorar a organização visual

A cor é armazenada como entidade no banco de dados, permitindo:

* Padronização
* Expansão futura
* Associação com código HEX

---

## 📦 Funcionalidades (MVP)

### ✔ Moradores

* Cadastrar morador
* Listar moradores
* Buscar por apartamento

### ✔ Encomendas

* Registrar encomenda
* Listar encomendas
* Buscar por morador
* Atualizar status (PENDENTE, ENTREGUE)
* Remover encomenda

---

## 🚀 Tecnologias Utilizadas

* Java
* Spring Boot
* Spring Data JPA
* PostgreSQL
* Maven
* Postman

---

## 🧪 Exemplos de Uso

### Criar encomenda:

* Informar descrição
* Associar ao morador
* Sistema define cor automaticamente

---

## 📈 Evoluções Futuras

* Autenticação (login de porteiro)
* Controle de retirada de encomendas
* Histórico de entregas
* Impressão de etiquetas
* Filtro por bloco/andar
* Dashboard administrativo

---

## 🧠 Decisões Técnicas

* Banco modelado seguindo a 3ª Forma Normal (3FN)
* Separação de responsabilidades por entidade
* Uso de tabela de cores ao invés de ENUM para maior flexibilidade
* API REST seguindo boas práticas

---

## 🎯 Objetivo Profissional

Este projeto foi desenvolvido como prática para:

* Evolução em desenvolvimento backend com Java
* Construção de APIs REST
* Modelagem de banco de dados
* Simulação de problema real de negócio

---

## 💡 Contexto

Este projeto foi inspirado em um cenário real de gestão de encomendas em condomínio residencial, trazendo uma abordagem prática e aplicável ao dia a dia.
