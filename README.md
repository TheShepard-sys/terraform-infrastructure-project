# Terraform Infrastructure Project

## Overview

Provisioned an AWS EC2 instance using Terraform with variables and outputs.
The instance is configured automatically to run a Docker container (Nginx).

---

## Features

* Infrastructure as Code (Terraform)
* Modular configuration using variables
* Output values (Public IP, Instance ID)
* Automated setup using user_data
* AWS Free Tier compliant

---

## Tech Stack

* Terraform
* AWS (EC2)
* Amazon Linux 2023
* Docker
* Nginx

---

## Project Structure

```
terraform-infrastructure-project/
├── main.tf
├── variables.tf
├── outputs.tf
├── screenshots/
└── README.md
```

---

## Usage

### Initialise

```
terraform init
```

### Plan

```
terraform plan
```

### Apply

```
terraform apply
```

### Destroy (Important)

```
terraform destroy
```

---

## Screenshots

* Project structure
* variables.tf
* main.tf
* outputs.tf
* terraform init
* terraform plan
* terraform apply
* outputs
* EC2 running
* nginx page
* terraform destroy

---

## Security Notes

* `.terraform/` and state files excluded via `.gitignore`
* No credentials stored in repository
* IAM user used (not root)

---

## Notes

* Uses `t3.micro` (Free Tier)
* Region: eu-west-2
* Security group allows HTTP (port 80) for demo access
