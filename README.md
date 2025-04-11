Ìº± Projeto Sement√°rio
Sement√°rio √© um projeto pessoal que registra e analisa dados de sementes que estou germinando em casa. A ideia √© aplicar, de forma pr√°tica e √∫til, conhecimentos em engenharia de dados com ferramentas reais. Todo o pipeline foi pensado para ser funcional localmente, lidando com dados reais do meu dia a dia.

Ì≥å Objetivo
Automatizar a coleta, tratamento, armazenamento e visualiza√ß√£o de dados relacionados √† germina√ß√£o de sementes, permitindo an√°lises como:

Taxa de germina√ß√£o por tipo de semente

Influ√™ncia da esta√ß√£o e temperatura

Tempo m√©dio at√© a germina√ß√£o

Compara√ß√£o entre marcas e m√©todos de plantio

Ì∑± Arquitetura do Pipeline
text
Copiar
Editar
[ Google Sheets ]         [ API Clima ]
       |                        |
       +------------------------+
                 |
        [ Ingest√£o: gdown + requests ]
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
Ì∑∞ Tecnologias e Ferramentas
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

Ì∫ß Status
Ìø¢ Em desenvolvimento
ÌæØ Etapas atuais:

 Defini√ß√£o da arquitetura

 Configura√ß√£o da ingest√£o automatizada

 Cria√ß√£o do modelo Snowflake em SQLite

 Desenvolvimento do dashboard

 Orquestra√ß√£o com Airflow

Ì≥¨ Contato
Se quiser trocar uma ideia sobre o projeto ou algo relacionado:
[Seu Nome] ‚Äî LinkedIn | GitHub
