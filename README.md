# Awesome-Spend-Management-Procurement-Analytics

# Awesome Spend Management & Procurement Analytics

> A curated list of top Spend Management and Procurement Analytics platforms — both SaaS/Hosted commercial solutions and open-source alternatives for controlling business spend, automating procurement, and analyzing purchasing data.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Coupa](#coupa)
  - [Ramp](#ramp)
  - [Brex](#brex)
  - [Spendesk](#spendesk)
  - [Airbase by Paylocity](#airbase-by-paylocity)
  - [Pleo](#pleo)
  - [Payhawk](#payhawk)
  - [Teampay](#teampay)
  - [Procurify](#procurify)
- [Open-Source Software](#-open-source-software)
  - [Shillinq](#shillinq)
  - [aribacortex](#aribacortex)
  - [Ledgic](#ledgic)
  - [Odoo Purchase](#odoo-purchase)
  - [EzProcurements](#ezprocurements)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Spend Management and Procurement Analytics platforms. These are not open-source but are included as reference points for feature comparison.

### Coupa
**Type:** Comprehensive business spend management suite  
Coupa is a long-standing enterprise BSM platform covering procurement, invoicing, expense tracking, and supplier management. Reviewers note it is highly functional and flexible, handling the entire purchase lifecycle from sourcing to payment, though the interface can feel complex and less collaborative internally [citation:2]. Coupa is consistently positioned as the most expensive option in its class, but users often feel the depth justifies the cost [citation:2]. Its analytics are native to the suite, meaning they are powerful for data created inside Coupa but can miss spend in external systems [citation:1].  
**Best for:** Mid-to-large enterprises wanting a single, deeply integrated platform for end-to-end procurement and spend control.

### Ramp
**Type:** Finance automation with corporate cards and procurement  
Ramp combines corporate cards, expense management, accounts payable, and procurement into one platform, monetizing primarily through card interchange to offer free core spend management. Recent releases emphasize **real-time budget tracking** across T&E, AP, and POs, plus **AI purchasing agents** that handle sourcing, contract review, and renewal benchmarking [citation:3][citation:13]. It also added AI token spend management for teams consuming LLM APIs [citation:13].  
**Best for:** Startups and mid-market companies wanting modern, automated spend control with a free entry point and strong AI roadmap.

### Brex
**Type:** Global spend management with enterprise controls  
Brex provides corporate cards, expense management, and travel with a focus on **global and multi-entity operations**. It supports local cards in 60+ countries, automated VAT reclamation (via Fintua and VAT IT), and multi-entity ERP mapping for cleaner consolidation [citation:14]. Vendor management features let admins assign owners to vendor relationships and automate ERP vendor creation on export [citation:4]. Brex also integrates with procurement platforms like Coupa Pay for virtual card provisioning [citation:4].  
**Best for:** Enterprises and global companies needing multi-entity spend control, local currency cards, and automated tax recovery.

### Spendesk
**Type:** European spend management with AI data access  
Spendesk targets European finance teams with cards, expense claims, invoices, and budgets. Its **AI Connect** feature (via MCP) lets finance teams query spend data using AI assistants like Claude, without exporting to spreadsheets [citation:5]. The platform added French e-invoicing compliance (Plateforme Agréée) ahead of the September 2026 mandate, and **Smart Request Predictions** auto-fill cost centers and categories with 92% accuracy, reducing manual entry by 57% [citation:5].  
**Best for:** European SMBs and mid-market companies needing compliant, AI-assisted spend control with strong local integrations.

### Airbase by Paylocity
**Type:** Unified AP, procurement, and expense platform  
Airbase combines AP automation, guided procurement with purchase orders, corporate cards, and expense reimbursements on a single system with real-time GL sync [citation:6]. It was acquired by Paylocity in 2024 and now extends Paylocity's HCM suite into the office of the CFO [citation:6]. It offers a developer platform (REST API, webhooks, sandbox) for custom ERP/GL connections and exposes spend data across cards, bills, and reimbursements for reporting [citation:6].  
**Best for:** Mid-market companies wanting unified AP and procurement with strong API extensibility, particularly those in the Paylocity HCM ecosystem.

### Pleo
**Type:** European expense automation with subscription tracking  
Pleo focuses on automating expense capture, reviews, and reimbursements for European teams. It includes **Fetch** for collecting receipts from email, AI expense review against company guidelines, automated reimbursement schedules, and **subscription tracking** that generates an overview of recurring vendors and renewal reminders [citation:7]. Vendor cards apply default accounting values to recurring spend, reducing repetitive categorization [citation:7].  
**Best for:** European SMBs wanting to automate expense admin and gain visibility into SaaS/subscription spend without a heavy procurement suite.

### Payhawk
**Type:** Enterprise spend management with native SAP integration  
Payhawk targets complex, enterprise finance teams with a focus on ERP depth. Its Summer '26 release added **native SAP S/4HANA Public Cloud integration** for syncing expenses, payments, and master data, plus role-based field visibility for segregation of duties [citation:9]. It supports unified invoice capture (e-invoices, PDFs, supplier portals), global payments in 115+ currencies, and AI workflows (Financial Controller Agent in Teams) [citation:9].  
**Best for:** Enterprises running SAP or complex multi-entity operations needing deep ERP integration without sacrificing usability.

### Teampay
**Type:** Proactive spend management with real-time controls  
Teampay (by Paystand) emphasizes **proactive spend management** with pre-coded transactions, automated receipt matching, and real-time visibility into actuals, commitments, and budgets [citation:8]. It provides customizable reporting filtered by vendor, category, employee, or department, and integrates with accounting systems for automatic reconciliation [citation:8].  
**Best for:** CFOs and finance teams wanting granular, real-time control over employee and vendor spend with strong reporting.

### Procurify
**Type:** Procurement and spend control for mid-market  
Procurify provides purchase requisitions, approvals, purchase orders, and budget tracking with real-time visibility into committed spend [citation:10]. It supports configurable workflows, two- or three-way matching, and audit logs for compliance [citation:10]. Positioned as a mid-market suite that trades analytical depth for faster deployment and lower cost compared to enterprise BSM platforms [citation:1].  
**Best for:** Mid-market organizations needing structured purchasing workflows and budget control without enterprise complexity.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Spend Management and Procurement Analytics tools. The open-source ecosystem is **nascent** for full spend management, but several projects target procurement workflows, analytics, and AP automation.

### Shillinq
**Stack:** PHP / Nextcloud / OpenRegister | **License:** EUPL-1.2  
Shillinq is a complete open-source business administration suite for Nextcloud that includes **procurement management, supplier management, and contract lifecycle management** alongside bookkeeping and invoicing . It supports purchase orders, supplier approval chains, contract repositories with full-text search, and a **free plan for basic procurement management** . It is one of the few open-source projects explicitly covering the intersection of procurement and spend control in a self-hosted environment.  
**Best for:** Organizations already running Nextcloud wanting integrated procurement and supplier management without a separate SaaS subscription.

### aribacortex
**Stack:** Python | **License:** MIT  
aribacortex is an open-source Python library for **AI-powered SAP Ariba procurement intelligence and sourcing analytics** [citation:11]. It provides supplier scoring (cost, delivery, quality, risk, ESG, compliance), spend optimization by supplier or category, procurement risk detection (single-source exposure, compliance findings), and P2P workflow analytics (touchless rate, cycle time) [citation:11]. It is designed for SAP Ariba environments and can be embedded in CI/CD or analytics jobs. **Important:** This is an analytics library, not a full spend management platform—it analyzes data you provide.  
**Best for:** SAP Ariba teams and procurement analysts wanting open-source supplier scoring and spend analytics without a commercial suite.

### Ledgic
**Stack:** Next.js / FastAPI / Supabase / PostgreSQL | **License:** Open Source (per repository)  
Ledgic is an open-source **accounts-payable automation** platform with AI extraction, three-way matching, and tool-using agents [citation:19]. It enforces segregation of duties in SQL (AP managers approve up to $5,000, controllers above), maintains an append-only hash-chained audit log, and exposes an MCP server for AI agent access [citation:19]. While focused on AP rather than broad spend management, it provides the invoice-processing backbone that spend control depends on.  
**Best for:** Teams wanting self-hosted AP automation with strong security controls and AI-assisted invoice processing.

### Odoo Purchase
**Stack:** Python / PostgreSQL | **License:** LGPL-3.0 (Community)  
Odoo's Purchase module automates requisition-to-pay, controls invoicing, and manages vendor information within the broader Odoo ERP [citation:26]. It supports procurement propositions based on stock levels, purchase tenders with vendor comparison, vendor pricelist imports, and three-way matching for invoice control [citation:26]. The Community edition is free; Enterprise adds advanced features. It is part of a full ERP suite rather than a standalone spend management tool.  
**Best for:** Organizations already using or planning to adopt Odoo for ERP wanting integrated procurement within their existing system.

### EzProcurements
**Stack:** (Check repository) | **License:** Open Source  
EzProcurements is listed as a fast and free open-source e-Procurement solution suitable for companies from small businesses to global enterprises [citation:21]. (Search results were limited; verify current maintenance and feature coverage before adoption.)  
**Best for:** Teams wanting a lightweight, free e-procurement starting point, with careful evaluation of maintenance status.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Procurement | Spend Analytics | AP/Invoicing | Self-Hosted | Best For |
|----------|---------|-------|-------------|-----------------|--------------|-------------|----------|
| **Coupa** | Proprietary | Cloud | ✅ Deep | ✅ (Suite data) | ✅ | ❌ | Enterprise BSM |
| **Ramp** | Proprietary | Cloud | ✅ AI agents | ✅ Real-time budgets | ✅ | ❌ | Modern mid-market + AI |
| **Brex** | Proprietary | Cloud | (Vendor mgmt) | ✅ Global | ✅ | ❌ | Global multi-entity |
| **Spendesk** | Proprietary | Cloud | (Invoices) | ✅ AI Connect | ✅ | ❌ | European compliance |
| **Airbase** | Proprietary | Cloud | ✅ Guided POs | ✅ | ✅ | ❌ | Unified AP + procurement |
| **Payhawk** | Proprietary | Cloud | (Invoices) | ✅ SAP-native | ✅ | ❌ | SAP enterprises |
| **Procurify** | Proprietary | Cloud | ✅ POs + budgets | ✅ | (Matching) | ❌ | Mid-market procurement |
| **Shillinq** | EUPL-1.2 | PHP/Nextcloud | ✅ POs + suppliers | ✅ Contract spend | ✅ | ✅ | Nextcloud procurement |
| **aribacortex** | MIT | Python | (Ariba analytics) | ✅ Supplier scoring | ❌ | ✅ (Library) | Ariba spend analytics |
| **Ledgic** | Open Source | Next.js/FastAPI | (AP focus) | (Invoice) | ✅ 3-way match | ✅ | Self-hosted AP |
| **Odoo Purchase** | LGPL-3.0 | Python/Postgres | ✅ Requisition-to-pay | (ERP) | ✅ | ✅ | Odoo ERP procurement |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Spend Management or Procurement Analytics tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem for **full spend management** is very limited compared to commercial platforms. **Shillinq** is the most comprehensive open-source option for procurement and supplier management within a self-hosted suite . **aribacortex** fills a niche for SAP Ariba spend analytics [citation:11], while **Ledgic** provides AP automation with strong security controls [citation:19]. Commercial platforms like Coupa, Ramp, and Brex remain far more capable for real-time card controls, global payments, and AI-driven procurement automation.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
