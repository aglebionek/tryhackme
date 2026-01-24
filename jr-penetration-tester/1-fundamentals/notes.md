# Fundamentals


## Hattypes

<img src="../images/hattypes.png" alt="Hattypes" style="width: 500px;" />


## Rules of Engagement (RoE)

The ROE is a document that is created at the initial stages of a penetration testing engagement.

<img src="../images/roe.png" alt="Rules of Engagement" style="width: 500px;" />


## Stages

<img src="../images/stages.png" alt="Rules of Engagement" style="width: 500px;" />


## Methodologies - TODO
https://github.com/mtesauro/owasp-wte

## Whitebox, Greybox, Blackbox

<img src="../images/boxes.png" alt="Rules of Engagement" style="width: 500px;" />

- **Blackbox**: No prior knowledge of the target system. The tester approaches the system as an external attacker would, relying on publicly available information and reconnaissance techniques to identify vulnerabilities.

- **Greybox**: The tester has limited knowledge of the target system, such as network architecture or access credentials, but not full access. This approach simulates an insider threat or a partially informed attacker.

- **Whitebox**: The tester has complete knowledge of the target system, including access to source code, architecture diagrams, and configuration details. This approach allows for a thorough assessment of the system's security posture.




# Principles

## Confidentiality, Integrity, Availability (CIA Triad)

- **Confidentiality**: This element is the protection of data from unauthorized access and misuse. Organisations will always have some form of sensitive data stored on their systems. To provide confidentiality is to protect this data from parties that it is not intended for.

- **Integrity**:  This element is the condition where information is kept accurate and consistent unless authorized changes are made.

- **Availability**: In order for data to be useful, it must be available and accessible by the user. Availability is very often a key benchmark for an organisation. When a system is unavailable, it often results in damage to the organisation.




# Privileges

## Privileged Identity Management (PIM) - USER
Used to translate a user's role within an organisation into an access role on a system.

Example: An employee in the finance department may have access to financial records on a system, whereas an employee in the HR department may not have access to those same records. Roles would be: 
- ROLE_FINANCE - Access to financial records
- ROLE_HR - No access to financial records


## Privileged Access Management (PAM) - SYSTEM
The management of the privileges a system's access role has.

Example: The role ROLE_FINANCE has to have acces to financial records. We have to manage what level of access this role has. Does it have read-only access, or read and write access? This is where PAM comes into play. The ROLE_HR role has to be set to have none of these privileges of accessing financial records.

