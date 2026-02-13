---
name: gdpr-data-processor-agreement
description: "Generate GDPR-compliant data processor agreements (DPA) in Word document format. Triggers include: creating data processor agreements, generating DPA documents, ensuring GDPR compliance for data processing contracts, drafting data processing agreements. Use when you need to produce a legally-binding data processor agreement that: (1) Meets EU GDPR Article 28(3) requirements and standard contractual clauses, (2) Can be customized for specific countries (Denmark, Norway, Germany, EU), (3) Automatically detects and flags health data and special category data requiring stricter safeguards, (4) Produces professionally formatted .docx documents ready for use. NOT for general drafting advice, legal consultation, or non-GDPR contexts."
license: Creative Commons Attribution 4.0 International (CC BY 4.0)
---

# GDPR Data Processor Agreement Generator

Generate legally-compliant data processor agreements (DPA) that meet EU GDPR requirements, with built-in support for special category data detection and country-specific regulations.

## Quick Start

When you provide:
- **Processor details**: Name, CVR/Tax ID, address
- **Controller details**: Name, CVR/Tax ID, address  
- **Processing description**: What data is being processed, why, and where
- **Data types**: Categories of data (names, emails, health records, etc.)
- **Country**: EU default, or select Norway/Germany for specific adjustments
- **Service name**: Name of the service or system for processing

The skill will:
1. **Detect health data**: Automatically identify if provided data includes health/medical/special category data
2. **Flag stricter requirements**: Alert when additional HIPAA-like safeguards apply
3. **Generate DPA**: Create a complete, professionally formatted Word document
4. **Include all required sections**: Preamble, definitions, controller/processor obligations, appendices
5. **Apply country rules**: Adjust clauses if Norway or Germany selected

## Document Structure

The generated agreement includes:

- **Title page** with parties, CVR numbers, and execution date
- **Preamble** explaining the legal basis and purpose
- **Article 1-14**: Standard contractual clauses covering:
  - Rights and obligations of controller and processor
  - Scope of processing and sub-processor rules
  - Data subject rights and security obligations
  - International data transfers (if applicable)
- **Four Appendices**:
  - **Appendix A**: Details of processing (data categories, purposes, recipients)
  - **Appendix B**: Data controller's conditions and instructions
  - **Appendix C**: Technical and organizational measures (security)
  - **Appendix D**: Additional provisions (notification, liability, termination)

## Health Data Detection

The generator automatically scans provided data categories for indicators of health data or special category personal data, which includes:

- Medical records, diagnoses, treatments, prescriptions
- Mental health or psychological assessments
- Genetic data or DNA information
- Biometric data (fingerprints, facial recognition)
- Health insurance information
- Medication and pharmaceutical data
- Disability or accessibility information

When health data is detected, the agreement is flagged with enhanced security requirements aligned with international standards (HIPAA-like safeguards).

## Country-Specific Adjustments

### Denmark (Standard EU-compliant version)
No additional changes needed. The template is designed by Datatilsynet (Danish Data Protection Authority).

### Norway
Modifications include:
- Reference to Norwegian Personal Data Act (Personopplysningsloven)
- Compliance with Datatilsynet (Norwegian Data Protection Authority)
- Norwegian binding corporate rules acknowledgment
- Adjustments for Norwegian data residency preferences

### Germany
Modifications include:
- Reference to BDSG (Bundesdatenschutzgesetz - German Data Protection Act)
- Compliance with state Data Protection Commissioners (Landesbeauftragte)
- German standard contractual clauses adaptation
- TISAX certification support (if high-security processing)

## Output

The generated agreement is delivered as a `.docx` file ready to:
- Print and execute
- Further customize if needed
- Export to PDF
- Integrate with document signing platforms

---

## How to Use This Skill

When you request a data processor agreement, provide the following information:

```
Controller: [Company name, CVR, Address]
Processor: [Company name, CVR, Address]  
Service: [Name of service/system]
Data types: [List categories: names, emails, health records, etc.]
Storage location: [Country/region]
Country regulation: [Denmark/Norway/Germany/EU]
Additional notes: [Any special requirements]
```

The skill will validate the input and generate a complete DPA document.

For detailed guidance on sections and legal requirements, see:
- **GDPR clause templates**: [references/gdpr-requirements.md](references/gdpr-requirements.md)
- **Health data identification rules**: [references/health-data-detection.md](references/health-data-detection.md)
- **Country-specific provisions**: [references/country-specifics.md](references/country-specifics.md)

The Python generation script can be customized for additional requirements.
