# GDPR Data Processor Agreement - Requirements & Clauses

## Overview

A Data Processor Agreement (DPA) is required by GDPR Article 28(3) whenever a data controller engages a data processor to handle personal data. This reference document outlines the mandatory clauses and recommended best practices.

## Article 28 - Mandatory Requirements

### 28(1) - Controller Responsibility
Controller must use processors providing sufficient guarantees for technical and organizational measures ensuring security and confidentiality.

### 28(3) - Contractual Requirements
Processing must be governed by contract or another legal act binding the processor to the controller. The contract MUST specify:

1. **Subject matter and duration** of processing
2. **Nature and purpose of processing**
3. **Types of personal data** and categories of data subjects
4. **Data controller** (name and contact)
5. **Data processor obligations and rights**

## Standard Four-Part Structure

All DPAs should include these sections:

### Part 1: Title & Parties
- Full legal names of both parties
- CVR/Tax ID numbers
- Business addresses
- Contact persons and email addresses
- Execution date
- Service or system name being processed

### Part 2: Preamble
Establish legal context:
- "For the purposes of Article 28(3) of Regulation (EU) 2016/679..."
- Brief description of the relationship
- Acknowledgment of the processor's obligations
- Reference to standard contractual clauses (if using EU standard terms)

### Part 3: Core Clauses (Articles 1-14)

#### Article 1: Definitions
Define key terms:
- "Personal Data": Any information relating to an identified or identifiable natural person
- "Processing": Collection, recording, organization, alteration, retrieval, use, disclosure, etc.
- "Data Subject": The person to whom personal data relates
- "Special Category Data": Data revealing racial/ethnic origin, political opinions, religious beliefs, trade union membership, genetic data, biometric data, health data, sex life data

#### Article 2: Subject Matter
- Specify the exact data being processed
- List purposes of processing
- Duration of processing
- Categories of data subjects (e.g., customers, employees, patients)

#### Article 3: Instructions
Controller must provide written instructions for ALL processing. Processor must not process beyond these instructions except when required by law.

#### Article 4: Processor Obligations
Processor must:
- Process data only on documented instructions from controller
- Ensure confidentiality of persons processing data
- NOT disclose data to unauthorized third parties
- Implement appropriate technical/organizational security measures
- NOT process in countries without adequate protection (unless controller explicitly approves)
- Assist controller in fulfilling data subject rights requests
- Delete or return data after service termination

#### Article 5: Sub-processor Rules  
Controller must approve before processor engages sub-processors. Processor must:
- Inform controller of any sub-processor changes 30 days in advance
- Allow controller to object to new sub-processors
- Impose same data protection obligations on sub-processors via contract

#### Article 6: Data Subject Rights Assistance
Processor must assist controller in fulfilling data subject requests for:
- Access to their data
- Corrections or deletions
- Restrictions on processing
- Data portability
- Objections to processing

#### Article 7: Security Measures
Processor must implement and maintain:
- **Encryption**: For data in transit and at rest
- **Pseudonymization**: Where feasible
- **Access controls**: Role-based access, authentication
- **Audit trails**: Logging of access and changes
- **Incident response**: Procedures for data breaches
- **Backup and recovery**: Ability to restore data
- **Personnel training**: Security awareness for staff

#### Article 8: Assistance with Data Protection Impact Assessments (DPIA)
Processor must assist controller in:
- Assessing risks to data subjects
- Designing privacy-protective measures
- Documenting the DPIA process
- Consulting with supervisory authorities if needed

#### Article 9: Data Breach Notification
Processor must:
- Notify controller WITHOUT UNDUE DELAY (typically within 24-48 hours) of any personal data breach
- Provide details of: what happened, affected data subjects, likely consequences, remedial actions taken
- Assist controller in meeting notification deadlines to authorities

#### Article 10: Term and Termination
- Processing continues until written termination notice
- Upon termination, processor must (per controller's choice):
  - Return all personal data
  - Delete all personal data (including backups)
  - Prove deletion/return with evidence
- Consequences of breach or non-compliance may include contract termination

#### Article 11: Audit and Compliance
Processor must:
- Make available all information needed to demonstrate compliance
- Allow controller to conduct audits and inspections
- Undergo annual or periodic third-party audits (SOC 2, ISO 27001)
- Provide audit reports to controller on request

#### Article 12: Transfer of Data Outside EU/EEA
If processor transfers data outside the EU/EEA:
- ONLY with explicit controller approval
- Subject to adequacy decisions OR binding corporate rules OR standard contractual clauses (SCCs)
- Processor remains liable for third-party processors' compliance
- Controller must be informed of all transfer mechanisms

#### Article 13: Deletion or Return Upon Termination
Processor must delete all personal data upon contract end UNLESS legal obligations require retention.

#### Article 14: Liability and Indemnification
Processor is liable to controller for damages caused by breach of GDPR obligations.

Processor shall indemnify controller against third-party claims if breach is processor's fault.

#### Article 15: Governing Law and Jurisdiction
- Specify applicable law (typically where controller is established)
- Specify dispute resolution mechanism (jurisdiction or arbitration)
- Effective date and term of agreement

### Part 4: Appendices

#### Appendix A: Details of Processing
Table format with:
| Item | Detail |
|------|--------|
| **Data Categories** | Names, email addresses, phone numbers, location data, etc. |
| **Special Categories** | Any health data, biometric data, genetic data, etc. |
| **Purposes** | Service delivery, billing, analytics, etc. |
| **Data Subjects** | Customers, employees, patients, website users, etc. |
| **Retention Period** | How long data is kept (e.g., during contract + 30 days) |
| **Recipient Categories** | Internal staff, sub-processors, auditors, etc. |
| **Countries** | Where processing occurs (data residency) |
| **Technical Measures** | Encryption, access controls, logging, etc. |
| **Organizational Measures** | Staff training, policies, incident response, etc. |

#### Appendix B: Data Controller's Instructions
Document ALL instructions:
- What data can be processed
- For what purposes
- To whom it can be disclosed
- How long it can be retained
- What security measures must be applied
- How to handle data subject requests
- Procedures for sub-processors
- Breach notification procedures

#### Appendix C: Technical and Organizational Measures (TOMs)
Detailed security specifications:
- **Confidentiality**: Encryption (AES-256 or equivalent)
- **Integrity**: Hash verification, HMAC, digital signatures
- **Availability**: Redundancy, backups, disaster recovery
- **Resilience**: System monitoring, incident response
- **Recovery**: RTO/RPO targets, backup testing frequency
- **Restoration**: Ability to recover data within specified timeframe
- **Strength**: Aligned with NIST, ISO 27001, or industry standards

#### Appendix D: Additional Provisions
- **Notification procedures**: How to notify of breaches, changes, issues
- **Personnel**: Names/roles of data protection contacts
- **Liability caps** (if any): Typical limit is annual fees paid
- **Confidentiality period**: Often extends 2-5 years after termination
- **Dispute resolution**: Escalation procedures before litigation
- **Term**: Duration of agreement and renewal terms
- **Fees**: What processor is paid (may reference separate commercial agreement)

## Health Data Special Considerations

When the agreement involves health data (Article 9 GDPR), enhance with:

1. **Enhanced security requirements**: Encryption mandatory
2. **Stricter access controls**: Only healthcare staff with legitimate need
3. **Audit logs**: Immutable records of all access for 3+ years
4. **Data Subject Consent**: Explicit consent often required (not just legitimate interests)
5. **Data Protection Officer (DPO)**: Usually required for health data processing
6. **DPIA Required**: Data Protection Impact Assessment mandatory
7. **International compliance**: Alignment with HIPAA (if US involvement), eHealth standards

## Country-Specific Clauses

See [references/country-specifics.md](references/country-specifics.md) for Denmark, Norway, and Germany specific modifications.

## Standard Contractual Clauses (SCCs)

If data transfers outside EU to countries without adequacy decisions, include:

- **Module One** (Controller to Processor)
- **Module Two** (Processor to Processor)  
- **Module Three** (Controller to Third Party)
- **Module Four** (Processor to Sub-processor)

Select the appropriate module based on the transfer pattern.

## Document Best Practices

1. **Clear language**: Use simple, clear language despite legal nature
2. **Completeness**: Ensure ALL mandatory Articles 28(3) elements are included
3. **Signatures**: Both parties sign and date the agreement
4. **Copies**: Each party retains original signed copy
5. **Electronic signature**: Can use qualified electronic signature (eIDAS) where permitted
6. **Accessibility**: Use clear formatting, headings, readable font
7. **Updates**: Review annually and update when processing changes
8. **Record keeping**: Maintain signed agreements for audit purposes
