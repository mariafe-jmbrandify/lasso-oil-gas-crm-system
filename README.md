# Lasso Oil & Gas — CRM System

A purpose-built CRM for mineral rights acquisition: tracking deals, mailer campaigns, assets, and documents in one place, with an AI layer for drafting, extraction, due-diligence flagging, and reporting.

## Why this exists

Lasso Oil & Gas LLC acquires mineral rights through mailer campaigns and direct owner outreach. That work was previously spread across multiple spreadsheet tabs — a live deals tracker, a separate closed-deals tracker, mailer lists, campaign schedules, invoices — each maintained by hand, with no single source of truth and no way to see the whole pipeline at once. This repo documents and hosts the CRM built to replace that: one place for Deals, Mailer Lists, Campaigns, Assets, and Documents, with AI assistance layered on top of — not instead of — human review.

## Repo structure

```
lasso-oil-gas-crm-system/
├── README.md                    ← you are here
├── LICENSE
├── CHANGELOG.md
│
├── docs/                        ← how the system works, end to end
│   ├── PROJECT_OVERVIEW.md      ← what this is and who it's for
│   ├── PRODUCT_ARCHITECTURE.md  ← modules, user flows, UI structure
│   ├── SYSTEM_ARCHITECTURE.md   ← technical architecture, stack, data flow
│   ├── DATABASE_SCHEMA.md       ← record structure for every module
│   └── BUSINESS_WORKFLOWS.md    ← the real-world processes the system supports
│
└── modules/                     ← one doc per CRM module
    ├── Dashboard.md
    ├── Deals.md
    ├── Mailers.md
    ├── Campaigns.md
    ├── Assets.md
    ├── Documents.md
    ├── Due-Diligence.md
    ├── Title-Review.md
    ├── Curative.md
    ├── Closing.md
    ├── Payments.md
    ├── Reports.md
    ├── Tasks.md
    └── AI/                      ← the AI layer, documented separately
        ├── README.md
        └── ... (12 more files — see modules/AI/README.md for the index)
```

## Status

The MVP (Deals, Mailer Lists, Campaigns, Assets, Documents) is built and in active use, seeded with live data from the existing spreadsheet trackers. Everything else in this repo — due diligence automation, title review, curative tracking, closing, payments, and the AI layer — is documented as the target architecture and is being built incrementally.

## Getting started

This repo is documentation-first: read `docs/PROJECT_OVERVIEW.md` for the "what and why," then `docs/SYSTEM_ARCHITECTURE.md` for the "how." Each file in `modules/` documents one screen/capability in enough detail to build or review it independently.

## Ownership

Built and maintained by Maria Fe Blanca (JM Brandify) for Lasso Oil & Gas LLC.
