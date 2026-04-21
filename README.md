# Eco-Flow-Urban-Management
An AI-Driven Urban Management System using Kafka, Spark, and LSTM for real-time traffic and noise detection


Project Overview
Eco-Flow is an intelligent urban infrastructure framework designed to transition city management from reactive to proactive. By integrating real-time IoT data ingestion with advanced predictive analytics, the system monitors and optimizes urban "flows"—specifically focusing on traffic congestion and noise pollution. The project leverages a containerized microservices architecture to ensure scalability and reliability in a smart city environment.

Key Features
Real-Time Data Ingestion: Utilizes Apache Kafka as a high-throughput message broker to handle continuous data streams from distributed urban sensors.

Predictive Intelligence: Employs an LSTM (Long Short-Term Memory) neural network, trained in Google Colab, to perform time-series forecasting and classify urban noise patterns (e.g., sirens, traffic, construction).

Distributed Processing: Uses Apache Spark Streaming to process live data pipelines, enabling sub-second decision-making and resource optimization.

Containerized Infrastructure: Orchestrated via Docker Compose, ensuring seamless deployment and environment consistency across Zookeeper, Kafka, and Spark clusters.

System Architecture
Perception Layer: Python-based producers simulate IoT sensors generating real-time traffic and acoustic data.

Transport Layer: Kafka topics act as the system's "nervous system," decoupling data production from consumption.

Processing Layer: Spark consumers ingest Kafka streams and apply the pre-trained LSTM model for real-time inference.

Application Layer: Insights are outputted for urban planning dashboards, triggering alerts for noise violations or traffic bottlenecks.
