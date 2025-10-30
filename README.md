# 05proj-vpc-public-private-subnets

Certainly! Here's your VPC project description rewritten in clear, professional, and updated English:

---

### 🌐 VPC: Public and Private Subnet Project

**Objective:**  
To build a custom Virtual Private Cloud (VPC) on AWS with both public and private subnets. This setup demonstrates secure network segmentation between internet-facing components and internal backend systems.

**Architecture Reference:**  
See attached diagram: `architecture-diagram.png`

**Key Components:**
- **Custom VPC:** `10.0.0.0/16`
- **Public Subnet:** `10.0.1.0/24` (connected to an Internet Gateway)
- **Private Subnet:** `10.0.2.0/24` (no Internet Gateway)
- **Public EC2 Instance:** Accessible via SSH and ping from the internet
- **Private EC2 Instance:** Accessible only through SSH from the public EC2 instance

**Testing Steps:**
1. Use your key pair to SSH into the public EC2 instance.
2. From the public EC2, SSH into the private EC2 using its private IP address.

**Security Configuration:**
- Security Groups are configured to allow SSH access **only from your IP address**.

---

Let me know if you'd like this formatted for documentation, presentation, or deployment notes.
