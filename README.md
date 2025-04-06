
---
---

#  Module 16: **Logging in Kubernetes with EFK Stack (Elasticsearch, Fluentd, Kibana)**



##  **Introduction – Why Monitoring Is the Heartbeat of DevOps**

Monitoring is not just about graphs and alerts — it’s your **window into system health**. Without it, you’re flying blind.

Monitoring answers questions like:
- Is my app up?
- Is the database under pressure?
- Why are users facing errors?
- Where exactly is a failure happening in production?

Monitoring is **vital** for:
- Troubleshooting bugs  
- Ensuring uptime  
- Meeting SLAs and SLOs  
- Enabling rapid feedback for DevOps loops  

It’s a **core SRE discipline**, and it begins with:  
 **Logging**  
 **Metrics**  
 **Tracing**

This module focuses on the **logging pillar** — and sets the stage for metrics and observability tools coming next.

---
---



---

##  **Module Overview**

This module focuses on setting up **centralized logging** in a Kubernetes environment using the **EFK Stack**. Learners will understand how to collect, process, store, and visualize logs from distributed microservices deployed on a Kubernetes cluster (EKS).

They will learn to:
- Configure microservices (Java/Node.js) to produce structured logs  
- Build and push Docker images to a private registry  
- Deploy those apps on Kubernetes  
- Integrate Fluentd as a log collector using DaemonSet  
- Store logs in Elasticsearch and visualize them using Kibana  
- Understand StatefulSet and Helm concepts in the context of the logging stack

This is a **real-world, end-to-end logging architecture implementation** designed for production-grade systems.

---

##  Key Concepts Covered

###  Importance of Logging in Microservices

- Challenges of log management in distributed systems  
- Logging in monolithic vs microservice environments  
- Role of centralized logging in debugging, tracing, and observability  
- Logging as a prerequisite to monitoring and alerting

---

###  Structured Logging Fundamentals

- Understanding log levels: INFO, DEBUG, ERROR, FATAL  
- Benefits of structured logs (JSON format)  
- Best practices for log enrichment (timestamp, trace ID, service name)

---

###  Java and Node.js App Logging Configuration

- Enable and structure logs in Java (log4j, SLF4J)  
- Logging frameworks in Node.js (winston, pino)  
- Application logging format conventions  
- Injecting environment variables for log level control

---

###  Dockerization and Private Registry Integration

- Creating Dockerfiles for logging-ready applications  
- Building and tagging images  
- Setting up a private Docker registry (Docker Hub, Harbor, ECR)  
- Image pull secrets in Kubernetes

---

###  Kubernetes on AWS (EKS) for Logging Workload

- Creating and managing EKS clusters  
- Namespaces for logical separation (`apps` and `logging`)  
- Configuring image pull policies and RBAC permissions

---

###  ElasticSearch, Fluentd, and Kibana in Kubernetes

- Overview of EFK Stack architecture  
- Roles of each component in centralized logging

#### Elasticsearch
- Log indexing and storage  
- Scaling and resource management  
- StatefulSet in Kubernetes

#### Fluentd
- Log collection and transformation  
- Use of DaemonSet to run on all nodes  
- Parsing logs and forwarding to Elasticsearch  
- Mounting host logs and container logs

#### Kibana
- Visualizing logs  
- Filtering by labels, severity, service  
- Creating log dashboards for operations

---

### ✅ Helm-Based Deployment

- Using Helm to install EFK components  
- Managing versions, upgrades, and rollbacks  
- Helm values customization for EFK tuning

---

###  Real-World Architecture Scenarios

- Full deployment of logging solution in EKS  
- Handling multiple services with different logging formats  
- Centralized dashboards per microservice  
- Securing access to logs and dashboards  
- Cross-node log collection for troubleshooting

---

##  Skills Gained

- Build logging-ready microservices  
- Centralize logs in Kubernetes  
- Understand and apply DaemonSet and StatefulSet  
- Visualize logs for debugging and SRE use cases  
- Deploy EFK stack using Helm on AWS EKS  
- Architect production-grade log pipelines

---

##  Tools and Technologies Used

- **Kubernetes (EKS)**  
- **Elasticsearch**  
- **Fluentd**  
- **Kibana**  
- **Docker + Private Registry**  
- **Helm**  
- **Java / Node.js Logging Libraries**

---
---
