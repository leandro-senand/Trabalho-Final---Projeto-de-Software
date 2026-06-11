<a href="https://github.com/leandro-sena/bovigest"><img src="https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg" width="200"/></a>

---

# 🏷️ BoviGest - Sistema de Gestão de Gado de Corte 👨‍💻

<div align="center">
  <img src="BoviGest_Logo.png" alt="BoviGest Logo Completo" width="600px"/>
</div>

> [!NOTE]
> Sistema inteligente para apoio e controle completo do ciclo de engorda na pecuária de corte. **Foque na rastreabilidade individual, controle financeiro e eficiência zootécnica.** > <div align="center">
>   <img src="https://img.shields.io/badge/BoviGest-Engorda_Inteligente-darkgreen?style=for-the-badge&logo=google-earth" alt="BoviGest Logo" width="250px"/>
> </div>

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        O <b>BoviGest</b> é um sistema de informação voltado à pecuária de corte, projetado especificamente para gerenciar o ciclo de engorda (recria e terminação). O produtor rural adquire animais jovens (bezerros/garrotes), realiza o manejo sanitário preventivo, controla as pesagens e os custos de alimentação/pastagem e, por fim, vende os animais como boi gordo. O sistema apoia todo esse ecossistema, fornecendo controle financeiro rigoroso, rastreabilidade individual de cada animal e indicadores zootécnicos automáticos cruciais para a tomada de decisões estratégicas e lucratividade no agronegócio.
      </div>
    </td>
    <td>
      <div>
        <img src="https://joaopauloaramuni.github.io/image/logo_ES_vertical.png" alt="Logo do Projeto" width="120px"/>
      </div>
    </td>
  </tr> 
</table>

---

## 🚧 Status do Projeto

[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/joaopauloaramuni/joaopauloaramuni/main.yml?branch=main)](https://github.com/joaopauloaramuni/joaopauloaramuni/actions/workflows/main.yml)
[![Test Coverage](https://codecov.io/gh/joaopauloaramuni/laboratorio-de-desenvolvimento-de-software/branch/main/graph/badge.svg)](https://codecov.io/gh/joaopauloaramuni/laboratorio-de-desenvolvimento-de-software)
[![Versão](https://img.shields.io/badge/Vers%C3%A3o-v1.0.0-blue?style=for-the-badge)](https://github.com/leandro-sena/bovigest/releases)
[![Node.js](https://img.shields.io/badge/Node.js-v20.x-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-19.0-007ec6?style=for-the-badge&logo=react&logoColor=white)](#)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue?style=for-the-badge&logo=postgresql)](#)
[![Redis](https://img.shields.io/badge/Redis-7.2-red?style=for-the-badge&logo=redis)](#)

---

## 📚 Índice
- [Links Úteis](#-links-úteis)
- [Sobre o Projeto](#-sobre-orojeto)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Arquitetura](#-arquitetura)
- [Instalação e Execução](#-instalação-e-execução)
  - [Pré-requisitos](#pré-requisitos)
  - [Variáveis de Ambiente](#-variáveis-de-ambiente)
  - [Instalação de Dependências](#-instalação-de-dependências)
  - [Inicialização do Banco de Dados (PostgreSQL)](#-inicialização-do-banco-de-dados-postgresql)
  - [Como Executar a Aplicação](#-como-executar-a-aplicação)
- [Deploy](#-deploy)
- [Estrutura de Pastas](#-estrutura-de-pastas)
- [Demonstração](#-demonstração)
- [Testes](#-testes)
- [Documentações utilizadas](#-documentações-utilizadas)
- [Autores](#-autores)
- [Contribuição](#-contribuição)
- [Agradecimentos](#-agradecimentos)
- [Licença](#-licença)

---

## 🔗 Links Úteis
* 🌐 **Demo Online:** [Acesse a Aplicação Web do BoviGest](https://bovigest-web.vercel.app)
  > 💻 **Descrição:** Plataforma administrativa para acompanhamento de lotes, lançamentos financeiros e painel de indicadores.
* 📱 **Download Mobile:** [Google Play](https://play.google.com/store/apps/bovigest) | [APK Direto](https://bovigest-web.vercel.app/download/bovigest.apk)
  > 📱 **Descrição:** Aplicativo mobile em React Native focado em lançamentos rápidos diretamente no curral (pesagem e manejo sanitário offline).
* 📖 **Documentação:** [Leia a Wiki/Docs do BoviGest](https://github.com/leandro-sena/bovigest/wiki)
  > 📚 **Descrição:** Documentação técnica contendo o dicionário de dados completo e o mapeamento dos fluxos do C4 Model.

---

## 📝 Sobre o Projeto
O **BoviGest** foi idealizado para suprir a carência de controle analítico e rastreável no gerenciamento do gado de corte voltado para engorda.

- **Por que ele existe** — A falta de dados precisos sobre a evolução do peso individual e custos pulverizados (medicamentos, pastagem, ração) mascara prejuízos ocultos e prejudica a tomada de decisão do pecuarista.
- **Qual problema ele resolve** — Elimina o controle em cadernos ou planilhas descentralizadas, calculando de forma automatizada indicadores vitais como o Ganho Médio Diário (GMD) e o Retorno Sobre Investimento (ROI) de cada animal ou lote comercializado.
- **Qual o contexto** — Trabalho acadêmico final desenvolvido pelo aluno **Leandro Sena de Andrade Machado** para a disciplina de *Projeto de Software* da PUC Minas em **01/06/2026**.
- **Onde ele pode ser utilizado** — Pequenas, médias e grandes propriedades rurais de pecuária de corte que adotem os sistemas de recria e terminação (seja em regime de confinamento, semiconfinamento ou pastejo extensivo).

---

## ✨ Funcionalidades Principais
Com base no mapeamento de requisitos e casos de uso do sistema, as seguintes capacidades são entregues:

- 🐂 **Rastreabilidade Individual (UC-01):** Cadastro detalhado do animal associando brinco físico, raça, sexo, peso inicial e status (Ativo, Vendido, Morto, Descartado).
- 📉 **Gestão de Compras e Lotes (UC-02):** Registro de aquisições de animais calculando automaticamente colunas geradas com o custo total do lote (`quantidade × valor_unitário + frete`).
- ⚖️ **Manejo de Pesagem Automatizado (UC-03):** Registro cronológico de pesagens calculando automaticamente o indicador zootécnico **GMD (Ganho Médio Diário em kg/dia)**.
- 💉 **Controle Sanitário Preventivo (UC-04):** Agendamento e registro de vacinas, vermífugos e tratamentos clínicos calculando datas automáticas para as próximas aplicações (base para alertas).
- 🌾 **Manejo de Pastagens e Custos (UC-05):** Rateio de despesas operacionais da fazenda segmentadas em categorias (Alimentação, Sanidade, Pastagem) vinculando os animais aos respectivos piquetes.
- 🚨 **Mecanismo de Alertas Inteligentes (UC-12):** Notificação automática para animais apresentando perda de peso, GMD abaixo da meta do lote ou manejos sanitários atrasados.
- 📊 **Cotação em Tempo Real (UC-15):** Integração automática via API para consulta e exibição do preço atualizado da arroba do boi gordo utilizando como fonte o **CEPEA**.

---

## 🛠 Tecnologias Utilizadas

### 💻 Front-end
* **Framework/Biblioteca:** React v19.0 (Web) e React Native (Mobile)
* **Linguagem/Superset:** TypeScript
* **Estilização:** Tailwind CSS (Web) e Styled Components (Mobile)
* **Gerenciamento de Estado:** Zustand (ideal para suporte de cache offline no campo)
* **Build Tool:** Vite

### 🖥️ Back-end
* **Linguagem/Runtime:** Node.js v20.x
* **Framework:** Express / NestJS (Arquitetura Stateless orientada a endpoints REST)
* **Banco de Dados:** PostgreSQL 16 (Persistência transacional com integridade referencial estrita)
* **Mapeamento/ORM:** Prisma ORM / Sequelize (Padrão Data Mapper/Active Record)
* **Cache & Mensageria:** Redis v7.2 (Cache local das cotações da arroba do CEPEA e filas de alertas)
* **Autenticação:** JWT (JSON Web Tokens) com controle de perfis de acesso (*Roles*)

### ⚙️ Infraestrutura & DevOps
* **Containerização:** Docker e Docker Compose
* **CI/CD:** GitHub Actions integrado para testes automáticos
* **Hospedagem:** Vercel (Front-end) e Railway/AWS EC2 (Back-end e PostgreSQL)

---

## 🏗 Arquitetura
O sistema segue o modelo arquitetural de **Camadas Desacopladas** mapeado de acordo com o padrão **C4 Model (Nível de Contêineres)** para garantir escalabilidade e independência entre os clientes de visualização e o núcleo de regras de negócios (*Business Logic Layer*).

- **API REST Stateless:** Centraliza o processamento e cálculos complexos (GMD, ROI).
- **Camada de Repositórios:** Comunicação otimizada via SQL com o PostgreSQL utilizando chaves primárias indexadas (UUID) para as transações.
- **Worker Assíncrono:** Serviço em segundo plano dedicado ao envio de notificações de alertas sanitários e atualização de cotações de mercado via Redis.

| Diagrama de Arquitetura | Detalhe da Arquitetura |
| :---: | :---: |
| **Visão Geral (Contêineres C4)** | **Modelo de Dados (Entidades)** |
| <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="C4 Contêineres" width="120px" height="120px"> | <img src="https://joaopauloaramuni.github.io/image/aramunilogo.png" alt="DER" width="120px" height="120px"> |

---

## 🔧 Instalação e Execução

### Pré-requisitos
* **Node.js:** Versão LTS v20.x ou superior
* **Gerenciador de Pacotes:** `npm` ou `yarn`
* **Docker & Docker Compose:** Necessário para rodar o banco de dados e o cache localmente

---

### 🔑 Variáveis de Ambiente

#### 1 Back-end (Node.js/Express)
Crie um arquivo `.env` na raiz da pasta `/backend`:

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `PORT` | Porta onde o Back-end será executado. | `8080` |
| `DATABASE_URL` | URL de conexão JDBC (PostgreSQL). | `postgresql://postgres:senha-segura-123@localhost:5432/bovigest` |
| `REDIS_URL` | URL do servidor de cache Redis. | `redis://localhost:6379` |
| `JWT_SECRET` | Chave secreta de assinatura dos tokens de login. | `bovigest_chave_secreta_pucminas_2026` |

#### 2 Front-end (React, Vite)
Crie um arquivo `.env.local` na raiz da pasta `/frontend`:

```text
VITE_API_URL=http://localhost:8080/api
VITE_CEPEA_INTEGRATION_ENABLED=true
