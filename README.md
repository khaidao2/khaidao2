# Hi, I'm Khai Dao 👋

Data Engineer focused on building end-to-end data platforms — from streaming ingestion and lakehouse storage to orchestration, transformation, and visualization.

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white)
![Apache Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Spark-E25A1C?style=flat&logo=apachespark&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat&logo=dbt&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Google Cloud](https://img.shields.io/badge/GCP-4285F4?style=flat&logo=googlecloud&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Argo CD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat&logo=argo&logoColor=white)

## 🚀 Featured Projects

### 🎵 [Music Stream Data Pipeline](https://github.com/khaidao2/music_stream_pipeline)
A containerized real-time data pipeline that simulates, streams, and analyzes music listening events.
- **Ingest**: `eventsim` generates events → **Kafka** + **Apicurio Schema Registry** (Avro)
- **Process**: **Spark Streaming** consumes Kafka topics and lands partitioned Parquet on **GCS**
- **Load & Transform**: **Airflow** loads GCS data into **BigQuery**, then **dbt** builds analytics-ready models
- **IaC**: GCP infrastructure provisioned with **Terraform**

### 💼 [Job Listings Data Lakehouse](https://github.com/khaidao2/jobs_crawler)
An end-to-end Data Lakehouse for crawling, ingesting, transforming, and visualizing the Vietnamese job market.
- **Crawl**: Python crawlers for TopCV & TopDev
- **Stream & Store**: **Kafka** + **Apicurio** → **MinIO** (S3-compatible Bronze layer)
- **Transform**: **DuckDB** + **dbt** Medallion architecture (staging → intermediate → marts)
- **Orchestrate & Visualize**: **Apache Airflow** scheduling, **Apache Superset** dashboards

### 📊 [Sentiment Pulse](https://github.com/khaidao2/sentiment_pulse)
A GitOps-managed Kubernetes platform for real-time sentiment data, deployed via Argo CD's App-of-Apps pattern.
- **Streaming**: Kafka (KRaft mode) + Kafka UI + Apicurio Schema Registry
- **Orchestration**: Airflow 3.x with FastAPI API server, secured via Keycloak (OIDC)
- **GitOps**: Argo CD manages namespaces, Postgres, Keycloak, Airflow, and OAuth2 Proxy as declarative apps
- **Ingress**: Traefik with custom DNS resolution for internal SSO flows

## 📫 Reach Me

- 🌐 Portfolio: [portfolio-sandy-chi-22.vercel.app](https://portfolio-sandy-chi-22.vercel.app/)
- 💼 LinkedIn: [Khải Đào](https://www.linkedin.com/in/kh%E1%BA%A3i-%C4%91%C3%A0o-043035292/)
- 📧 Email: [daok257@gmail.com](mailto:daok257@gmail.com)
- GitHub: [@khaidao2](https://github.com/khaidao2)
