# Country-Specific DPA Modifications

## Overview

While GDPR Article 28 provides the core requirements, individual European countries have supplementary national laws and data protection authority guidance. This document outlines modifications when operating in specific jurisdictions.

---

## Denmark (Standard EU GDPR)

### Classification
Denmark is the EU baseline. The Datatilsynet template is designed by the Danish Data Protection Authority and is GDPR-compliant.

### Key Points
- **Authority**: Datatilsynet (Danish Data Protection Authority)
- **National Law**: Implementation of GDPR via national Danish legislation
- **Special**: No major deviations; use standard EU requirements
- **Template Origin**: Official Datatilsynet template

### Modifications
None required. The template is already Denmark-optimized.

### Contact
Datatilsynet: https://www.datatilsynet.dk
Email: dt@dt.dk

---

## Norway

### Classification
Norway is NOT an EU member but is part of the EEA (European Economic Area). Norway applies GDPR-equivalent regulations through the EEA agreement and national law.

### Key Legislation
1. **Norwegian Personal Data Act** (Personopplysningsloven - LOV 2018-06-15 nr 38)
   - Implements GDPR into Norwegian law
   - Article 28 equivalency: Chapter 2, Section 2.7
   - Effective June 20, 2018 (simultaneous with GDPR)

2. **Data Protection Authority**: Datatilsynet (Norwegian Data Protection Authority)
   - Equivalent to Swedish IMY, Dutch AP, etc.
   - Issues guidance documents and templates

3. **Norwegian Data Processing Agreement Standard**
   - Datatilsynet publishes official template: "Mal for databehandleravtale"
   - Template is similar to Danish/Swedish versions with Norwegian-specific language

### Modifications for Norwegian Contracts

#### 1. Reference Norwegian Law
Update preamble from:
> "For the purposes of Article 28(3) of Regulation (EU) 2016/679 (the GDPR)..."

To:
> "For the purposes of Section 2.7, Chapter 2 of the Norwegian Personal Data Act (Personopplysningsloven - LOV 2018-06-15 nr 38) and in accordance with Regulation (EU) 2016/679 (the GDPR)..."

#### 2. Reference Norwegian Authority
Add reference to Datatilsynet:
> The parties acknowledge that processing is subject to oversight by Datatilsynet (Norwegian Data Protection Authority: www.datatilsynet.no).

#### 3. Norwegian Registered Address
If either party is Norwegian-registered:
- Use Norwegian CVR equivalent: Organisasjonsnummer (organization number)
- Often 9-digit format vs. Danish 8-digit CVR

#### 4. Notification Requirements
Nordic countries (including Norway) prefer WITHIN 24-48 HOURS for breach notification:

Standard clause:
> "Processor shall notify Controller without undue delay and, in any case, not later than 72 hours after becoming aware of a Personal Data Breach."

Norwegian preference:
> "Processor shall notify Controller IMMEDIATELY and, in any case, not later than 48 hours after becoming aware of a Personal Data Breach, enabling Controller to meet its legal obligations."

#### 5. Sub-processor Notification
Norway (via Datatilsynet guidance) prefers specific modification:

Standard clause:
> "Processor shall inform Controller of any changes concerning the addition or replacement of Sub-processors, thereby giving Controller the opportunity to object to such changes."

Norwegian recommended:
> "Processor shall inform Controller with at least 30 days' notice before engaging, replacing, or modifying any Sub-processor arrangements. Controller may object on grounds of significant concern relating to GDPR compliance. In the event of justified objection, Controller may terminate the contract without penalty."

#### 6. Data Residency
Norway is preferred location for Norwegian data. Add:

Appendix A annotation:
> "Personal data relating to Norwegian data subjects shall be processed and stored primarily within Norwegian territory or, if not possible, within the EEA. Any transfer outside the EEA requires explicit prior written approval."

#### 7. Operator Changes
Add clause for Norwegian context:

> "The parties acknowledge that processing may involve sub-processors operating in other EEA countries. The Processor shall maintain a current list of Sub-processors at [URL], updated at least quarterly."

### Norwegian Authority Contact
**Datatilsynet (Norwegian Data Protection Authority)**
- Website: https://www.datatilsynet.no
- Email: postkasse@datatilsynet.no
- Phone: +47 22 39 69 00
- Address: Hausmanns gate 3, 0186 Oslo

### Standard Template Resource
Datatilsynet provides official templates: https://www.datatilsynet.no/en/about-datatilsynet/templates/

---

## Germany

### Classification
Germany is an EU member with additional national data protection laws that layer on top of GDPR. Germany has 16 state-level Data Protection Commissioners in addition to federal oversight.

### Key Legislation
1. **GDPR** - Directly applicable (Articles 1-99)

2. **BDSG** (Bundesdatenschutzgesetz - Federal Data Protection Act)
   - Current version: BDSG 2018 (amended 2021)
   - Implements GDPR into German law
   - Adds additional requirements for processing in Germany
   - Article 28 equivalency: Section 7, BDSG

3. **State-Level Laws** (Datenschutzgesetze der Länder)
   - 16 state variations (Baden-Württemberg, Bavaria, Berlin, etc.)
   - Primarily for public sector processing
   - Less relevant for private sector DPAs

4. **Regulatory Authority**
   - Federal: BfDI (Bundesbeauftragter für Datenschutz und Informationsfreiheit)
   - States: Landesbeauftragte für Datenschutz (State Commissioners)

5. **Standard Template**
   - Working group of German DPs publishes official template
   - More detailed than GDPR baseline
   - Often 50+ pages

### Modifications for German Contracts

#### 1. Reference German Law
Update preamble:

> "For the purposes of Section 7 of the Federal Data Protection Act (Bundesdatenschutzgesetz - BDSG) and Articles 28(3) and 28(4) of Regulation (EU) 2016/679 (the GDPR)..."

#### 2. Reference German Authority
Add clause:

> "Processing shall comply with requirements of the Federal Data Protection Commissioner (BfDI - Bundesbeauftragter für Datenschutz und Informationsfreiheit) and applicable State Commissioners (Landesbeauftragte für Datenschutz). Contact details: https://www.bfdi.bund.de"

#### 3. German Registered Details
If either party German-registered:
- Use German UStID (VAT ID) or HRB number instead of/in addition to CVR
- Format: DE[9-digit number]
- Example: DE123456789

#### 4. TISAX Requirement (If Applicable)
For high-security sensitive data processing in Germany, may require:

> "The Processor shall, upon request by Controller, provide evidence of TISAX certification or equivalent third-party audit (SOC 2 Type II or ISO 27001:2013/2022) confirming compliance with German security standards for critical infrastructure or sensitive industrial/commercial data."

#### 5. Data Processing Agreement Formality
German law requires more formal DPA structure. Ensure:

- **Written form**: Must be signed, not just email acceptance (German courts strict on this)
- **Explicit signatures**: Both parties' authorized representatives must sign with full legal names and titles
- **Date and Place**: Contract must show execution date and location (e.g., "Executed in Berlin on [date]")
- **Notarization**: Optional but common for high-value processing (€100k+ annual value)

#### 6. Instructions Documentation
BDSG Section 7(1) requires particularly detailed instructions. Add clause:

> "The Controller shall provide to Processor a detailed written specification of all processing instructions (Verarbeitungsanweisung) including: (a) data categories; (b) purposes; (c) data subject categories; (d) permitted recipients; (e) retention periods; (f) security requirements (Appendix C); (g) sub-processor list (Appendix D). Any material changes require Controller's prior written approval."

#### 7. Data Subject Access Rights
German law emphasizes data subject rights. Add:

> "Processor shall, within 15 calendar days (shorter than GDPR's usual timeframe) of receipt of a data subject's access request, provide Controller with all relevant personal data and processing details to enable Controller to respond within GDPR's 30-day deadline."

#### 8. Sub-processor Management
German authorities are strict on sub-processor oversight. Modify as:

> "Processor shall provide Controller with a current list of all Sub-processors at [URL]. Controller must be informed of Sub-processor changes at least 45 days in advance (longer than GDPR's 30-day standard, reflecting German authority preference). Controller may object to any Sub-processor on reasonable grounds related to data protection or technical competence. In case of rejection, Controller may terminate the contract without penalty. If no objection is raised within 45 days, approval is assumed."

#### 9. Breach Notification
German authorities expect FASTER notification. Modify:

> "Processor shall notify Controller IMMEDIATELY upon discovery of any Personal Data Breach and, in any case, within 24 hours of discovery, providing: (a) date/time of breach; (b) data categories and subjects affected; (c) likely impact; (d) remedial actions taken. This satisfies Controller's obligation to notify BfDI within 72 hours."

#### 10. Data Processing Location
Germany has significant data residency preferences, especially for government and sensitive sectors. Add:

> "Processing shall be conducted in [Specify: Germany, EU, or other with explicit approval]. Any Processing outside the Processor's primary location requires Controller's detailed approval and DPIA confirmation."

#### 11. Audit Rights
German law emphasizes auditor access. Add explicit clause:

> "Controller reserves the right to audit Processor's compliance at least annually. Processor shall provide access to systems, staff, documentation, and audit reports. Processor shall engage an independent auditor (Big Four or equivalent) to conduct ISO 27001 or SOC 2 Type II audit annually, with results provided to Controller within 30 days of completion."

#### 12. Liability
German law may impose higher liability standards. Add:

> "Processor shall indemnify and hold harmless Controller from any claims, damages, or regulatory fines arising from Processor's breach of this Agreement. Processor's liability is uncapped for breaches involving unauthorized disclosure or failures to implement mandatory security measures."

#### 13. Termination Rights
German authorities emphasize clear exit strategies:

> "Either party may terminate this Agreement for material breach with 30 days' notice if breach is not cured within 15 days of notification. Upon termination: (a) Processor shall return or destroy all personal data within 5 business days; (b) provide certification of destruction to Controller; (c) maintain no copies except as required by law; (d) delete all backups within 30 days."

### German Authority Contacts

**Federal Level:**
- **BfDI** (Federal Data Protection Commissioner)
- Website: https://www.bfdi.bund.de
- Address: Husarenstraße 30, 53117 Bonn
- Phone: +49 228 77007-0

**Key State Commissioners (Examples):**
- **Bavaria** (Bayern): BayLDA - https://www.datenschutz-bayern.de
- **Baden-Württemberg**: LfDI BW - https://www.baden-wuerttemberg.datenschutz.de
- **Berlin**: Berliner BfDI - https://www.datenschutz-berlin.de
- **North Rhine-Westphalia** (NRW): LDI NRW - https://www.ldi.nrw.de

**Find all 16 state commissioners**: https://www.ldi.nrw.de/links/landesdatenschutzbeauftragte.html

### Standard Template Resources
- **Working Group Model Contract**: Published by conference of German DPAs
- **BfDI Guidance**: https://www.bfdi.bund.de/DE/Datenschutz/Grundlagen/Auftragsverarbeitung/auftragsverarbeitung.html

---

## Comparison Table

| Feature | Denmark | Norway | Germany |
|---------|---------|--------|---------|
| **Primary Law** | GDPR | GDPR + Norwegian PA | GDPR + BDSG |
| **Authority** | Datatilsynet | Datatilsynet | BfDI + 16 states |
| **Sub-processor notice** | 30 days | 30 days | 45 days |
| **Breach notification** | 72 hours | 48 hours (rec'd) | 24 hours (rec'd) |
| **Data residency** | EU default | EEA preferred | Germany preferred |
| **Signature requirement** | E-signature OK | E-signature OK | Original/notarized preferred |
| **Audit frequency** | Annual (recommended) | Annual (recommended) | Annual (required) |
| **TISAX requirement** | No | No | Yes (if applicable) |
| **Liability cap** | Standard | Standard | Often uncapped |

---

## Implementation Workflow

When user specifies country:

1. **Denmark**: Use template as-is (no modifications)
2. **Norway**: Apply Norwegian PA references, shorten sub-processor notice to 30 days, add EEA residency preference
3. **Germany**: Apply BDSG references, extend sub-processor notice to 45 days, require annual audits, add TISAX if applicable

For multi-country processing, create separate DPA for each country with country-specific clauses, or create single master DPA with country-specific appendices.
