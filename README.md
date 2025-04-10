# sonarqube_intergration_jenkins_maven

# 🔍 SonarQube (Docker) + Jenkins + Maven Integration


## 🛠️ Tools Required

- EC2 Instance (Ubuntu)
  
- Docker
  ```bash
  sudo apt install docker.io
  
- Java (JDK 8 or higher)
  ```bash
  sudo apt install openjdk-17-jkd -y
  
- Apache Maven
  
- Jenkins
  ```bash
  sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
  echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
  sudo apt-get update
  sudo apt-get install Jenkins
 
- Git

---

## 🚀 Step-by-Step Instructions

### 🐳 1. Run SonarQube with Docker

```bash

# Run SonarQube container
docker run -itd --name SonarQube-Server -p 9000:9000 sonarqube:lts-community


