� Projeto Sementário
Sementário é um projeto pessoal que registra e analisa dados de sementes que estou germinando em casa. A ideia é aplicar, de forma prática e útil, conhecimentos em engenharia de dados com ferramentas reais. Todo o pipeline foi pensado para ser funcional localmente, lidando com dados reais do meu dia a dia.

� Objetivo
Automatizar a coleta, tratamento, armazenamento e visualização de dados relacionados à germinação de sementes, permitindo análises como:

Taxa de germinação por tipo de semente

Influência da estação e temperatura

Tempo médio até a germinação

Comparação entre marcas e métodos de plantio

� Arquitetura do Pipeline
text
Copiar
Editar
[ Google Sheets ]         [ API Clima ]
       |                        |
       +------------------------+
                 |
        [ Ingestão: gdown + requests ]
                 |
        [ Bronze - /data/raw ]
                 |
    [ Silver - Limpeza (Python + Pandas) ]
                 |
 [ Gold - SQLite3 (Modelo Snowflake) ]
                 |
     [ Streamlit Dashboard ]
                 |
         [ Airflow Orquestra ]
� Tecnologias e Ferramentas
Python

Pandas

SQLite3

gdown + PyDrive

requests

Streamlit

Apache Airflow

Google Sheets

API de clima (OpenWeatherMap ou Visual Crossing)

Git/GitHub

� Status
� Em desenvolvimento
� Etapas atuais:

 Definição da arquitetura

 Configuração da ingestão automatizada

 Criação do modelo Snowflake em SQLite

 Desenvolvimento do dashboard

 Orquestração com Airflow

� Contato
Se quiser trocar uma ideia sobre o projeto ou algo relacionado:
[Seu Nome] — LinkedIn | GitHub
