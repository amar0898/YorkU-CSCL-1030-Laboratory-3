# YorkU CSCL1030 Laboratory 3

#### This assignment focuses on the implementation of Continuous Integration (CI) and Continuous Delivery (CD) pipelines for a Python API using Jenkins, Terraform, and Ansible. The main objective is to automate the process of building, testing, and deploying a Python-based application, integrating various tools and technologies to streamline deployment in an AWS environment.

## Project Structure:

### Jenkins Setup:

#### The project sets up a complex Jenkins environment using the JenkinsComplex repository. The environment includes a Python node configured according to the specifications in class instructions. The Java node is not required for this lab, as the focus is on the Python API.

### CI/CD Pipelines:

#### Continuous Integration Pipeline: 
Built using the guidelines from class 9, this pipeline automates the process of building and testing the Python API. It includes stages like code linting with pylint, running unit tests, and building the Python application.
#### Continuous Delivery Pipeline: 
This pipeline automates the deployment process using Ansible. It provisions a Python application server, deploys the API, and ensures that it is running successfully.

### Infrastructure Provisioning:

#### AWS EC2 Instances: Terraform is used to create and configure AWS EC2 instances, including the Jenkins master, Jenkins agents, a MariaDB SQL database server, and a Python application server. The project also includes a MariaDB database instance, which is part of the backend for the Python API. The EC2 instances are listed, showing their public IPs for easy access.

#### Application Deployment: The Python application is deployed to an EC2 instance, and Ansible is used to automate the process. After deployment, the API is tested by executing a curl command to verify its successful operation.

### Purpose: This project demonstrates the use of CI/CD pipelines to streamline application deployment, reduce manual intervention, and ensure the Python API is continuously tested and deployed in an efficient and automated manner.

### Repo Structure:

### JenkinsComplex: Jenkins setup for Python-based CI/CD pipelines.
### ContinuousDelivery: Defines the CI/CD pipeline structure and configurations.
### ProvisionAppServer: Terraform and Ansible scripts for provisioning AWS resources and deploying the application.
### Links and Outputs:
#### Output from terraform apply for provisioning servers and resources.
#### AWS EC2 list with public IPs of the provisioned instances.
#### Pipeline console outputs for integration and deployment jobs.
#### Curl command executed on the Python app server to verify the API's operation.
#### By the end of this lab, you will have a fully automated CI/CD pipeline in place, making your Python application deployment process efficient and scalable.
