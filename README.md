# Ingestão de dados com OpenMetadata, Apache Airflow e Trino

## 📝 Descrição do Projeto
Este repositório contém um projeto que demonstra o uso de **OpenMetadata** para gestão de metadados, **Apache Airflow** para orquestração de pipelines, e **Trino** para execução de consultas distribuídas em grandes volumes de dados. 

O objetivo é facilitar o monitoramento, a catalogação e o processamento de dados de forma eficiente e escalável.

## 🛠️ Tecnologias Utilizadas
- **OpenMetadata**: Ferramenta para gestão de metadados e integração com ferramentas de ingestão.
- **Apache Airflow**: Plataforma para orquestração de workflows.
- **Trino**: Engine SQL distribuída para análise de dados.

## 📂 Estrutura do Repositório
```plaintext
openmetadata.data-management/
├── data/
│   ├── tiktok_dataset.csv      # Dados a serem adicionados ao banco MySQL
├── trino/
│   ├── catalog/
│   │   ├── mysql.properties    # Propriedades do banco MySQL
│   ├── Dockerfile              # Dockerfile para adicionar o MySQL ao catálogo do Trino
├── docker-compose.yml          # Configuração dos containers Docker
└── README.md                   # Documentação do projeto
```

## 🚀 Configuração e Execução

### Passos para Configuração
1. Clone o repositório:
 ```bash
git clone https://github.com/serpicode/openmetadata.data-management.git
cd openmetadata.data-management
```

2. Inicie os serviços:
```bash   
docker compose -f docker-compose.yml up --detach
```

## 🗒️ Notas
É preciso adicionar os dados (tiktok_dataset.csv) manualmente ao banco de dados para poder visualizá-los com o OpenMetaData.
