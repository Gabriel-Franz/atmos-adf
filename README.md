# Atmos ADF — Azure Data Engineering Pipeline ☁️

Pipeline de Engenharia de Dados desenvolvida utilizando Azure Data Factory, Azure Databricks e arquitetura Lakehouse para ingestão, processamento e disponibilização de dados climáticos em ambiente cloud.

---

# 🚀 Objetivo

O projeto tem como objetivo construir uma pipeline de dados ponta a ponta utilizando serviços Azure para ingestão automatizada, orquestração, armazenamento e processamento distribuído de dados climáticos provenientes de múltiplas fontes externas.

A solução utiliza Azure Data Factory para orquestração dos pipelines, Azure Storage Account como Data Lake e Azure Databricks para processamento e transformação dos dados utilizando Apache Spark e Delta Lake.

---

# 🛠️ Tecnologias utilizadas

- Azure Data Factory
- Azure Storage Account
- Azure Databricks
- Azure Key Vault
- Google BigQuery
- Apache Spark
- PySpark
- Delta Lake
- Python
- SQL

---

# 🔄 Fluxo da Pipeline

Visual Crossing API / Google BigQuery
                ↓
       Azure Data Factory
                ↓
      Azure Storage Account
                ↓
       Azure Databricks
                ↓
      Camadas Bronze/Silver/Gold
                ↓
        Dashboard Analítico

---
  
# 📂 Arquitetura do Projeto

## 🔹 Ingestão de Dados
- Coleta automatizada de dados climáticos através da API Visual Crossing
- Integração com Google BigQuery para ingestão de datasets adicionais
- Orquestração utilizando Azure Data Factory
- Parametrização de pipelines para execução automatizada

## 🔹 Segurança
- Gerenciamento seguro de credenciais utilizando Azure Key Vault
- Secrets e chaves de API armazenadas fora do código

## 🔹 Armazenamento
- Persistência dos dados no Azure Storage Account
- Estruturação dos dados em Data Lake

## 🔹 Processamento
- Transformações distribuídas utilizando Azure Databricks e Apache Spark
- Padronização e tratamento dos dados
- Escrita das tabelas em formato Delta Lake

## 🔹 Camada Analítica
- Organização dos dados na arquitetura Medallion (Bronze, Silver e Gold)
- Criação de tabelas analíticas para consumo e visualização

---

# 🖼️ Arquitetura e Componentes

## Resource Group

![Resource Group](images/resource-group.png)

---

## Azure Storage Account

![Storage](images/storage.png)

---

## Azure Key Vault

![Key Vault](images/keyvault.png)

---

## Azure Data Factory Pipeline

![ADF Pipeline](images/adf-pipeline.png)

---

# 🧠 Decisões Técnicas

## Azure Data Factory
Responsável pela orquestração das pipelines e ingestão automatizada dos dados provenientes das fontes externas.

## Azure Key Vault
Utilizado para armazenamento seguro de secrets e credenciais, evitando exposição de chaves diretamente no código.

## Delta Lake
Utilizado para garantir confiabilidade, versionamento e melhor performance nas operações de leitura e escrita.

## Medallion Architecture
Separação das camadas Bronze, Silver e Gold para melhor governança, organização e qualidade dos dados.


# ⚙️ Funcionalidades

- Pipelines automatizadas no Azure Data Factory
- Orquestração de fluxos de dados
- Integração com Azure Databricks
- Processamento distribuído com Spark
- Armazenamento em Delta Lake
- Estrutura escalável para projetos de Engenharia de Dados
- Integração com Google BigQuery
- Gerenciamento seguro de secrets com Azure Key Vault

---

# 📊 Resultados

O projeto realiza a ingestão e processamento automatizado de dados climáticos provenientes de múltiplas fontes externas, organizando os dados em uma arquitetura Medallion (Bronze, Silver e Gold) para consumo analítico e visualização.

A solução foi construída utilizando serviços Azure focando em escalabilidade, organização e boas práticas de Engenharia de Dados.

---

# ▶️ Como executar o projeto

## Clone o repositório

```bash
git clone https://github.com/Gabriel-Franz/atmos-adf.git
