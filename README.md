# company-ops

Central repository for all operations of an in-house software products company.

## Structure

```
company-ops/
├── immigration/              # Everything related to my F-1 / OPT status
│   ├── rebuttals/            # RFE/NOID responses, rebuttal letters, evidence
│   ├── opt-ead/              # I-765, approval notice, EAD card copies
│   ├── i20-sevis/            # I-20s, SEVP Portal reporting, DSO correspondence
│   ├── employment-evidence/  # Proof work relates to degree, 20+ hrs/week, unemployment-day log
│   ├── passport-visa-i94/    # Passport, F-1 visa, I-94 records
│   └── future-status/        # STEM OPT, H-1B, O-1 research and filings
├── company-req/              # Setup roadmap: registration, SEVP reporting, 2–3 yr plan
│   └── roadmap.md
├── bank-info/                # Accounts, statements, wire instructions, bank contacts
├── corporate-legal/
│   ├── formation/            # Articles of organization/incorporation, state filings
│   ├── ein-tax-ids/          # EIN letter (CP 575), state tax IDs
│   ├── operating-agreement/  # Operating agreement / bylaws and amendments
│   ├── annual-filings/       # Annual reports, registered agent, BOI filings
│   ├── ip-trademarks/        # Software IP assignments, trademarks, domain names
│   └── resolutions-minutes/  # Member/board resolutions, meeting minutes
├── expenses/
│   ├── software-subscriptions/  # SaaS tools, dev tools, licenses
│   ├── cloud-hosting/           # AWS/GCP/Azure, domains, hosting
│   ├── hardware-equipment/      # Laptops, devices, peripherals
│   ├── professional-fees/       # Attorney, CPA, filing fees
│   ├── office-utilities/        # Coworking, internet, phone
│   ├── travel-meals/            # Business travel and meals
│   └── marketing/               # Ads, website, branding
└── future/                   # Folders to activate as the company grows
    ├── contracts/
    ├── hr-employees/
    ├── insurance/
    ├── licenses-compliance/
    ├── clients-vendors/
    └── investors-fundraising/
```

## Security

Do not store raw account numbers, passwords, or SSNs in plain files here. Keep
them in a password manager and reference them. If this is ever pushed to a
remote, the repository must be private.
