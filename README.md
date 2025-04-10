# sonarqube_intergration_jenkins_maven

# 🔍 SonarQube (Docker) + Jenkins + Maven Integration


## 🛠️ Tools Required

- Docker
  
- Java (JDK 8 or higher)
- Apache Maven
- Jenkins
- Git

---

## 🚀 Step-by-Step Instructions

### 🐳 1. Run SonarQube with Docker

```bash

# Run SonarQube container
docker run -itd --name SonarQube-Server -p 9000:9000 sonarqube:lts-community
