# 🌟 YorkU CSCL1030 Laboratory 3
## 🚀 Automating CI/CD Pipelines for Python API using Jenkins, Terraform, and Ansible
#### This assignment focuses on the implementation of Continuous Integration (CI) and Continuous Delivery (CD) pipelines for a Python API using Jenkins, Terraform, and Ansible. The main objective is to automate the process of building, testing, and deploying a Python-based application, integrating various tools and technologies to streamline deployment in an AWS environment.

## 📁 Project Structure:

### Jenkins Setup:
The project establishes a robust Jenkins environment using the JenkinsComplex repository. This environment includes:

✅ A Python node configured per class instructions.
❌ No Java node required, as the lab focuses exclusively on the Python API.

### 📈 CI/CD Pipelines:

### 🛠️ Continuous Integration Pipeline:
Automates building and testing of the Python API.

Includes steps for:
✅ Code linting with pylint.
🧪 Running unit tests.
📦 Building the Python application.

### 🚀 Continuous Delivery Pipeline:
Automates deployment using Ansible.
Provisions a Python application server.
Deploys the API and verifies its successful operation.

### 🌐 Infrastructure Provisioning:

#### ☁️ AWS EC2 Instances:
Terraform provisions AWS EC2 instances, including:
🖥️ Jenkins master.
🤖 Jenkins agents.
🗄️ MariaDB SQL database server.
🐍 Python application server.
🛡️ Includes MariaDB database as part of the backend for the Python API.
🌍 Public IPs for EC2 instances are listed for easy access.

#### 🖥️ Application Deployment:
Python application is deployed to an EC2 instance.
Deployment process is automated using Ansible.
✅ Verified using a curl command to ensure the API is operational.

### 🎯 Purpose:
This project demonstrates the power of CI/CD pipelines to:

🚀 Streamline application deployment.
🔄 Reduce manual intervention.
✅ Ensure continuous testing and deployment for the Python API.

### 📂 Repo Structure:

### 📂 JenkinsComplex:
Jenkins setup for Python-based CI/CD pipelines.
### 📂 ContinuousDelivery:
Defines the CI/CD pipeline structure and configurations.
### 📂 ProvisionAppServer:
Terraform and Ansible scripts for provisioning AWS resources and deploying the application.
### 🔗 Links and Outputs:
##### 🖥️ Terraform Output: Results from terraform apply for provisioning servers and resources.
##### 🌍 AWS EC2 List: Includes public IPs of provisioned instances.
##### 📜 Pipeline Console Outputs:
##### Integration job outputs (pylint results to the end).
##### Deployment job outputs.
##### 🔗 Curl Command Execution: Verifies the Python API is operational.
