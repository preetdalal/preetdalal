# Preet Dalal

B.Tech Information Technology, DJSCE Mumbai — specializing in DevOps and Cloud Engineering, with a backend engineering foundation and applied AI/ML experience.

I build backend services in Java and Python, then containerize and deploy them with Docker and Kubernetes, wiring up autoscaling and monitoring along the way. Machine learning is a secondary track I use to build and ship real models, not just notebooks.

---

## Current Focus

- Deploying and operating containerized services on Kubernetes: autoscaling, service architecture, observability
- Backend systems in Spring Boot and FastAPI: auth, caching, migrations, testing
- Linux fundamentals and CI/CD as the backbone of shipping reliably
- Applied ML: training and deploying models behind real APIs, not just experiments

---

## Tech Stack

**Languages**
Java · Python · TypeScript

**Backend**
Spring Boot · FastAPI · REST APIs · Spring Security (JWT) · Spring Data JPA

**DevOps & Cloud**
Docker · Kubernetes (HPA) · Prometheus · Grafana · Linux · Render · Vercel · Hugging Face Spaces

**Databases & Infrastructure**
PostgreSQL · Redis · Flyway

**AI / ML**
PyTorch · TensorFlow · scikit-learn · Computer Vision (segmentation, classification)

**Frontend**
React · Next.js · Tailwind CSS

---

## Featured Projects

### [FraudGuard AI](https://github.com/preetdalal/fraud-detection-system-scoe)
Multi-channel fraud and phishing detection platform analyzing SMS, email, and URLs in real time.

The engineering focus here is the deployment, not just the models. The FastAPI backend and React frontend run as separate services on Kubernetes, with a Horizontal Pod Autoscaler tracking memory utilization to handle bursty inference traffic, plus a `/metrics` endpoint scraped by Prometheus and visualized in Grafana. Detection itself uses TF-IDF classifiers for SMS/email and a Random Forest model for malicious URLs.

`FastAPI` `React` `scikit-learn` `Docker` `Kubernetes` `Prometheus` `Grafana`

### [Job Application Tracker API](https://github.com/preetdalal/job-tracker)
A Spring Boot REST API for tracking job applications, built to cover the backend patterns that show up in production systems rather than a toy CRUD app.

JWT authentication with role-based access, dynamic filtering via JPA Specifications, Redis caching on stats endpoints, scheduled email reminders through Spring Mail, and Flyway-managed migrations. Integration tests run against a real Postgres instance via Testcontainers, and the whole stack (app, Postgres, Redis) runs through Docker Compose.

`Java 17` `Spring Boot` `PostgreSQL` `Redis` `Docker` `Testcontainers`

### [RASC-Net: Adversarial Skin Cancer Defense](https://github.com/preetdalal/adversial-skin-cancer)
A deep learning framework for skin lesion classification that stays accurate under adversarial attacks, plus a clinical decision support layer for reporting.

Built a custom Residual Attention network (2.88M params) trained with a curriculum adversarial schedule, and paired it with a pre-processing defense pipeline (bit-depth reduction, blur, JPEG compression) that recovers accuracy an attacked model would otherwise lose. FGSM-attacked accuracy went from 24% on the baseline to 62.5% with the proposed defenses. Model weights are hosted on Hugging Face Hub since they're too large for standard deployment, with the Flask backend deployable on Hugging Face Spaces or tunneled from a local machine via Microsoft Dev Tunnels.

`PyTorch/TensorFlow` `React` `Docker` `Hugging Face Hub`

### [SVAMITVA AI Feature Extraction](https://github.com/preetdalal/svamvitva-sih) · [demo](https://nerdvana-sih.vercel.app)
Built for Smart India Hackathon: converts drone orthophotos into vector GIS village maps, extracting building footprints, roads, and waterbodies.

A PyTorch U-Net handles semantic segmentation and an EfficientNet-B0 classifies roof material, with custom GIS vectorization (contour extraction, Shoelace area calculation) turning raster masks into real-world measurements. Deployed across three services: FastAPI backend on Render, Next.js frontend on Vercel, and model weights synced from Hugging Face Hub at runtime.

`PyTorch` `FastAPI` `Next.js` `Render` `Vercel` `Hugging Face Hub`

---

## Building Toward

Deliberately deepening the infrastructure side of the stack I already build on:

- CI/CD pipelines for the services above, currently deployed manually
- Deeper Kubernetes: multi-service manifests, ingress, and secrets management beyond a single HPA
- Cloud platforms beyond Render/Vercel free tiers (AWS/GCP fundamentals)
- Infrastructure as code

---

[GitHub](https://github.com/preetdalal) · [LinkedIn](https://linkedin.com/in/preetdalal)
