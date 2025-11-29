# Projeto Banco de Dados - Hospital

Trabalho da disciplina de Banco de Dados utilizando MongoDB para modelar o sistema de um hospital, incluindo:

- Controle de **consultas**, **receitas médicas**, **médicos**, **pacientes** e **convênios**.
- Controle de **internações**, **quartos**, **tipos de quarto** e **profissionais de enfermagem**.

## Estrutura do projeto

- `docs/modelagem_hospital.md`  
  Descrição da modelagem das coleções (Partes 1 e 2 da atividade).

- `scripts/parte3_populamento.js`  
  Scripts de inserção (povoamento) das coleções: especialidades, convênios, médicos, pacientes, tipos de quarto, quartos, enfermeiros, consultas e internações.

- `scripts/parte4_atualizacoes.js`  
  Scripts de alteração de dados e estrutura (adição da coluna/campo `em_atividade` para médicos, com atualização de valores).

- `scripts/parte5_consultas.js`  
  Script com consultas (queries) em MongoDB para responder às questões da Parte 5.

## Como executar no MongoDB

1. Abra o shell do MongoDB (ou use o MongoDB Compass com scripts).
2. Execute:

```js
use HospitalFundamental;

// Parte 3 – povoamento inicial
load("scripts/parte3_populamento.js");

// Parte 4 – alterações (campo em_atividade nos médicos)
load("scripts/parte4_atualizacoes.js");

// Parte 5 – consultas
// (você pode carregar o arquivo ou copiar/colar as consultas conforme necessário)
load("scripts/parte5_consultas.js");
