## Project Description

This lab was created to gain hands-on experience with Security Information and Event Management (SIEM) using Wazuh. A Windows 11 endpoint was connected to the Wazuh server through the Wazuh agent, allowing security events to be collected and analyzed in real time.

The objective was to generate common Windows security events and observe how they are detected and logged within the Wazuh dashboard. Each alert was reviewed to understand its significance from a SOC analyst perspective.

## Activities Performed

### Failed Login Attempt (Event ID 4625)

Generated multiple failed login attempts using incorrect credentials. Wazuh successfully detected the authentication failures and generated alerts for investigation.

### Successful Login (Event ID 4624)

Performed a successful login using valid credentials. The event was recorded and correlated within the Wazuh dashboard.

### Account Lockout (Event ID 4740)

Triggered multiple failed login attempts until the target account was automatically locked by Windows security policy.

### User Account Creation (Event ID 4720)

Created a new local user account and verified that Wazuh detected the account creation event.

### User Added to Administrators Group (Event ID 4732)

Added a user account to the local Administrators group to generate a privilege-related security event.

### Service Configuration Change (Event ID 7040)

Modified the startup configuration of the Background Intelligent Transfer Service (BITS) and verified alert generation.

### System Restart Event (Event ID 1074)

Performed a system restart and confirmed that the event was captured within Windows logs and displayed in Wazuh.

## Security Analysis

The generated events represent common activities that SOC analysts investigate during daily monitoring operations. Authentication failures, account lockouts, account creation, privilege modifications, and service changes can indicate malicious activity when performed without authorization. Wazuh provided centralized visibility into these actions through Windows Event Log monitoring.

## Key Learnings

* Deployment and configuration of Wazuh SIEM
* Windows Event Log monitoring
* Security alert investigation
* User account activity monitoring
* Privilege change detection
* Service modification monitoring
* Basic SOC analyst workflow
* Security event documentation

## Conclusion

The lab successfully demonstrated Wazuh's capability to collect, process, and analyze Windows security events. Through practical alert generation and investigation, valuable experience was gained in security monitoring and incident analysis using a SIEM platform.
