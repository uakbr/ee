| Gap Area | Identified Gap | Justification and Implications |
|----------|----------------|-------------------------------|
| 1. Governance for cloud security configurations and processes | Lack of automated drift detection and remediation | Current manual processes may lead to undetected security misconfigurations. Automated drift detection is planned but not implemented, risking potential security vulnerabilities in the interim. |
| | Incomplete integration of account request process | Account requests are managed in Nimbus without ServiceNow integration, potentially leading to inconsistent approval processes and lack of centralized tracking. |
| | Azure environment not fully aligned with security best practices | Ongoing modernization efforts indicate current Azure setup may not meet all security requirements, potentially exposing resources to unnecessary risks. |
| | Absence of regular canary testing | Lack of periodic testing may result in undetected failures in event flows and alerting mechanisms, potentially delaying incident response. |
| | Insufficient controls for root account access | Current access controls for the root account workflow mailbox may not be robust enough, risking unauthorized access to critical cloud resources. |
| 2. Cloud account creation and configuration management | Large number of unmanaged legacy accounts | 53 out of 66 production accounts not managed by Nimbus, potentially leading to inconsistent security practices and increased risk of misconfigurations. |
| | Lack of automated compliance logging for account creation | Current processes don't leverage Splunk for automated logging of account creation, hindering ability to demonstrate consistent compliance over time. |
| | Incomplete service certification process | While a certification process exists, its completeness and currency are unclear, potentially allowing use of services that don't meet all security requirements. |
| | Underutilization of AWS Config for compliance tracking | AWS Config not currently used to track and demonstrate compliance with AMI management policies, limiting automated oversight of configuration states. |
| | Unclear Azure tenant creation and management process | Lack of documented, standardized process for Azure tenant creation may lead to inconsistencies in security configurations across tenants. |
| 3. Server machine image creation, hardening and launching | Inconsistent AMI lifecycle management | Potential gaps in AMI versioning, deployment, and retirement processes may result in use of outdated or vulnerable images. |
| | Presence of systems running on unsupported OS versions | Some systems still use unsupported operating systems, significantly increasing security risks due to lack of security updates. |
| | Manual AMI compliance tracking processes | Reliance on manual processes for tracking AMI lifecycle and compliance increases risk of human error and oversight. |
| | Unclear Azure image management process | Lack of clear understanding of Azure image management, particularly regarding on-premises VM handoffs, may lead to security gaps in the image lifecycle. |
| | Limited visibility into non-VM application security | Focus on VM security may overlook security settings and upgrade processes for non-VM services like AWS App Service and Azure SQL Database. |
| 4. Security event logging and monitoring | Fragmented logging and alerting systems | Use of multiple tools (Cribble, Splunk) for logging and alerting may lead to inefficiencies and potential gaps in security event coverage. |
| | Incomplete VPC Flow Logs management | Current plans to move VPC flow logs suggest they're not optimally managed, potentially limiting network traffic visibility and analysis capabilities. |
| | Disparity in logging and alerting capabilities between AWS and Azure | Azure environment may lack parity with AWS in logging and alerting capabilities, creating inconsistent security monitoring across cloud platforms. |
| | Over-reliance on manual alert verification | Cloud Ops team manually verifies Splunk alerts, increasing response time and risk of human error in threat detection. |
| | Reactive security team involvement | Security team's reactive involvement in monitoring may delay identification and response to potential security incidents. |
| | Potential gaps in logging continuity | Lack of mechanisms to detect and alert on logging disruptions may result in undetected security events during periods of logging failure. |
