# Health Data Detection & Special Category Data Rules

## Overview

Special Category Personal Data (Article 9 GDPR) receives heightened protection because it poses particular risks to individuals. Health data is a primary category requiring enhanced safeguards. This reference guides automated detection and compliance flagging.

## What Constitutes "Health Data"?

Health data includes information that:

### Direct Health Indicators
- Medical diagnoses or medical history
- Treatment plans or therapies
- Medication names or prescriptions
- Hospital or clinic records
- Medical test results or lab reports
- Mental health assessments or therapy notes
- Disability status (physical, mental, cognitive, intellectual)
- Chronic condition information
- Vaccination records
- Drug or alcohol dependency information
- Genetic or DNA information
- Biometric data used for medical purposes

### Indirect/Secondary Health Indicators
- Health insurance claims or coverage information
- Workers' compensation records
- Fitness tracking data (if linked to health monitoring)
- Lifestyle data used for insurance underwriting
- Employment records related to sick leave or disability accommodations
- Educational records noting medical accommodations
- Travel records indicating medical appointments or treatments

### Not Necessarily "Health Data" (but often restricted)
- General fitness data (step count, exercise records) - only health data if used for health monitoring
- Age/date of birth alone - not health data unless combined with health info
- Insurance type without claims history - depends on context
- Workplace arrangements for disabilities - only health data if revealing disability

---

## Automated Detection Keywords & Patterns

When scanning provided data descriptions, flag as HEALTH DATA if containing:

### Medical/Clinical Terms
- medical, doctor, physician, nurse, clinic, hospital, treatment
- diagnosis, diagnose, patient, prescription, medication, drug
- therapy, therapeutic, counseling, mental health, psychiatry, psychologist
- physiotherapy, physical therapy, rehabilitation, recovery
- surgery, surgical, operation, procedure
- symptom, condition, illness, disease, disorder, syndrome
- vaccine, vaccination, immunization, inoculation
- genetic, DNA, genome, biometric (fingerprint, facial recognition for health)
- disability, disabled, impairment, handicap, accommodation

### Health Service Providers
- hospital, clinic, medical center, health center, practice
- pharmacy, dentist, orthodontist, optometrist, chiropractor
- mental health provider, therapist, counselor, psychiatrist
- nursing home, assisted living, rehabilitation center
- urgent care, emergency room, ER, A&E

### Health Insurance & Benefits
- health insurance, medical insurance, disability insurance
- workers' compensation, workmen's comp, workers' comp
- health plan, medical plan, benefit plan
- insurance claim, coverage, premium, deductible
- health savings account, HSA, FSA, medical savings

### Health-Related Data Categories
- medical history, patient records, clinical records
- health records, EHR, EMR (electronic health/medical records)
- health status, health condition, health information
- medical treatment, medical services, healthcare services
- health data, protected health information, PHI

### Regulatory/Compliance Terms (indicating health data context)
- HIPAA, GDPR Article 9, PII, protected health information
- health information privacy, medical privacy
- CCPA health exemptions, health data regulations
- FDA-regulated, healthcare compliance
- patient consent, medical consent

---

## Detection Scenarios

### Scenario 1: E-commerce Platform
**Provided data**: Names, email, address, purchase history, browsing behavior, payment info

**Health data detected?** NO - unless purchases reveal health products (medications, medical devices)

**ACTION**: Standard DPA applies

---

### Scenario 2: Fitness App
**Provided data**: Heart rate, step count, exercise duration, sleep patterns, calorie burn

**Health data detected?** MAYBE - depends on use
- If used only for fitness tracking: NOT health data
- If used for health monitoring or wellness insights: HEALTH DATA
- If shared with insurance company: HEALTH DATA

**ACTION**: Clarify intended use, apply health data safeguards if monitoring/insurance context

---

### Scenario 3: Employee Time Tracking
**Provided data**: Employee names, departments, hours worked, sick leave dates, location tracking

**Health data detected?** POTENTIALLY - sick leave information could reveal health status

**ACTION**: Alert that sick leave data may need health data handling if employee can specify date ranges or patterns revealing health conditions

---

### Scenario 4: Healthcare Provider Processing
**Provided data**: Patient names, medical diagnoses, treatment codes (ICD-10), medication lists, test results, provider notes

**Health data detected?** YES - CLEAR AND COMPREHENSIVE

**ACTION**: MANDATORY health data safeguards:
- Explicit consent required (not legitimate interest)
- DPIA mandatory
- Data Protection Officer required
- Enhanced encryption (AES-256)
- Strict access controls (role-based, healthcare staff only)
- Audit logging mandatory (3+ years)
- Data handling policy mandatory
- Sub-processors carefully vetted

---

### Scenario 5: HR Platform
**Provided data**: Employee names, salary, performance reviews, attendance records, emergency contacts

**Health data detected?** USUALLY NO - unless:
- Performance reviews mention health-related absences
- Records track medical leave patterns
- Emergency contact info includes relationship to healthcare provider

**ACTION**: Standard DPA unless clarified that health-related leave tracking occurs

---

### Scenario 6: Customer Database
**Provided data**: Customer names, contact info, order history, health & fitness products (vitamins, fitness equipment)

**Health data detected?** NO - purchase history alone is not health data

**ACTION**: Standard DPA. However, if combined with health assessments or recommendations: HEALTH DATA

---

## Enhanced Safeguards When Health Data Detected

### Technical Safeguards (TOMs)

1. **Encryption**
   - Data at rest: AES-256 or equivalent
   - Data in transit: TLS 1.2+ (minimum), TLS 1.3+ (recommended)
   - Healthcare data in backups: Encrypted separately

2. **Access Control**
   - Role-based access (RBAC)
   - Principle of least privilege
   - Multi-factor authentication (MFA) mandatory
   - Active directory or equivalent identity management
   - Quarterly access reviews

3. **Audit & Monitoring**
   - Immutable audit logs for all access
   - Log retention: minimum 3 years (often 6-7)
   - Log monitoring for suspicious patterns
   - Real-time alerts for unauthorized access attempts
   - Monthly audit review

4. **Data Isolation**
   - Separate database or schema for health data
   - Network segmentation if possible
   - Separate backup storage
   - Restricted API access

### Organizational Safeguards

1. **Policies & Procedures**
   - Written data handling policy
   - Privacy by design documentation
   - Data breach response plan (mandatory notification < 72 hours)
   - Data retention & deletion schedule

2. **Personnel**
   - Healthcare privacy training (annual minimum)
   - Background checks for staff accessing health data
   - Confidentiality agreements (sign-on, sign-off)
   - Designated data protection officer (often required)

3. **Compliance & Oversight**
   - Annual or biennial audit (internal or third-party)
   - SOC 2 Type II certification (recommended)
   - ISO 27001 certification (recommended for larger processors)
   - Regular vulnerability assessments
   - Incident response plan testing (quarterly)

4. **Documentation**
   - Data Protection Impact Assessment (DPIA) - mandatory
   - Record of Processing Activities (ROPA)
   - Sub-processor assessment documentation
   - Security incident documentation

---

## Consent & Legal Basis for Health Data

### General Data (Articles 6)
Legal bases: Consent, contract, legal obligation, vital interests, public task, legitimate interests

### Health Data (Articles 9)
Processing generally PROHIBITED except when:

1. **Explicit Consent** - Data subject freely gives specific, informed, unambiguous consent
   - Cannot be conditioned on service access (except healthcare services)
   - Must be clear, easy to withdraw
   
2. **Vital Interests** - Processing necessary to protect life or serious interests

3. **Employment/Social Law** - Processing necessary for employment or social security obligations (limited scope)

4. **Public Interest** - By healthcare provider, health insurance, social protection (member state law governs)

5. **Healthcare Services** - By healthcare professional for diagnosis, treatment, care

6. **Legitimate Activity** - By not-for-profit organization with sufficient safeguards

7. **Legal Claims** - Necessary for legal claims or courts

8. **Manifestation in Public Domain** - Data made public by data subject

**Most common**: **Explicit Consent** or **Healthcare Services** basis

---

## Red Flags & Compliance Warnings

Alert users if DPA involves:

⚠️ **Health data without explicit consent mechanism** - Add consent process
⚠️ **Third-party sub-processors with health data** - Requires explicit approval
⚠️ **International transfer of health data** - Ensure adequacy decision or SCCs
⚠️ **Health data + vague purposes** - Specify precise health purposes
⚠️ **Health data + consumer profiling** - Ensure not used for automated decisions
⚠️ **No DPIA when health data present** - MANDATORY, must be documented
⚠️ **No Data Protection Officer** - Often required for systematic monitoring of health data
⚠️ **Insufficient encryption/access controls** - Upgrade to health data standards

---

## Documentation Requirements When Health Data Involved

All agreements with health data MUST document:

- [x] Type of health data being processed (categories)
- [x] Legal basis for processing (usually explicit consent)
- [x] Data Subject consent mechanism (if required)
- [x] Purposes and legitimate limitations
- [x] Recipients and sub-processors (individually approved)
- [x] Retention period and deletion procedures
- [x] Data Subject rights procedures (access, deletion, objection)
- [x] International transfer mechanisms
- [x] Technical measures (encryption standards, access controls)
- [x] Organizational measures (personnel, training, incident response)
- [x] Data Protection Impact Assessment summary
- [x] Data Protection Officer contact (if applicable)
- [x] Processor's liability and insurance coverage
