### preet dalal

```java
public class Preet {
    String study = "B.Tech IT, DJSCE Mumbai (DevOps Honours, GPA 8.4)";
    String[] stack = {"Java/Spring Boot", "Python", "React", "Docker", "Kubernetes"};
    String focus = "backend systems that hold up in production, plus ML on the side";
}
```

---

### FraudGuard AI
Multi-channel fraud and cybersecurity threat detection platform. Analyzes SMS smishing, phishing emails, and malicious URLs in real time with confidence scoring, plus a community threat-sharing feed.

- FastAPI backend with scikit-learn models (Random Forest for URLs, TF-IDF classifiers for SMS/email)
- React 19 + Vite + Tailwind frontend
- Deployed on Kubernetes with Horizontal Pod Autoscaling, Prometheus metrics, and Grafana dashboards
- [Repo](https://github.com/preetdalal/fraud-detection-system-scoe)

### RASC-Net: Adversarial Skin Cancer Defense
Deep learning framework for skin lesion classification that stays robust under adversarial attacks, built around a custom Residual Attention network.

- Curriculum adversarial training (FGSM schedule) plus a multi-stage image defense pipeline (bit-depth reduction, blur, JPEG compression)
- Lightweight backbone at 2.88M params, model weights hosted on Hugging Face Hub
- Clinical decision support layer: patient metadata, rule-based risk scoring, hospital-grade PDF reports
- Raised adversarial accuracy from ~24% to 62.5% (FGSM) over the baseline while keeping clean accuracy competitive
- [Repo](https://github.com/preetdalal/adversial-skin-cancer)

### Job Application Tracker API
Spring Boot 3.2 REST API built on Java 17, in progress.

- JWT authentication, Redis caching, Flyway migrations
- Testcontainers for integration tests, Docker deployment
- [Repo](https://github.com/preetdalal/job-tracker)

---

[LinkedIn](https://linkedin.com/in/preetdalal) · [GitHub](https://github.com/preetdalal)
