# **$\color{blue}{\textsf{OneRecord — A Unified Semantic Data Model for Procurement}}$**

Enabling consistent, reusable data mapping between enterprise systems and exchange standards across the construction supply chain.

---

## **$\color{blue}{\textsf{The Problem}}$**

Construction procurement relies on multiple document types — catalogues, orders, despatch advices, invoices — each exchanged between different parties using different systems. Every company maps its ERP data to these standards independently, creating dozens of point-to-point integrations that are expensive, error-prone, and difficult to maintain.

The standards themselves (UBL/Peppol, EDIFACT) define document *structure*, but each implementation fills that structure with its own values and logic. Two companies mapping "buyer" from their ERP to a Peppol Order may use completely different field paths, naming conventions, and identifiers — even though they mean the same thing. There is no shared semantic reference that connects these mappings.

---

## **$\color{blue}{\textsf{The Idea}}$**

OneRecord is a single semantic data model that merges all procurement-related Peppol documents into one unified structure. Instead of treating each document as a separate mapping problem, OneRecord assigns every data element a **unique, human-readable example value** that carries the same meaning across all documents and systems.

> **Core principle:** One value = one meaning = reused everywhere. When a company populates its own ERP system document data with OneRecord data, AI-assisted comparing reveals exactly which ERP document data elements correspond to which standard document elements — automatically forming a mapping between ERP and standard.

---

## **$\color{blue}{\textsf{How It Works}}$**

- **Populate.** A company fills the OneRecord model with its own data, using unique example values as anchors.
- **Generate.** Standard documents (Order, Invoice, etc.) are produced from the same model with the same values.
- **Compare.** Matching values between ERP output and standard documents reveals the field-level mapping.
- **Reuse.** The resulting mapping works across tools, systems, and formats — including AI-assisted alignment.

Because the example values are human-readable, they are also machine-readable. This means mapping can be performed using simple Excel tools, graphical JSON editors, or AI-driven semantic matching — lowering the barrier for companies without deep integration expertise.

---

## **$\color{blue}{\textsf{What OneRecord Covers}}$**

| Area | Content | Status |
|------|---------|--------|
| Documents | Catalogue, Order, Order Response, Despatch Advice, Receiving Advice, Invoice | v0.9 |
| Parties | 14 roles including Buyer, Seller, Supplier, OEM, Carrier, Consignor/Consignee, Tax Representative | v0.9 |
| Items | Product hierarchy with sub-items, GTIN, serial/lot, dimensions, hazardous goods classification | v0.9 |
| Sustainability | Digital Product Passport (DPP) and Environmental Product Declaration (EPD) references | v0.9 |
| Mappings | ERP → OneRecord → UBL (SAP, Dynamics examples) and UBL → OneRecord → EDIFACT | v0.9 |
| Traceability | Serial numbers, lot numbers, GPS coordinates, party handoff chain | v0.9 |

---

## **$\color{blue}{\textsf{What OneRecord Is Not}}$**

OneRecord is not a new standard. It does not modify, extend, or replace Peppol BIS, UBL, EDIFACT, or any specification maintained by OpenPeppol, CEN, ISO, or UNECE. All documents generated using OneRecord remain fully BIS-compliant, with no additional mandatory elements or schema extensions. OneRecord is an **informative semantic reference layer** that sits alongside existing standards to improve consistency and reduce integration effort.

---

## **$\color{blue}{\textsf{Why This Matters for Construction}}$**

The construction industry operates across long supply chains with many specialised actors — architects, general contractors, element manufacturers, component suppliers, carriers. Each handoff (design to tendering, ordering to delivery, delivery to invoicing) involves data that originates in one system and must be understood by another.

OneRecord traces data from its origin through every reuse point. An element designed in Tekla, ordered through Peppol, shipped with a waybill, and invoiced months later can carry the same identifiers, sustainability references, and technical data throughout — without re-entry, without ambiguity.

---

## **$\color{blue}{\textsf{Getting Involved}}$**

OneRecord v0.9 is published as a reference implementation governed by the BETK working group in Finland. Participation is open. Joint development has been expanded to the BEAST working group in Sweden, and several academic research projects have joined the work.

Findings, tools, and results are available openly on GitHub. Companies can adopt OneRecord voluntarily to support their own interoperability, ERP mapping, and digitalisation initiatives. The model evolves through additive, consensus-based changes with no breaking modifications within a major version.

> **Target release:** OneRecord v1.0 is planned for Q2/2026.

---

## **$\color{blue}{\textsf{Contributors}}$**

**OneRecord v0.9**

**Lead:** Kari Korpela

**Contributors:** Hannu Kivinen, Henrik Vinell, Juuso Autiosalo, Jyrki Oraskari, Mikael af Hällström, Peter L. Borresen, Rikard Larsson, Teemu Alaluusua, Tom Partanen, Antti Taskinen
