# Spring Boot Legacy Security Demo  

## Overview  
This repository is a **demo showcasing an older version of Spring Boot** that is **no longer publicly maintained for security patches** by the Spring team.  

While regular Spring users can upgrade to the latest version to receive ongoing security updates, **organizations relying on older versions** must either:  
- Upgrade to a **supported** Spring version, or  
- **Obtain commercial support** for backported security fixes.  

This demo highlights the **risks of running outdated Spring versions** and demonstrates how to assess your application's dependency health.  

## Spring Health Assessment  

Our **Spring Health Assessment** report helps you understand the **health of your Spring dependencies**. The generated report will provide:  
✅ **Security vulnerability analysis**  
✅ **Upgrade effort estimation**  
✅ **Library support duration**  

By using this assessment, you can:  
- **Remediate issues** based on recommendations  
- **Improve software compliance**  
- **Mitigate risks** associated with outdated dependencies  

Try the **free Spring Application Health Assessment** today and explore how **Tanzu Spring Runtime** or the **Spring Consulting team** can support your transition.  

---

## 🚀 Running the Assessment  

### Prerequisites  
- **Java 8 or 11** (depending on the Spring Boot version used)  
- **Maven or Gradle** for dependency management  

### **Step 0: Setup the repo and run the spring app**  
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-org/spring-boot-legacy-demo.git
   cd spring-boot-legacy-demo
   mvn clean install
   mvn spring-boot:run


### **Step 1: Execute the SBOM Generation Script**  
Run the following command in your terminal:  
```bash
./run-mvn-assessment.sh
```

### **Step 2: Upload SBOM to Tanzu Platform**  
1. Go to [Tanzu Platform Assessment Center](https://www.platform.tanzu.broadcom.com/assessment-center/home/assessments)  
2. Click **"New Spring Health Assessment"**  
3. Click **"Next"**  
4. **Upload the SBOM file** generated from Step 1  
   - _Max supported file size: 10 MB_  
5. Click **"Upload"** and wait for the assessment to complete  

---

## 📊 Viewing the Assessment Results  

Upon completion, you will receive a **dashboard with key insights**, including:  

- **OSS Support Status:**  
  - ✅ **100% Unsupported** _(Your Spring version is no longer maintained)_  

- **Libraries with Vulnerabilities:**  
  - ⚠️ **60% of dependencies contain known vulnerabilities**  

- **Upgrade Effort:**  
  - 🔧 **100% High Upgrade Effort** _(Major refactoring required)_  

### 🌟 Additional Features in Tanzu Platform  
- **Analyze Git Repos at scale** for vulnerabilities and EOS  
- **Discover dependencies between Infra & Applications**  
- **Analyze Applications on Kubernetes & Tanzu Application Services**  