# I'm currently looking for a New Adventure in DevOps

I'm a **Senior DevOps/Infrastructure Engineer** that is passionate about scalable systems, well-designed architecture, and product-driven development. 

My expertise:
- _Auto-scaling_, _auto-healing_, _rapidly scalable_, and _cost efficient_ **Ruby on Rails**, **Sidekiq**, **Java/SCORM** on **AWS Fargate** via **Cloudformation**
- _Auto-scaling_, _auto-failover_, **RDS Aurora MySQL** clusters using Rails Multi-database support
- Comprehensive **Datadog observability** using Ruby APM, Tracing, Profiling, Monitors, Synthetics, and Datadog logs integration to get full visibility
- Ensure infrastructure and deployment pipeline parity across **Commercial and GovCloud AWS regions** to support compliance, operational consistency, and streamlined cross-environment deployments
- Proactively manage the SDLC of our software stack and dependencies to **mitigate security vulnerabilities, avoid end-of-life risks**, and ensure long-term operational integrity
- Use **Copilot, OpenAI, Claude**, etc, wherever possible, to accelerate my development and workflow

My key principles:
- Keep it Simple
- Configure to rapidly scale when needed
- Pay only for what you actually need and use
- Low maintenance, limited yaml configuration necessary
- Practical DevSecOps in CI/CD (dependency versioning/management, SAST, DAST, periodic penetration tests)
- Focus on optimizing the feedback loop and speeding up the deployment pipelines
- Unblock development so that product enhancements get out faster and more reliably
  
I’m currently **open to new roles** where I can bring my expertise in infrastructure, DevOps, CI/CD automation, AWS architecture, and system reliability to help teams ship faster, scale smarter, and operate more securely.

On this page, you’ll find a few highlights of my work.  If you’re interested in what I can help build for your company — whether it’s simplifying infrastructure, improving reliability, or scaling operations — feel free to reach out.  I’d be happy to walk you through my work and discuss how I can contribute to your team’s goals.

[Connect with me](https://www.linkedin.com/in/damianfuentes/)
---

## 🛠️ Tech Stack
![Ruby on Rails](https://img.shields.io/badge/-Ruby%20on%20Rails-CC0000?style=flat-square&logo=ruby-on-rails&logoColor=white)
![Sidekiq](https://img.shields.io/badge/-Sidekiq-DD0031?style=flat-square&logo=ruby&logoColor=white)
![Fargate Powered](https://img.shields.io/badge/Powered_by-Fargate-blueviolet?logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Cloudformation](https://img.shields.io/badge/-Cloudformation-orange?style=flat-square&logo=amazon-aws&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-blue?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Datadog](https://img.shields.io/badge/-Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)
[![Concourse CI](https://img.shields.io/badge/Build-Concourse%20CI-0078D7?logo=azuredevops&logoColor=white)](https://concourse-ci.org/)

---
## 🏆 Key Accomplishments
- Designed and Maintained comprehensive **Concourse pipelines** automating full CI/CD for all services and infrastructure [📸](#concourse-pipelines)
- Built and simplified our core API and Frontend pipeline for automated container builds and deployments [📸](#container-build-and-deployment-pipeline)
- Migrated and upgraded from Percona 5.6 to Aurora MySQL 5.7 -> 8 and implemented Rails multi-database support [📸](#aurora-upgrades-and-scaling)
- Architected cost-effective and massively scalable **ECS Fargate** services across regions and clusters [📸](#fargate-infrastructure)
- Scaled **Sidekiq** to process millions of background jobs daily with zero downtime [📸](#sidekiq-dashboard)
- Provisioned and expanded our **Datadog observability** with **Datadog Dashboards, APM, Logs, Monitors, Synthetics, etc** [📸](#datadog-observability)

---

## 📸 Featured Work

### Concourse Pipelines
- Thank you [Concourse CI team](https://github.com/concourse/concourse)!
- Single page view of all CI/CD and Deployment pipelines
- Status (green=good, yellow/red=need to fix)
- Drill down to each task and related logs / Pause resources, tasks, pipelines
- Crazy stable, running for years, no issues
<a href="https://github.com/user-attachments/assets/76794d12-4a91-4088-b60e-e9d4e18f958a" target="_blank">
  <img src="https://github.com/user-attachments/assets/76794d12-4a91-4088-b60e-e9d4e18f958a" alt="Concourse Pipelines Screenshot" width="100%" />
</a>

---

### Container Build and Deployment Pipeline
- Comprehensive pipeline for Pull-request to Production deployment
- Simple OCI builds via Dockerfile and Buildkit, using [best practices](https://docs.docker.com/build/building/best-practices/)
- Automated linting, unit testing, and staging deployments
- Continuous regression testing against staging, and push button Production deployments
- Automated and Deterministic builds and build configurations
- TODO: Use [ECR remote cache when building](https://aws.amazon.com/blogs/containers/announcing-remote-cache-support-in-amazon-ecr-for-buildkit-clients/)
- TODO: Use [SOCI indices for container lazy loading](https://aws.amazon.com/about-aws/whats-new/2022/09/introducing-seekable-oci-lazy-loading-container-images/)
<a href="https://github.com/user-attachments/assets/66c78e25-c70c-4173-b2ae-278d82b4321a" target="_blank">
  <img src="https://github.com/user-attachments/assets/66c78e25-c70c-4173-b2ae-278d82b4321a" alt="Concourse API Pipeline Screenshot" width="100%" />
</a>

---

### Aurora Upgrades and Scaling
- Initially migrated from Percona 5.6 to Aurora MySQL 5.7 using manual replication
- Over time, continually upgraded Aurora MySQL and eventually to Aurora MySQL 8
<a href="https://github.com/user-attachments/assets/54e08084-226b-49b8-9934-e9f6ac7c731e" target="_blank">
  <img src="https://github.com/user-attachments/assets/54e08084-226b-49b8-9934-e9f6ac7c731e" alt="Aurora Database Console Screenshot" width="100%" />
</a>

#### Make use of Aurora replicas with Rails
- Thank you [Rails Team](https://github.com/rails/rails)!
- Use the Aurora Reader endpoint in [Rails multi-database support configuration](https://guides.rubyonrails.org/active_record_multiple_databases.html)
- This allowed us to scale down our resources since we're now using all databases
- Aurora instances can scale vertically to hundreds of vCPUs and horizontally to 15 readers
- Massive scalability while still only paying for what you use
<a href="https://github.com/user-attachments/assets/b163ef5a-c690-4de8-8a2a-20d80da443eb" target="_blank">
  <img src="https://github.com/user-attachments/assets/b163ef5a-c690-4de8-8a2a-20d80da443eb" alt="Aurora Metrics Screenshot" width="100%" />
</a>

---

### Fargate Infrastructure
- Cloudformation snippet of Task Definition with JSON logging and Datadog sidecars
- Uses TargetTrackingScaling to autoscale all services.  Easily enable predictive scaling for normal day to day patterns of scaling.
- Use AWS Secrets Manager for high level secrets
- Prefer encrypted credentials files for environment specific secrets
- Rails credentials [is a great example](https://guides.rubyonrails.org/security.html#custom-credentials)
<a href="https://github.com/user-attachments/assets/a9bcc8dd-0f49-42de-b917-f52e5ad5d4d0" target="_blank">
  <img src="https://github.com/user-attachments/assets/a9bcc8dd-0f49-42de-b917-f52e5ad5d4d0" alt="AWS Fargate Cloudformation Screenshot" width="100%" />
</a>

#### View and troubleshoot via e1s
- Thank you Xing Yahao for [e1s](https://github.com/keidarcy/e1s)!
- Crazy easy way to traverse multiple clusters, regions, services, tasks, and containers
- Shell into a container easily to investigate (Rails console is your friend)
<a href="https://github.com/user-attachments/assets/10d0e257-6ef6-4a0f-9722-9904df01f89e" target="_blank">
  <img src="https://github.com/user-attachments/assets/10d0e257-6ef6-4a0f-9722-9904df01f89e" alt="AWS Fargate e1s Screenshot" width="100%" />
</a>

---

### Sidekiq Dashboard
- Thank you [Sidekiq Team](https://github.com/sidekiq/sidekiq)!
- **Millions** of jobs a day
- **Billions** of jobs to date
- Autoscaling, auto-healing, Aurora Reader/Writer balanced jobs, makes use of all database resources using Rails Multi-database support
- No more unused standby databases
- Embedded cron jobs in Sidekiq configuration
<a href="https://github.com/user-attachments/assets/6c026dd8-2cb1-489a-a9ce-00cda6a351cc" target="_blank">
  <img src="https://github.com/user-attachments/assets/6c026dd8-2cb1-489a-a9ce-00cda6a351cc" alt="Sidekiq Dashboard Screenshot" width="100%" />
</a>

---

### Datadog Observability
- Single Dashboard view of entire Platform and critical metrics, events, logs, infrastructure costs, etc
- Drill down to each critical service, metric, log, trace, profile, and monitor with deep integration for full visibility
- Know exactly what's happening, when it happens, and the root cause, faster (MTTK)
<a href="https://github.com/user-attachments/assets/1457bec5-ba64-44a0-aef1-e870a18c1959" target="_blank">
  <img src="https://github.com/user-attachments/assets/1457bec5-ba64-44a0-aef1-e870a18c1959" alt="Datadog Dashboard Screenshot" width="100%" />
</a>

---

## ✍️ Latest Blog Posts (pending)
- [Build and deploy containers in Concourse Pipelines](./blog/concourse-containers.md)
- [Scaling Rails and Sidekiq with Multi-database support using Aurora databases](./blog/railsdb-scaling.md)
- [Simple Container Orchestration with CloudFormation and ECS Fargate](./blog/cloudformation-fargate.md)
- [Optimizing costs with AWS Fargate and Fargate SPOT](./blog/fargate-costs-scaling.md)
- [Datadog Observability for Fargate Containers](./blog/datadog-observability.md)


---

## 📈 Stats
![Profile Views](https://komarev.com/ghpvc/?username=dfuentes77&label=Profile%20views&color=0e75b6&style=flat)

---

> “Fast code wins features. Clear architecture wins teams.”
