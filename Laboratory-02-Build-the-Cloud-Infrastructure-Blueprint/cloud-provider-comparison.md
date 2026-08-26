# Cloud Provider Comparison: AWS vs. Microsoft Azure vs. Google Cloud Platform

## Service Comparison Table

| Infrastructure Component | Amazon Web Services (AWS) | Microsoft Azure | Google Cloud Platform (GCP) |
|--------------------------|---------------------------|-----------------|----------------------------|
| **Compute** | Amazon EC2 [citation:1][citation:11][citation:13] | Azure Virtual Machines [citation:1][citation:4][citation:11] | Google Compute Engine [citation:1][citation:11][citation:15] |
| **Compute (Containers)** | Amazon EKS [citation:1] | Azure Kubernetes Service (AKS) [citation:1][citation:4] | Google Kubernetes Engine (GKE) [citation:1][citation:15] |
| **Compute (Serverless)** | AWS Lambda [citation:1][citation:11] | Azure Functions [citation:1][citation:11] | Cloud Functions [citation:1][citation:11] |
| **Storage (Object)** | Amazon S3 [citation:1][citation:11][citation:13] | Azure Blob Storage [citation:1][citation:9][citation:11] | Cloud Storage [citation:1][citation:11][citation:15] |
| **Storage (Block)** | Amazon EBS [citation:1][citation:3] | Azure Managed Disks [citation:1] | Persistent Disk [citation:1][citation:15] |
| **Storage (File)** | Amazon EFS [citation:3] | Azure Files [citation:1] | Filestore [citation:15] |
| **Networking** | Amazon VPC [citation:1][citation:11][citation:13] | Virtual Network (VNet) [citation:1][citation:9][citation:11] | VPC Network [citation:1][citation:11][citation:15] |
| **Identity & Access Management (IAM)** | AWS IAM [citation:1][citation:3][citation:8] | Microsoft Entra ID (formerly Azure AD) [citation:1][citation:9][citation:11] | Cloud IAM [citation:1][citation:11][citation:15] |

---

## Guide Questions

### 1. Which cloud provider offers the broadest range of services? Explain your answer.

AWS offers the broadest range of services among the three major cloud providers. As the first major cloud provider, AWS has had the longest time to develop its service portfolio and has the most mature ecosystem of third-party integrations and community resources [citation:3].

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

Microsoft Azure is the best recommendation for organizations that primarily use Microsoft products. Azure provides seamless integration with Microsoft's ecosystem, including Microsoft 365, Active Directory, and development tools like Visual Studio [citation:4][citation:9]. Azure's Microsoft Entra ID allows organizations to unify on-premises and cloud identity management, simplifying hybrid environments.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

Google Cloud Platform (GCP) is widely recognized for its strength in AI, ML, and Kubernetes services. GCP's Vertex AI provides a unified platform for the entire ML workflow, and Google's background in AI research gives it a competitive advantage [citation:1][citation:11]. Google Kubernetes Engine (GKE) is considered one of the most mature Kubernetes services, building on Google's experience with container orchestration [citation:11].

### 4. What similarities did you observe among the three cloud providers?

All three cloud providers offer the same core categories of services—compute, storage, networking, and identity management—under different names [citation:6]. The fundamental concepts are identical across platforms: virtual machines (EC2 = VMs = Compute Engine), object storage (S3 = Blob Storage = Cloud Storage), and serverless computing (Lambda = Functions = Cloud Functions). This similarity allows cloud engineers to transfer their skills between providers, learning only new terminology rather than entirely new concepts [citation:6].
