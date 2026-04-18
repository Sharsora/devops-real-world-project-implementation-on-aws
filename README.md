# Project: Retail Store Sample App


<img width="983" height="591" alt="image" src="https://github.com/user-attachments/assets/a215399b-9afe-4a29-bbd0-a353efa88ef7" />


In this section, we’ll introduce the **Retail Store Sample App** — a real-world, cloud-native microservices application built and maintained by AWS Containers team. We’ll use this app.

---

### **Section 1: Project Overview**
**Module-01:** Complete Retail Store Microservices Architecture
- Full-stack e-commerce application with 5 microservices
- Multi-language stack (Java Spring Boot, Node.js, Go)
- Production-grade architecture patterns

---

### **Section 2: Docker Commands (3 Demos)**
**Module-02:** Docker Fundamentals and Essential Commands
1. EC2 Docker Setup - Installing Docker on AWS Amazon Linux 2023
2. Pull from Docker Hub and Run Containers
3. Build Docker Images and Push to DockerHub
   - Docker CLI: `pull`, `run`, `exec`, `stop`, `start`, `rm`, `rmi`, `logs`, `inspect`
   - Container lifecycle management
   - Image registry operations

---

### **Section 3: Dockerfile Mastery (1 Comprehensive Demo)**
**Module-03:** Building Custom Docker Images
- **Dockerfile Instructions:** `FROM`, `LABEL`, `COPY`, `ADD`, `ARG`, `ENV`, `RUN`, `EXPOSE`, `CMD`, `ENTRYPOINT`, `WORKDIR`, `HEALTHCHECK`, `USER`
- Security best practices
- Multi-stage builds for optimization
- Image layer caching strategies

---

### **Section 4: Docker Compose (1 Comprehensive Demo)**
**Module-04:** Multi-Container Application Orchestration
- Docker Compose basics with real microservices
- Named volumes, networks, and health checks
- Scaling services with DEPLOY
- Startup order with dependencies and conditions
- Profiles, links, and aliases

---

### **Section 5: Docker BuildKit (1 Comprehensive Demo)**
**Module-05:** Advanced Docker Builds
- Docker BuildKit and `buildx` CLI
- Building multi-platform images (AMD64, ARM64)
- Multi-stage builds for production optimization

---

### **Section 6: Terraform Basics (7 Demos)**
**Module-06:** Infrastructure as Code Fundamentals
1. Terraform Tools Installation (AWS CLI, Terraform, kubectl)
2. Terraform Foundation - Providers, Resources, Variables, Outputs
3. Build Production VPC with Public/Private Subnets
4. VPC with tfvars - Variable Management
5. Remote Backend with S3 and DynamoDB State Locking
6. VPC with Remote Backend - Production Setup
7. VPC Terraform Module - Creating Reusable Infrastructure
   - **Key Concepts:** State management, variable precedence, data sources, modules

---

### **Section 7: Terraform EKS Cluster (1 Comprehensive Demo)**
**Module-07:** Complete AWS EKS Cluster with Terraform
- EKS cluster provisioning
- EKS node groups configuration
- IAM roles for EKS cluster and worker nodes
- kubectl and kubeconfig configuration
- Cluster authentication and authorization

---

### **Section 8: Kubernetes Foundation (5 Demos)**
**Module-08:** Kubernetes Core Concepts
1. Kubernetes Pods - Creating and Managing
2. Kubernetes Deployments - Declarative Updates
3. Kubernetes Services - ClusterIP
4. Kubernetes ConfigMaps - Environment Variables and Configuration
5. Kubernetes StatefulSets - Stateful Applications
   - **Additional Topics:** Labels, selectors, annotations, liveness probes, readiness probes, resource requests/limits

---

### **Section 9: Kubernetes Secrets (4 Demos)**
**Module-09:** Secrets Management
1. Kubernetes Secrets Basics
2. EKS Pod Identity Agent Setup
3. AWS Secrets Manager Driver Installation
4. AWS Secrets Manager Catalog Service Integration
   - External Secrets Operator
   - Secrets CSI Driver
   - Mounting secrets as files and environment variables

---

### **Section 10: Kubernetes Persistent Storage (3 Demos)**
**Module-10:** Storage and Databases
1. AWS EBS CSI Driver Installation
2. EBS CSI Integration with Catalog Service
3. AWS RDS MySQL Production Database Integration
   - PersistentVolumes (PV) and PersistentVolumeClaims (PVC)
   - StorageClasses and dynamic provisioning
   - StatefulSets with persistent storage

---

### **Section 11: Kubernetes Ingress (3 Demos)**
**Module-11:** Load Balancing and Ingress
1. AWS Load Balancer Controller Installation
2. Kubernetes Ingress with HTTP
3. Kubernetes Ingress with HTTPS/SSL
   - Application Load Balancer (ALB) configuration
   - SSL/TLS termination with AWS Certificate Manager
   - Health checks and target group configuration

---

### **Section 12: Helm Package Manager (5 Demos)**
**Module-12:** Kubernetes Application Management
1. Helm Basics - Installation and Fundamentals
2. Helm Custom Values - Customization and Overrides
3. Helm Chart Exploration - Understanding Chart Structure
4. Helm Package and Publish - Creating and Publishing Charts
5. Helm Retail Store Deployment - Complete Application

---

### **Section 13: Terraform EKS Cluster with Add-Ons (1 Comprehensive Demo)**
**Module-13:** Production-Ready EKS with Add-Ons
- AWS Load Balancer Controller Add-On
- EBS CSI Driver Add-On
- Pod Identity Agent Add-On
- AWS Load Balancer Controller
- Secret Store CSI Driver
- AWS Secrets and Configuration Provider (ASCP)

---

### **Section 14: Retail Store Microservices - AWS Data Plane (2 Demos)**
**Module-14:** Real-World Microservices Deployment

**1. Retail Store AWS Data Plane Setup**
- AWS RDS for MySQL (Catalog Service Relational database)
- Amazon ElastiCache for Redis (Checkout Service cache)
- Amazon SQS for Messaging (Orders Service Message broker)
- Amazon DynamoDB (Carts Service NoSQL Database)
- Amazon RDS for PostgreSQL (Orders Service Relational Database)
- Terraform automation for AWS services

**2. Microservices with AWS Data Plane Integration**
- UI Service (Spring Boot)
- Carts Service (Spring Boot + DynamoDB)
- Catalog Service (Go + Amazon MySQL/RDS)
- Orders Service (Spring Boot + PostgreSQL/RDS)
- Checkout Service (Node.js + Redis + SQS)
- End-to-end integration and testing

---

### **Section 15: Terraform EKS with External DNS (1 Comprehensive Demo)**
**Module-15:** Automated DNS Management
- External DNS Add-On installation with Terraform
- Automatic DNS record creation in Route53
- Custom domain configuration
- Integration with AWS Load Balancer Controller

---

### **Section 16: Retail Store with External DNS (1 Demo)**
**Module-16:** Production DNS Setup
- Retail Store application with custom domains
- SSL certificate automation with ACM
- Production DNS management

---

### **Section 17: Autoscaling - Karpenter (4 Demos)**
**Module-17:** Pod-Driven Node Autoscaling

**1. Karpenter Installation with Terraform**
- Architecture deep dive
- IAM roles and permissions
- EventBridge and SQS for spot interruption handling

**2. Karpenter On-Demand Instances**
- NodePools and EC2NodeClass configuration
- Right-sizing nodes for workloads
- Node consolidation

**3. Karpenter Spot Instances**
- 70% cost savings with Spot
- Spot NodePool configuration
- Instance diversification strategy

**4. Karpenter Spot Interruption Handling**
- Understanding 2-minute Spot interruption warning
- EventBridge → SQS → Karpenter flow
- Graceful pod eviction and rescheduling
- PodDisruptionBudgets for zero downtime
- Production-ready Spot strategy

---

### **Section 18: Autoscaling - HPA (1 Comprehensive Demo)**
**Module-18:** Horizontal Pod Autoscaler
- Metrics Server installation
- CPU-based and memory-based autoscaling
- HPA + Karpenter integration (HPA scales pods, Karpenter scales nodes)

---

### **Section 19: Helm Retail Store with AWS Data Plane (1 Comprehensive Demo)**
**Module-19:** Complete Helm Deployment
- Deploying full retail store with Helm
- Separate charts for each microservice
- Managing AWS data plane services with Helm
- Environment-specific values
- Chart versioning and release management

---

### **Section 20: Observability - OpenTelemetry (4 Demos)**
**Module-20:** Production Observability Stack

**1. EKS Environment with ADOT (AWS Distro for OpenTelemetry)**
- ADOT Operator installation
- OTEL Collector architecture

**2. OpenTelemetry Traces with AWS X-Ray**
- Auto-instrumentation for Java Spring Boot
- Auto-instrumentation for Node.js
- Trace sampling and filtering
- Cost optimization (85% reduction filtering health checks)
- Service maps and trace analysis

**3. OpenTelemetry Logs with CloudWatch**
- Log aggregation and analysis
- CloudWatch Insights queries

**4. OpenTelemetry Metrics with AMP & AMG**
- Amazon Managed Prometheus setup
- Amazon Managed Grafana setup
- Custom dashboards creation
- Application metrics and business KPIs

---

### **Section 21: DevOps CI/CD Pipeline (4 Demos)**
**Module-21:** Complete CI/CD with GitOps

**1. CI with GitHub Actions and AWS ECR**
- GitHub Actions workflow fundamentals
- Building Docker images
- OIDC authentication (No access keys!)
- Semantic versioning with Git tags

**2. ArgoCD Installation**
- Installing ArgoCD on EKS
- ArgoCD architecture and components
- GitOps principles

**3. CD with ArgoCD and Helm**
- Creating ArgoCD applications
- Helm integration
- Auto-sync and self-heal

**4. Complete CI/CD Flow Testing**
- Code commit → Build → Push to ECR → Update Helm values → ArgoCD deploys
- End-to-end demonstration
- Rollback strategies

---

## DevOps Technologies & Tools Covered

### **1. Docker & Containerization**
   - Docker installation, commands, and lifecycle management
   - Dockerfile instructions and multi-stage builds
   - Docker Compose for multi-container applications
   - Docker BuildKit and multi-platform images
   - Container security and best practices

### **2. Terraform Infrastructure as Code**
   - Terraform fundamentals (providers, resources, variables, outputs)
   - State management (local and remote with S3/DynamoDB)
   - Terraform modules for reusability
   - AWS VPC architecture
   - EKS cluster provisioning
   - EKS Add-Ons management
   - AWS services automation (RDS, ElastiCache, DynamoDB, SQS)

### **3. Kubernetes on AWS EKS**
   - Kubernetes core concepts (Pods, Deployments, Services)
   - ConfigMaps and Secrets management
   - Persistent Volumes and StatefulSets
   - Ingress controllers and load balancing
   - RBAC, namespaces, and resource requests and limits
   - Liveness and readiness probes

### **4. Helm Package Manager**
   - Helm charts structure and templating
   - Values files and overrides
   - Chart dependencies and hooks
   - Packaging, versioning, and publishing
   - Managing complex applications

### **5. Autoscaling**
   - **Karpenter:** Pod-driven node autoscaling, On-Demand/Spot provisioning, node consolidation, spot interruption handling
   - **HPA:** CPU/memory-based pod autoscaling, custom metrics
   - Combined HPA + Karpenter strategy

### **6. Observability - OpenTelemetry**
   - AWS Distro for OpenTelemetry (ADOT)
   - Distributed tracing with AWS X-Ray
   - Logs aggregation with CloudWatch
   - Metrics with Amazon Managed Prometheus
   - Dashboards with Amazon Managed Grafana
   - Auto-instrumentation for Java and Node.js

### **7. CI/CD Pipeline**
   - GitHub Actions for continuous integration
   - Docker image building and multi-arch support
   - Amazon ECR integration
   - OIDC authentication
   - ArgoCD for GitOps-based deployment
   - Automated rollouts and rollbacks

### **8. AWS Services Integration**
   - Amazon EKS, VPC, Load Balancer Controller
   - RDS (MySQL), ElastiCache (Redis), DynamoDB, SQS
   - Secrets Manager, X-Ray, CloudWatch
   - Amazon Managed Prometheus, Amazon Managed Grafana
   - ECR, Route53, Certificate Manager

### **9. Real-World Microservices Application**
   - 5-microservice e-commerce application
   - Multi-language (Java Spring Boot, Node.js, Go)
   - Service-to-service communication
   - Database integration (MySQL, DynamoDB, Redis)
   - Message queuing with SQS

### **10. Production Best Practices**
   - Security: RBAC, Secrets Management, IMDSv2
   - Cost Optimization: Spot instances (70% savings), node consolidation
   - High Availability: Multi-AZ, PodDisruptionBudgets
   - Monitoring and alerting
   - GitOps workflows

---

## Additional Reference
Retail Store Sample App GitHub:
- [https://github.com/aws-containers/retail-store-sample-app](https://github.com/aws-containers/retail-store-sample-app)
