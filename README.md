# 🔍 AWS Glue Log Optimizer – Hackathon Cubo Itaú 2025

Este projeto foi desenvolvido como solução para o **Hackathon Cubo Itaú 2025**, com foco na **redução de custos com loggers em microserviços** implementados via AWS Glue.

## 💡 Desafio

Muitos microserviços legados e novos, implementados em ambientes distribuídos, geram logs desnecessários ou mal estruturados. Isso causa um aumento significativo nos custos de armazenamento e observabilidade. Este script automatiza a detecção e correção desses problemas.

## 🚀 O que o script faz

- 🔎 **Varredura automatizada** de todos os microserviços registrados no AWS Glue.
- 🤖 Utilização de um modelo LLM (via AWS Bedrock) para analisar os scripts de ETL.
- 🧠 **Identificação de padrões incorretos de logging** que resultam em custo extra.
- 🛠️ **Recriação automática do código** para corrigir problemas de logging.
- 🔄 Funciona para **serviços legados** e **novos microserviços** com más práticas.
- 💸 Reduz significativamente o **custo operacional com logs** na nuvem.

## 🛠️ Tecnologias e Ferramentas

- `boto3` – Interação com serviços AWS (Glue, S3, Bedrock)
- `awswrangler` – Integração com Glue Data Catalog e S3
- `pandas` – Manipulação de dados
- `Amazon Bedrock` – Análise e geração de código via LLM

## 📦 Pré-requisitos

- Python 3.8+
- Conta AWS com permissões para acessar:
  - Glue (`glue:GetJobs`)
  - S3
  - Bedrock Runtime
- As seguintes bibliotecas instaladas:
  ```bash
  pip install boto3 awswrangler pandas
