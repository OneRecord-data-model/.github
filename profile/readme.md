# OneRecord v1.0 – GitHub Release Note

**Version:** OneRecord v1.0  
**Status:** Reference implementation  
**Release type:** Informative (non-normative)

---

## 1. Introduction

OneRecord v1.0 is published as a reference implementation of a single semantic data model intended to support consistent mapping between enterprise systems and existing data exchange standards, including UBL (Peppol BIS) and EDIFACT.

The purpose of OneRecord is to provide a shared semantic reference layer that can be used alongside existing standards to improve interoperability, consistency, and reusability of business data across processes and document types.

---

## 2. Scope and intent

OneRecord is designed to be used as:

- an informative reference model  
- a semantic alignment tool for mappings  
- a supporting artefact for interoperability and digitalisation initiatives  

OneRecord is **not a standard**, and it does **not modify or extend** any existing standards maintained by OpenPeppol, CEN, ISO, or UNECE.

---

## 3. Relationship to Peppol and standards

OneRecord operates outside the scope of Peppol governance and is intended to be fully compatible with Peppol BIS specifications.

Specifically:

- All Peppol documents generated using OneRecord remain fully BIS-compliant  
- No additional mandatory elements are introduced  
- No schema extensions are required  
- All documents validate independently  

OneRecord addresses semantic reuse and consistency, while Peppol BIS specifications continue to define document structure and rules.

---

## 4. Content of OneRecord v1.0

The v1.0 reference package includes:

### 4.1 Semantic reference lists

- Parties (e.g. Buyer, Seller, Supplier, Manufacturer)  
- Items and sub-items (product structures)  
- Business documents  
- Traceability identifiers (serial and lot)  
- Sustainability references (Digital Product Passport, Environmental Product Declaration)

### 4.2 Mapping references

- ERP → OneRecord → UBL  
- UBL → OneRecord → EDIFACT  

These mappings are illustrative and informative, demonstrating how a shared semantic layer can be used to reduce point-to-point mappings.

---

## 5. Intended use

OneRecord v1.0 may be used to:

- support interoperability projects  
- assist ERP and integration mappings  
- enable AI-assisted semantic alignment  
- serve as a reference in pilots, demonstrations, and research activities  

Use of OneRecord is voluntary and does not impose requirements on Peppol participants.

---

## 6. Governance and evolution

OneRecord v1.0 is governed as a neutral, vendor-independent reference model.

The following principles apply:

- No breaking changes within a major version  
- Additive evolution only  
- Stable identifiers are preserved  
- Changes are reviewed through a working group process  

Future versions may extend the reference content while maintaining backward compatibility.

---

## 7. Contributors

### Lead

- Kari Korpela

### Working group

- Hannu Kivinen  
- Henrik Vinell  
- Juuso Autiosalo  
- Jyrki Oraskari  
- Mikael af Hällström  
- Peter L. Borresen  
- Rikard Larsson  
- Teemu Alaluusua  
- Tom Partanen  
- Antti Taskinen  

---

## 8. Status of this document

This release note and the accompanying OneRecord v1.0 materials are provided for information purposes.

They do **not** constitute:

- a Peppol specification  
- a CEN or ISO standard  
- a conformance requirement  

---

## 9. Concluding statement

OneRecord v1.0 provides an informative semantic reference layer that can be used alongside existing standards to support consistent mappings between enterprise systems and data exchange formats, contributing to improved interoperability and digitalisation.
