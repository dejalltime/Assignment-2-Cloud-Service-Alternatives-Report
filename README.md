
# Cloud Security & Compliance Service Comparison

## Objective
This report compares key Microsoft Azure services used in our course with equivalent offerings in Amazon Web Services (AWS) and Google Cloud Platform (GCP). The goal is to understand similarities and differences in features, security/compliance, pricing, and DevSecOps integration.

---

## 1. Azure Active Directory (SSO, IAM)

| Feature               | Azure Active Directory | AWS Equivalent: AWS IAM + AWS SSO | GCP Equivalent: Google Identity Platform |
|-----------------------|------------------------|------------------------------------|-------------------------------------------|
| **Overview**          | Cloud-based identity and access management service for SSO, MFA, and conditional access. | Manages AWS accounts, roles, and permissions; AWS SSO handles single sign-on. | Provides identity services, SSO, MFA, and integration with Google Workspace. |
| **Core Features**     | SSO, MFA, Conditional Access, B2B/B2C identity, Role-based access control. | IAM roles, policies, federated access; AWS SSO for multi-app sign-on. | OAuth 2.0, OpenID Connect, MFA, Cloud Identity for RBAC. |
| **Security & Compliance** | ISO 27001, SOC 1/2, FedRAMP, HIPAA, GDPR. | ISO 27001, SOC, FedRAMP, HIPAA, GDPR. | ISO 27001, SOC 1/2/3, FedRAMP, HIPAA, GDPR. |
| **Pricing Model**     | Free tier, premium per-user/month pricing. | Free for IAM; AWS SSO free but charges for directory integration. | Free tier, premium per-user pricing for Cloud Identity Premium. |
| **DevSecOps Integration** | Integrates with Azure DevOps, GitHub, APIs for automation. | Supports AWS CLI, SDK, and CI/CD pipelines. | Integrates with Google Cloud Build, APIs, and CI/CD tools. |

---

## 2. Azure Monitor & Log Analytics

| Feature               | Azure Monitor & Log Analytics | AWS Equivalent: Amazon CloudWatch | GCP Equivalent: Google Cloud Operations Suite |
|-----------------------|--------------------------------|------------------------------------|-----------------------------------------------|
| **Overview**          | Monitors applications and infrastructure, collects telemetry data. | Observes resources and apps, collects metrics and logs. | Provides logging, monitoring, and error reporting for apps and services. |
| **Core Features**     | Metrics, logs, alerts, Kusto query language (KQL), visualization. | Metrics, logs, alarms, dashboards. | Metrics Explorer, logging, alerts, tracing. |
| **Security & Compliance** | ISO 27001, SOC, GDPR, HIPAA. | ISO 27001, SOC, GDPR, HIPAA. | ISO 27001, SOC, GDPR, HIPAA. |
| **Pricing Model**     | Pay-as-you-go for data ingestion and retention. | Pay per metric and log storage/ingestion. | Pay per metric and log storage/ingestion. |
| **DevSecOps Integration** | Integrates with CI/CD pipelines for monitoring. | CloudWatch Agent for CI/CD monitoring. | Integrates with Cloud Build, Cloud Functions for automated alerts. |

---

## 3. Azure Policy

| Feature               | Azure Policy | AWS Equivalent: AWS Organizations + Service Control Policies | GCP Equivalent: Organization Policy Service |
|-----------------------|--------------|---------------------------------------------------------------|----------------------------------------------|
| **Overview**          | Defines and enforces resource compliance at scale. | Manages organization-wide policies and permissions. | Enforces constraints on resources at the org/folder/project level. |
| **Core Features**     | Policy definition, assignment, compliance dashboard, remediation tasks. | SCPs, tag policies, account management. | Constraints, policy hierarchy, enforcement. |
| **Security & Compliance** | Ensures governance, aligns with ISO/GDPR/HIPAA/FedRAMP. | Governance and compliance frameworks supported. | Supports compliance requirements through enforced constraints. |
| **Pricing Model**     | Included in Azure subscription. | Included with AWS Organizations. | Included in GCP. |
| **DevSecOps Integration** | Policy-as-Code with CI/CD enforcement. | Terraform, AWS CLI, CDK integration. | Deployment Manager, Terraform, API integration. |

---

## 4. Microsoft Defender for Cloud

| Feature               | Defender for Cloud | AWS Equivalent: AWS Security Hub | GCP Equivalent: Security Command Center |
|-----------------------|--------------------|-----------------------------------|------------------------------------------|
| **Overview**          | Cloud security posture management and threat protection. | Centralized security and compliance dashboard. | Provides asset inventory, vulnerability scanning, threat detection. |
| **Core Features**     | CSPM, workload protection, regulatory compliance, threat detection. | Aggregates findings, compliance checks, integrations. | Threat detection, vulnerability scanning, policy enforcement. |
| **Security & Compliance** | ISO 27001, SOC, FedRAMP, GDPR, HIPAA. | Same as above. | Same as above. |
| **Pricing Model**     | Free tier for basic CSPM, pay-per-resource for advanced features. | Free for basic; charges for integrated services. | Free tier, premium pricing for advanced threat detection. |
| **DevSecOps Integration** | REST API, integrations with Azure DevOps, GitHub Actions. | API, CLI, AWS Lambda integration. | API, Terraform, CI/CD tools. |

---

## 5. Azure Sentinel (SIEM/SOAR)

| Feature               | Azure Sentinel | AWS Equivalent: Amazon Security Lake + Partner SIEM | GCP Equivalent: Chronicle Security Operations |
|-----------------------|----------------|------------------------------------------------------|-----------------------------------------------|
| **Overview**          | Cloud-native SIEM/SOAR with AI-based analytics. | Centralized security log storage, query, and partner SIEM integration. | Threat hunting, investigation, and response platform. |
| **Core Features**     | Data connectors, KQL queries, playbooks, incident response automation. | Centralized logs, Athena queries, integration with third-party SIEMs. | Incident detection, threat intelligence, SOAR capabilities. |
| **Security & Compliance** | FedRAMP, ISO, SOC, GDPR, HIPAA. | Compliance depends on integrated services. | FedRAMP, ISO, SOC, GDPR, HIPAA. |
| **Pricing Model**     | Pay-as-you-go for ingested data. | Pay for log ingestion and storage. | Pay for data ingestion and retention. |
| **DevSecOps Integration** | Automation rules, API, integration with CI/CD security checks. | Supports integration with AWS Security Hub, Lambda. | API, automation scripts, SIEM connectors. |

---

## Summary Table

| Azure Service | AWS Equivalent | GCP Equivalent |
|---------------|---------------|----------------|
| Azure Active Directory | AWS IAM + SSO | Google Identity Platform |
| Azure Monitor & Log Analytics | Amazon CloudWatch | Cloud Operations Suite |
| Azure Policy | AWS Organizations + SCPs | Organization Policy Service |
| Defender for Cloud | AWS Security Hub | Security Command Center |
| Azure Sentinel | AWS Security Lake + Partner SIEM | Chronicle Security Operations |

---

## Conclusion
While Azure, AWS, and GCP offer similar core functionalities, their pricing models, integration options, and native tooling vary. Azure excels in tight integration with Microsoft products and Policy-as-Code, AWS provides mature IAM and security aggregation tools, and GCP offers strong data analytics capabilities within security tooling. Understanding these differences is crucial for effective multi-cloud DevSecOps strategies.

