Issue Summary:
- Duration: The outage occurred from 10:00 AM to 11:30 AM on May 10, 2024 (EAT).
- Impact: The outage affected the user authentication service, resulting in users being unable to log in to their accounts. Approximately 30% of users attempting to access the service experienced login failures or delays.
- Root Cause: The root cause of the outage was identified as a misconfiguration in the load balancer settings, leading to an overload on the authentication service.

Timeline:
- 10:00 AM: The issue was detected when monitoring alerts indicated a significant increase in failed login attempts.
- 10:05 AM: Engineers investigated the issue and suspected a potential issue with the authentication service or its dependencies.
- 10:15 AM: Initial investigation focused on the authentication service and database servers to identify any performance bottlenecks or service disruptions.
- 10:30 AM: Misleading investigation paths were explored, including network connectivity issues and database replication delays, but no significant findings were identified.
- 10:45 AM: The incident was escalated to the infrastructure team for further investigation and resolution.
- 11:00 AM: After thorough analysis, the misconfiguration in the load balancer settings was identified as the root cause of the issue.
- 11:15 AM: The misconfiguration was corrected, and load balancing parameters were adjusted to ensure optimal distribution of incoming traffic.
- 11:30 AM: The authentication service was restored to normal operation, and users were able to log in without any further issues.

Root Cause and Resolution:
- Root Cause: The misconfiguration in the load balancer settings caused an imbalance in incoming traffic, leading to an overload on the authentication service and subsequent login failures.
- Resolution: The misconfiguration was corrected by adjusting the load balancer settings to evenly distribute incoming traffic across multiple backend servers. Additionally, monitoring and alerting mechanisms were enhanced to detect similar issues proactively in the future.

Corrective and Preventative Measures:
- Improvements/Fixes: 
  - Review and update load balancer configurations regularly to prevent misconfigurations.
  - Implement automated testing of load balancer settings to detect potential issues before deployment.
  - Enhance monitoring and alerting systems to provide real-time visibility into service performance and detect anomalies promptly.
- Tasks to Address the Issue:
  - Conduct a comprehensive review of load balancer configurations to identify and correct any other potential misconfigurations.
  - Implement automated deployment pipelines for load balancer configurations to ensure consistency and reduce the risk of human error.
  - Enhance documentation and training for infrastructure teams to improve awareness of best practices and troubleshooting procedures related to load balancer management.
  
