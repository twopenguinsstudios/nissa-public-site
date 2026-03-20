# Nissa — Product Spec

## Product Philosophy

Nissa is not a CLM replacement. It's the contract intelligence layer that CLMs should have been but never built because they were too busy optimizing pre-signature workflow.

**Design principles:**
- Zero-friction ingestion (email forward, not file upload)
- Answers in real time, inside existing tools
- Post-signature intelligence as the core value loop
- No behavior change required for adoption
- Lightweight by design: live in days, not months

## Architecture

```
Contract arrives (email, Slack, Teams, shared drive)
    ↓
Nissa ingests and parses
    ↓
AI extracts: pricing, terms, clauses, renewals, SLAs
    ↓
Compares against historical contract database
    ↓
Returns: benchmarks, risk alerts, suggested actions
    ↓
Output delivered via email reply, Slack, or Teams
    ↓
Contract enters post-signature monitoring loop
```

## Core Features

### Contract Ingestion
- Email forward (nissa@yourdomain.com)
- Slack integration
- Microsoft Teams integration
- Google Drive / SharePoint / OneDrive sync
- No templates, no tagging, no metadata cleanup required

### AI Extraction
- Pricing and payment terms
- Renewal dates and auto-renewal clauses
- Termination windows and notice periods
- SLAs and performance obligations
- Liability and indemnification clauses
- Key contacts and signatories
- All surfaced in plain English

### Post-Signature Intelligence
- **Renewal tracking:** Automated alerts before renewal windows close
- **Pricing benchmarks:** Cross-vendor comparison across your contract portfolio
- **Obligation monitoring:** SLA tracking, deliverable deadlines, compliance requirements
- **Savings detection:** AI identifies renegotiation opportunities based on market data and historical terms
- **Risk alerts:** Auto-renewals, missing SLAs, unfavorable termination clauses flagged immediately

### Policy Enforcement
- Procurement rules applied at ingestion
- Compliant contracts auto-approved
- Exceptions flagged and escalated
- No manual review bottleneck for standard contracts

### Reporting & Exports
- Contract portfolio overview
- Vendor spend analysis
- Renewal calendar
- Risk exposure summary
- Available on Scale tier

## Pricing Tiers

### Monthly Billing

| Tier | Price | Active Contracts | Key Features |
|------|-------|-----------------|--------------|
| **Starter** | $556/mo | Up to 100 | Ingestion, AI extraction, renewal tracking, basic policy rules, email alerts |
| **Pro** | $1,333/mo | Up to 300 | + Full contract memory, clause recall, advanced policy, auto-approval, AI redlines, pricing normalization, renewal & savings agents |
| **Scale** | $2,667/mo | Up to 1,000 | + Cross-vendor benchmarking, multi-entity support, advanced reporting, centralized policy, priority onboarding, dedicated success manager |

### Annual Billing (25% savings)

| Tier | Price |
|------|-------|
| Starter | $5,000/yr |
| Pro | $12,000/yr |
| Scale | $24,000/yr |

## Integrations

### Live / Planned
- Email (Outlook, Gmail)
- Slack
- Microsoft Teams
- Google Drive
- SharePoint / OneDrive
- Dropbox
- Box

### Future
- Salesforce
- HubSpot
- QuickBooks / Xero
- DocuSign
- Ironclad (import/migration)

## Technical Considerations

- **Security:** Contract data segregated per customer, encrypted at rest and in transit
- **AI accuracy:** Nissa surfaces terms and context but does not make legal decisions. Procurement stays in control.
- **Data ownership:** Customers own their data. Full export available at any time.
- **Compliance:** SOC 2 and GDPR readiness on the roadmap

## What Nissa Is NOT

- Not a CLM replacement (it complements or replaces, depending on what you have)
- Not a legal review tool (it surfaces risk, doesn't provide legal advice)
- Not a workflow automation platform (intentionally lightweight)
- Not an e-signature tool (integrates with existing signing tools)

---

*Last updated: March 2026*
