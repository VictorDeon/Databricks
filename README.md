## Engenharia de Dados do Tico Creator

| Funcionalidade / Caso de Uso| Em Databricks| Equivalente Principal no GCP|
|-----------------------------|--------------|-----------------------------|
| Processamento de Dados (ETL/ELT) | Notebooks e Jobs Spark | Dataproc (para rodar Spark/Hadoop) ou BigQuery (para ELT baseado em SQL) ou Dataflow (para processamento serverless em batch/streaming). |
| Notebooks e Data Science | Notebooks Databricks | Vertex AI Workbench (ambiente de notebooks Jupyter gerenciado e integrado ao ecossistema de IA do GCP). |
| Machine Learning (MLOps) | MLflow (rastreamento, registro) | Vertex AI Platform (inclui Vertex AI Experiments, Model Registry, Training, Prediction). É a solução MLOps completa do GCP. |
| Data Warehouse & SQL Analytics | Databricks SQL | BigQuery. Este é o carro-chefe do GCP, um data warehouse serverless, massivamente escalável e frequentemente mais performático e econômico para análise SQL. |
| Arquitetura Lakehouse (Delta Lake) | Delta Lake sobre um Data Lake (GCS) | BigQuery + BigLake + Google Cloud Storage (GCS). Com o BigLake, o BigQuery pode consultar dados em formatos abertos (Parquet, ORC) no GCS com governança e performance, criando uma arquitetura lakehouse nativa. |
| Orquestração de Workflows | Databricks Jobs | Cloud Composer (versão gerenciada do Apache Airflow) ou Workflows. |
| Governança e Catálogo de Dados | Unity Catalog | DataPlex (para gerenciamento de data lakes e data meshes) e Data Catalog (para descoberta e metadados). |