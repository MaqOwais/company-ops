# Company Roadmap: F-1 OPT Founder

> General guidance, not legal or tax advice. Before acting on immigration steps,
> confirm them with your DSO and an immigration attorney. Confirm entity and tax
> steps with a CPA. Rules change often (H-1B rules changed a lot in 2025).

**Month 0 = the start date printed on your EAD card.** Your 90 days of allowed
unemployment start counting from that date, so the company needs to be set up
and you need to be working 20+ hrs/week as early as possible.

---

## Phase 1: Decide before filing (Week 0–1)

### Entity type

| | Single-member LLC | Delaware C-Corp |
|---|---|---|
| Cost / admin | Low | Higher (franchise tax, separate tax return) |
| Investors | VCs won't invest; you'd have to convert | Standard for VC funding |
| Taxes for you (nonresident alien) | Must file **Form 5472 + pro forma 1120** every year ($25,000 penalty if missed) | Company files Form 1120 |
| Future H-1B through own company | Possible | Possible, and simpler once you have a board |

- **If you're serious about raising money in 1–3 years, a C-Corp is usually the
  better choice.** Converting later costs money.
- **An S-Corp is not an option.** Nonresident aliens cannot own S-Corp shares.
- **If you choose Delaware:** you also have to register (foreign-qualify) in the
  state where you live and work.

### Other decisions
- [ ] Company name. Check it's available with the state and USPTO, and that the domain is free
- [ ] Registered agent (a service costs about $50–$300/yr, or use your own address)
- [ ] Business address (a virtual address keeps your home address private)

---

## Phase 2: Register the company (Week 1–3)

| # | Task | Notes | Save to |
|---|---|---|---|
| 1 | Get an SSN | Bring your EAD, passport, I-94 and I-20 to the SSA office. Having an SSN makes getting the EIN easy | `immigration/passport-visa-i94/` |
| 2 | File formation documents | LLC: Articles of Organization. C-Corp: Certificate of Incorporation | `corporate-legal/formation/` |
| 3 | Get an EIN | Free at irs.gov (online needs an SSN or ITIN). Without either, fax Form SS-4 | `corporate-legal/ein-tax-ids/` |
| 4 | Operating agreement or bylaws | C-Corp: also adopt initial board consent and issue founder shares | `corporate-legal/operating-agreement/` |
| 5 | **83(b) election** (C-Corp with vesting) | File with the IRS **within 30 days** of the share issuance. There's no extension, so don't miss it | `corporate-legal/resolutions-minutes/` |
| 6 | Foreign qualification | Only if formed in a state other than where you operate | `corporate-legal/formation/` |
| 7 | State and city business license | Requirements vary. SEVP expects self-employed students to hold the licenses the business needs | `future/licenses-compliance/` |
| 8 | State tax registration | Only if you sell taxable products. Software and SaaS sales tax rules vary by state | `corporate-legal/ein-tax-ids/` |
| 9 | BOI report (FinCEN) | US-formed companies are currently exempt (rule changed in March 2025). Check again | `corporate-legal/annual-filings/` |
| 10 | Business bank account | Bring formation docs, EIN letter, operating agreement, passport and EAD. Never mix personal and business money | `bank-info/` |
| 11 | Bookkeeping | QuickBooks, Wave, or a spreadsheet. Save receipts from day 1 | `expenses/` |
| 12 | IP assignment | Assign any code you wrote before forming the company to the company | `corporate-legal/ip-trademarks/` |

---

## Phase 3: SEVP Portal and OPT compliance (within 10 days of starting)

### Report your employment
Report within **10 days** of starting work. Use the SEVP Portal, or go through
your DSO if your portal account isn't active. You'll need to enter:
- Employer name (your company) and address
- Start date
- Job title, for example "Founder & Software Engineer"
- Hours per week (**must be 20 or more**)
- **How the job relates to your degree.** This matters most. Write 3–5 sentences
  connecting your coursework to the actual work.

After that, report any change (address, employer details, a new job) within **10 days**.

### OPT rules for being self-employed
- [ ] Work is directly related to your degree field
- [ ] At least 20 hours a week, every week
- [ ] Unpaid work is allowed on post-completion OPT, but it must be real, documented work
- [ ] Unemployment days stay under **90 in total** across your 12-month OPT
- [ ] You hold any business licenses the work requires

### Keep this evidence in `immigration/employment-evidence/`
- Weekly timesheets or a work log (commits, tickets, calendar)
- A written role description tied to your degree
- Product evidence: repos, releases, website, client emails
- Formation docs, EIN letter and licenses (copies or links)
- A screenshot of each SEVP Portal submission

---

## Phase 4: Ongoing compliance calendar

| When | Task |
|---|---|
| Every week | Log hours and save receipts |
| Every month | Reconcile the bank account and categorize expenses |
| Each quarter | Estimated tax payments, if profitable (April, June, Sept, Jan) |
| By Jan 31 | Send a 1099-NEC to each US contractor paid $600 or more (threshold rises to $2,000 for payments from 2026) |
| By March 1 | Delaware annual report and franchise tax (C-Corp). Use the *assumed par value* method, because the default calculation can produce a huge bill |
| By March 15 | Partnership/S-Corp returns (doesn't apply to you) |
| By April 15 | Personal **Form 1040-NR + Form 8843**. LLC: **5472 + pro forma 1120**. C-Corp: **Form 1120** |
| Your state's anniversary date | State annual report and registered agent renewal |
| Within 10 days of any change | SEVP Portal update |

**Tax residency:** F-1 students are usually nonresident aliens for their first 5
calendar years in the US. That generally means filing the 1040-NR, no FICA on
your wages, and no self-employment tax. Have a CPA confirm this for your
situation.

---

## Phase 5: 2–3 year outlook

```
Month 0      EAD start. Company formed, SEVP reported, working 20+ hrs/week
Month 0–3    MVP built, first users or clients, bookkeeping running
Month 3–9    Revenue or traction. Decide: raise money or bootstrap
~Month 9     Plan next status (STEM OPT? H-1B? O-1?) with an attorney
Month 12     12-month OPT ends
Year 2–3     Status depends on the path chosen below
```

### Path A: STEM OPT extension (+24 months)
- Only possible if your degree is on the STEM designated list
- **Self-employment is not allowed on STEM OPT.** You need a real
  employer-employee relationship, an employer enrolled in E-Verify, and a Form
  I-983 training plan with a supervisor.
- For a company you own, that means real supervision by someone else, such as a
  board or co-founder. It's risky and needs an attorney.
- The other route is a STEM OPT job at another company while you build yours on
  the side, within the rules.
- Apply up to 90 days before OPT ends.

### Path B: H-1B through your own company
- Since January 2025, owners holding more than 50% can be sponsored by their own
  company, but approvals are limited to **18 months** for the first petition and
  the first extension.
- The company must be able to pay the prevailing wage and show it has a real
  need for the role.
- Registration opens in **March** each year, and selection is a lottery. Cap-gap
  can extend your OPT to April 1 if you're selected.
- 2025 brought changes to selection and fees. Check the current rules before
  each March.
- **Investors help here.** A board that can hire and fire you strengthens the
  employer-employee relationship.

### Path C: O-1A (extraordinary ability)
- No lottery. You need evidence such as press, awards, judging, high pay,
  significant funding or original contributions.
- Start building this evidence now: speaking, publications, open source, press.

### Path D: Other
- **Cap-exempt H-1B:** part-time work at a university or nonprofit research
  organization, while running the company.
- **E-2:** only if your country of citizenship has a treaty with the US.
- **EB-2 NIW (long term, green card):** possible once the company shows
  national-level impact.

### If you raise money
- Convert the LLC to a C-Corp first (if you started as an LLC)
- Early rounds commonly use SAFEs
- Set up a cap table and an option pool
- Keep everything in `future/investors-fundraising/`

---

## Your next 5 actions
1. [ ] Write down your EAD start date. Your 90-day unemployment count starts then
2. [ ] Choose LLC or C-Corp (talk to a CPA or attorney this week)
3. [ ] Apply for an SSN
4. [ ] File formation documents, then get the EIN
5. [ ] Report the company in the SEVP Portal within 10 days of starting work
