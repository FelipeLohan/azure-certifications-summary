
# 📊 Resumo AZ-900: Dados, Big Data e IA na Azure

**Tags:** `#AZ-900` `#AzureData` `#BigData` `#MachineLearning` `#Analytics`

## 1. Soluções de Armazenamento de Dados (Banco de Dados)

A Azure oferece bancos de dados relacionais e não-relacionais (NoSQL).

- **Azure Cosmos DB:** Banco de dados **NoSQL** extremamente rápido, com distribuição global e baixa latência.
    - _Buzzwords:_ "Globalmente distribuído", "Escalabilidade horizontal", "NoSQL".
    
- **Azure SQL Database:** Banco de dados relacional (RDBMS) baseado no Microsoft SQL Server. É um serviço **PaaS**.
    - _Buzzwords:_ "Relacional", "SQL Server", "PaaS".
    
- **Azure Database for MySQL/PostgreSQL:** Versões totalmente gerenciadas (PaaS) desses bancos de dados de código aberto.

## 2. Soluções de Big Data e Analytics

Serviços para processar e analisar volumes massivos de dados (Petabytes).

- **Azure Synapse Analytics:** É um serviço de análise ilimitado que reúne data warehousing corporativo e análise de Big Data.
    - _Foco:_ É a "central" de análise que une o mundo do SQL e do Spark.

- **Azure HDInsight:** Um serviço de análise de código aberto gerenciado. Permite rodar frameworks como **Hadoop, Spark e Kafka**.
    - _Foco:_ Quando o cenário exige ferramentas de código aberto específicas.

- **Azure Databricks:** Uma plataforma de análise baseada em **Apache Spark**, otimizada para a Azure e focada em colaboração entre cientistas de dados e engenheiros.

- **Azure Data Lake Storage:** Repositório escalável para armazenar grandes quantidades de dados brutos (não estruturados) antes de serem processados.


## 3. Inteligência Artificial e Machine Learning

A prova divide isso entre ferramentas para cientistas de dados e ferramentas prontas para desenvolvedores.

- **Azure Machine Learning:** Uma plataforma completa para criar, treinar e implantar modelos de aprendizado de máquina.
    - _Público:_ Cientistas de dados que precisam de controle total do ciclo de vida do modelo.

- **Azure AI Services (Antigos Cognitive Services):** APIs prontas para uso que permitem adicionar inteligência aos apps sem precisar ser um expert em IA.
    - _Exemplos:_ Visão computacional (reconhecer imagens), Linguagem (tradução), Fala (texto para voz).

- **Azure AI Bot Service:** Plataforma para criar bots inteligentes que podem interagir via chat, e-mail ou voz.

---

## 📑 Tabela Comparativa para a Prova

|**Serviço**|**Tipo**|**Diferencial**|
|---|---|---|
|**Cosmos DB**|NoSQL|Baixíssima latência em escala global.|
|**Synapse Analytics**|Big Data|Integração total de BI, SQL e Big Data em um só lugar.|
|**HDInsight**|Big Data|Uso de frameworks Open Source (Hadoop/Spark).|
|**Azure ML**|IA/ML|Ambiente para **criar** e **treinar** modelos do zero.|
|**AI Services**|IA/ML|**APIs prontas** (Visão, Fala, Tradução).|

---

> [!tip] Callout de Revisão: Synapse vs. Databricks
> 
> Se a questão falar em **Data Warehouse moderno** e integração com Power BI, pense em **Synapse**. Se falar em **processamento colaborativo em Spark** focado em Ciência de Dados, pense em **Databricks**.
