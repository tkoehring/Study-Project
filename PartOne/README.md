# 📚 ML + AWS + Docker/Kubernetes Study Plan (8 Weeks)

**Goal:** Reach ML Engineer 1 level proficiency, gain AWS Cloud Practitioner & AI Practitioner certifications, and become comfortable with Docker & Kubernetes.  
**Schedule:** 2–4 hrs/day, 5 days/week (~15–20 hrs/week).  

---

## 📅 Week 1 – Machine Learning Fundamentals + AWS Basics
- **Machine Learning:**
  - Regression (linear/logistic): intuition, implementation in scikit-learn, metrics (MSE, accuracy).
  - Classification: decision boundaries, confusion matrix, ROC-AUC.
  - Loss functions: why MSE, cross-entropy, hinge loss matter.
  - Overfitting: causes, detection, regularization (L1/L2), train/test splits.
- **AWS:**
  - AWS global infrastructure (regions, AZs, VPCs).
  - IAM basics (roles, policies, least privilege).
  - S3 for storage, EC2 for compute.
- **Resources:**  
  - Andrew Ng ML Coursera (Weeks 1–2)  
  - AWS Cloud Practitioner Essentials (free digital training)  
  - Book: *Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow* (Ch. 1–3)

✅ **Checkpoint:** Implement linear regression in Python from scratch and deploy a dataset into S3.  

---

## 📅 Week 2 – Supervised Learning + Docker Basics
- **Machine Learning:**
  - Decision Trees, Random Forests, Gradient Boosted Trees.
  - Bias-variance tradeoff.
  - Model evaluation (cross-validation, learning curves).
- **Docker:**
  - Images, containers, volumes, networks.
  - Dockerfile basics, building and running containers.
  - Containerizing a simple Python app.
- **Resources:**  
  - Fast.ai Intro to ML  
  - Docker Docs: Get Started  
  - YouTube: TechWorld with Nana – Docker explained  

✅ **Mini Project:** Train a Random Forest model, save with `joblib`, containerize inference script in Docker.  

---

## 📅 Week 3 – Neural Networks + AWS ML Services
- **Machine Learning:**
  - Basics of neural networks (forward/backprop).
  - Activation functions (ReLU, sigmoid, tanh).
  - Optimization (SGD, Adam).
- **AWS:**
  - SageMaker basics: training jobs, endpoints.
  - CloudWatch logging & monitoring.
  - Security with IAM roles for ML.
- **Resources:**  
  - DeepLearning.AI TensorFlow Specialization  
  - AWS SageMaker Workshop (official)  

✅ **Checkpoint:** Deploy a small neural network using SageMaker built-in algorithms.  

---

## 📅 Week 4 – Model Deployment + Kubernetes Basics
- **Machine Learning:**
  - Model serving strategies (batch vs real-time).
  - Serialization with `pickle`, `joblib`, TorchScript, TF SavedModel.
- **Kubernetes:**
  - Pods, deployments, services.
  - ConfigMaps, secrets.
  - Minikube for local testing.
- **Resources:**  
  - *Kubernetes Up & Running* (Ch. 1–3)  
  - YouTube: Nana’s Kubernetes explained  

✅ **Mini Project:** Wrap a trained model in FastAPI → containerize → deploy to Minikube.  

---

## 📅 Week 5 – Advanced AWS + Kubernetes Scaling
- **AWS:**
  - IAM advanced (assume roles, cross-account access).
  - Networking (VPC, subnets, security groups).
  - Load balancing (ELB, ALB).
- **Kubernetes:**
  - Scaling with replicas, HPA (Horizontal Pod Autoscaler).
  - Monitoring (Prometheus/Grafana).
  - Logging best practices.
- **Resources:**  
  - AWS Well-Architected Labs  
  - Kubernetes Docs: Workloads & Services  

✅ **Checkpoint:** Deploy ML inference API on AWS EKS cluster.  

---

## 📅 Week 6 – MLOps Essentials
- ML pipeline concepts: data → training → validation → deployment.
- Experiment tracking (MLflow basics).
- Model monitoring: drift, latency, failure handling.
- CI/CD for ML (basic GitHub Actions to build & push Docker image).
- **Resources:**  
  - Google MLOps Whitepaper  
  - Made With ML (MLOps section)  

✅ **Mini Project:** Automate training & deployment pipeline with MLflow + GitHub Actions.  

---

## 📅 Week 7 – Capstone Project
### 📦 Project Components
1. **Modeling:**
   - Use an existing classification model (from Week 2 or 4).
   - Export model using `joblib` or `pickle`.

2. **API Service:**
   - Flask or FastAPI app that loads the model and provides a `/predict` endpoint.
   - JSON input/output, proper validation and error handling.

3. **Dockerization:**
   - Dockerfile for app, use slim Python base image.
   - `docker-compose` for local dev/test.

4. **Kubernetes Setup:**
   - YAML manifests for deployment, service, configMap.
   - Add resource requests, readiness/liveness probes.
   - Test locally with Minikube.

5. **AWS Deployment:**
   - Deploy to AWS EKS.
   - Configure `kubectl`, IAM roles, and load balancer.
   - Validate endpoint accessibility.

---

## ✅ Week 7 Deliverables / Checkpoints
- ✅ Fully functional and documented GitHub repository:
  - `README.md` with project overview, setup instructions, and screenshots.
  - Dockerfile, `docker-compose.yml`, and all K8s manifests.
- ✅ Public demo (if possible):
  - Host on a temporary EC2, EKS LoadBalancer, or similar.
  - Share a testable URL or include CLI walkthrough.
- ✅ Resume-ready bullet point:
  - "Developed and deployed a containerized ML inference API using Docker, Kubernetes, and AWS EKS as part of a production-style MLOps capstone."

---

## 📅 Week 8 – Review + Mock Interviews
- **Review:** ML concepts (bias-variance, overfitting, evaluation metrics).  
- **AWS exam prep:** Cloud Practitioner + AI Practitioner practice exams.  
- **Docker/K8s:** commands, YAML manifests, scaling.  

### 🎤 Mock Interview Questions
**Easy:**
- What’s the difference between supervised and unsupervised learning?  
- What is a Dockerfile?  
- What is a Kubernetes Pod?  
- How do you evaluate a classification model?  

**Moderate:**
- Explain precision vs recall tradeoff.  
- Walk me through deploying a containerized ML API.  
- What happens when you run `kubectl apply -f deployment.yaml`?  
- How does SageMaker simplify ML workflows?  

**High-Probability:**
- Describe an ML project you’ve built end-to-end.  
- How would you handle model drift in production?  
- How do you scale an ML inference API to handle traffic?  
- What steps secure an AWS ML deployment?  

---

✅ **End Result:**  
- AWS Certified Cloud Practitioner + AI Practitioner ready  
- Intermediate Docker + Kubernetes  
- A full-stack ML inference system deployed to AWS (resume portfolio project)  
- Confidence for ML Engineer 1–level interviews  
