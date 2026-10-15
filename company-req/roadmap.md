# Company Roadmap: California, F-1 OPT Founder

> General guidance, not legal or tax advice. Before acting on immigration steps,
> confirm them with your DSO and an immigration attorney. Confirm entity and tax
> steps with a CPA. Rules change often (H-1B rules changed a lot in 2025).

## My situation (what this plan assumes)

| | |
|---|---|
| State | **California** |
| SSN | Yes |
| Tax status | **Resident for tax purposes** (not a nonresident alien) |
| Immigration status | F-1, post-completion OPT, EAD received |
| Business | In-house software: mobile apps, web apps, SaaS |
| Revenue | All app and software income goes to **the company**, not to me personally |

> **Tax status and immigration status are separate things.** For taxes I'm a
> resident, so I file like a US person: Form 1040 and CA Form 540, and I pay
> FICA and self-employment tax. This usually applies once someone has been in
> the US on F-1 for more than 5 calendar years. For immigration I'm still F-1,
> so **every OPT and SEVP rule below still applies.**

**Month 0 = the start date printed on my EAD card.** My 90 days of allowed
unemployment count from that date, so the company needs to be formed and I need
to be working 20+ hrs/week as early as possible.

---

## Phase 1: Choose the entity (Week 0–1)

| | California LLC | California C-Corp | Delaware C-Corp + CA registration |
|---|---|---|---|
| State filing fee | $70 | $100 | DE ~$90, plus CA foreign registration $100 |
| Minimum yearly cost | **$800 CA franchise tax starting in year 1** | $800 (CA waives it for a corp's first tax year) | $800 CA, plus DE franchise tax ($400+) and $50 report |
| How profit is taxed | Goes on my personal 1040 (Schedule C). 15.3% self-employment tax | Corp pays 21% federal + 8.84% CA, then I'm taxed on salary or dividends | Same as CA C-Corp |
| Can elect S-Corp later (saves SE tax) | Yes, once profit is around $60k+/yr | Yes | Yes |
| Investors | Must convert first | OK for angels | **Standard for VCs** |
| Paperwork | Low | Medium | Highest |

**Recommendation:**
- **Bootstrapping, with investors at least a year away: California LLC.** It's
  cheapest and simplest. Elect S-Corp tax treatment when profit grows. Convert
  to a Delaware C-Corp when an investor actually asks for it.
- **Raising money within about 12 months: Delaware C-Corp** from the start, plus
  CA foreign registration. Converting an LLC later costs legal fees.

Other decisions:
- [ ] Legal name. Check availability on CA bizfile, search the USPTO trademark
      database, and check the domain is free
- [ ] Registered agent. I can be my own (needs a CA street address) or use a
      service (~$50–$150/yr)
- [ ] Business address. A virtual mailbox keeps my home address off public records

---

## Phase 2: Register in California (Week 1–3)

All state filings go through **bizfileOnline.sos.ca.gov**.

| # | Task | California details | Save to |
|---|---|---|---|
| 1 | File formation documents | LLC: **Form LLC-1** ($70). C-Corp: **Articles of Incorporation** ($100) | `corporate-legal/formation/` |
| 2 | Get an EIN | Free and instant at irs.gov using my SSN | `corporate-legal/ein-tax-ids/` |
| 3 | Operating agreement or bylaws | Not filed with the state, but needed for the bank and for investors | `corporate-legal/operating-agreement/` |
| 4 | **Statement of Information** | Due **within 90 days** of forming. LLC: Form LLC-12 ($20, then every 2 years). Corp: SI-550 ($25, every year) | `corporate-legal/annual-filings/` |
| 5 | Founder shares + **83(b)** | C-Corp with vesting only. File with the IRS **within 30 days**. There's no extension | `corporate-legal/resolutions-minutes/` |
| 6 | IP assignment | Assign all code and designs I made before forming to the company | `corporate-legal/ip-trademarks/` |
| 7 | City business license | Register with my city's business tax office (e.g., LA BTRC, SF Treasurer). SEVP expects self-employed students to hold the licenses the business needs | `future/licenses-compliance/` |
| 8 | Fictitious Business Name (DBA) | Filed with my **county** if I sell under a brand that differs from the legal name, e.g., an app's name. About $25–$60, and I must publish it in a newspaper for 4 weeks | `corporate-legal/formation/` |
| 9 | Seller's permit (CDTFA) | **Usually not needed.** In CA, SaaS and digital downloads generally aren't taxable, and Apple/Google collect sales tax on app sales. Only needed if I sell physical goods | `future/licenses-compliance/` |
| 10 | BOI report (FinCEN) | US-formed companies are currently exempt (rule changed in March 2025). Check again | `corporate-legal/annual-filings/` |
| 11 | Business bank account | Bring formation docs, EIN letter, operating agreement, my ID and EAD. **Never mix personal and business money** | `bank-info/` |
| 12 | Bookkeeping | QuickBooks, Wave, or a spreadsheet. Save receipts from day 1 | `expenses/` |
| 13 | EDD payroll account | Only when I pay myself a salary (C-Corp or S-Corp) or hire. File Form DE 1 | `future/hr-employees/` |
| 14 | D-U-N-S number | Free from Dun & Bradstreet and **required for Apple and Google org accounts**. Can take 1–2 weeks, so apply right after the EIN | `corporate-legal/ein-tax-ids/` |

---

## Phase 3: Route all app and software revenue to the company

The goal: **every dollar from users lands in the company bank account under the
company EIN.** Nothing goes through my personal accounts.

| Platform | How | Notes |
|---|---|---|
| **Apple App Store** | Enroll in the Apple Developer Program as an **Organization**, not an Individual ($99/yr) | Needs the D-U-N-S number, the legal entity name, and a website and email on the company domain. In App Store Connect, enter the **company W-9** and **company bank account** |
| **Google Play** | Create an **Organization** developer account ($25 one time) | Needs the D-U-N-S number. Payments profile in the company name, company bank account |
| **Web / SaaS** | Stripe (or Paddle or Lemon Squeezy) in the company name with the company EIN | Paddle and Lemon Squeezy act as merchant of record and handle sales tax for me |
| **Client or contract work** | Contracts signed by the **company**, invoices from the company | I give clients the company W-9 |
| **Ads / in-app ads** | AdMob and similar, in the company name | Same rule: company W-9, company bank account |

Rules to follow:
- [ ] **Publish under the company accounts from day 1.** Moving apps from a
      personal account to an organization account later is possible but slow.
- [ ] Domain, GitHub org, cloud accounts and trademarks are all owned by the company
- [ ] Record **gross** revenue and the platform fee separately. Apple and Google
      take 15% under their small business programs (if under $1M/yr) or 30%
- [ ] Taking money out. LLC: an **owner's draw** (transfer to my personal
      account and record it). C-Corp or S-Corp: a **salary through payroll**,
      plus dividends or distributions

**OPT note:** Company revenue doesn't affect OPT. What matters is that *I* work
20+ hrs/week for the company in a role related to my degree. Being paid isn't
required, but documented work is.

---

## Phase 4: SEVP Portal and OPT compliance (within 10 days of starting)

### Report my employment
Report within **10 days** of starting work. Use the SEVP Portal, or go through
my DSO if my portal account isn't active. I'll need to enter:
- Employer name (the company's legal name) and address
- Start date
- Job title, for example "Founder & Software Engineer"
- Hours per week (**must be 20 or more**)
- **How the job relates to my degree.** This matters most. Write 3–5 sentences
  connecting my coursework to the actual work: mobile development, backend
  systems, and so on.

After that, report any change (home address, employer details, a new job) within **10 days**.

### OPT rules for being self-employed
- [ ] Work is directly related to my degree field
- [ ] At least 20 hours a week, every week
- [ ] Unemployment days stay under **90 in total** across my 12-month OPT
- [ ] I hold any business licenses the work requires (city license, from Phase 2)

### Keep this evidence in `immigration/employment-evidence/`
- Weekly timesheets or a work log (commits, tickets, calendar)
- A written role description tied to my degree
- Product evidence: repos, App Store and Play Store listings, website, client emails
- Formation docs, EIN letter and city license (copies or links)
- A screenshot of each SEVP Portal submission

---

## Phase 5: Ongoing compliance calendar

| When | Task |
|---|---|
| Every week | Log hours and save receipts |
| Every month | Reconcile the bank account. Categorize expenses and app store payouts |
| Each quarter | Federal **1040-ES** and CA **540-ES** estimated taxes. CA's schedule is 30% / 40% / 0% / 30% (April, June, Sept, Jan) |
| By Jan 31 | Send a 1099-NEC to each US contractor paid $2,000 or more (the threshold for payments from 2026 on). File the CA DE 542 report for new contractors |
| By March 1 | Delaware only: annual report and franchise tax. Use the *assumed par value* method, because the default calculation can produce a huge bill |
| By March 15 | S-Corp: Form 1120-S + CA 100S. Multi-member LLC: Form 1065 + CA 568 |
| By April 15 | Personal **Form 1040 + CA 540**. Single-member LLC: Schedule C on my 1040, plus **CA Form 568**, plus **$800 (Form 3522)**. C-Corp: **Form 1120 + CA Form 100** |
| By June 15 | LLC only: estimated LLC fee (Form 3536) if CA gross receipts exceed $250k |
| Every 1 or 2 years | CA Statement of Information (corp: yearly; LLC: every 2 years) |
| Within 10 days of any change | SEVP Portal update |

**Self-employment tax:** as a tax resident I owe 15.3% self-employment tax on
LLC profit. Electing S-Corp status, once profit is meaningful, can lower it by
splitting income into a reasonable salary plus distributions. Ask a CPA when
that becomes worthwhile.

---

## Phase 6: Opening a company under my company (subsidiary)

A **subsidiary** is a separate legal entity that my main company (the
**parent**) owns. I own the parent, and the parent owns the subsidiary.

```
        Me (100%)
            │
     ParentCo (LLC or C-Corp)
       ┌────┴─────┐
   AppOne LLC   AppTwo LLC     ← each owned 100% by ParentCo
```

### When it's worth it
- One product carries **legal risk** (payments, health data, user-generated
  content) and I want to protect the other products
- An investor wants to invest in **one product only**
- I'm selling one product someday. Selling a whole entity is cleaner
- A product is a **different line of business** (e.g., a consulting arm
  alongside a product arm)

### When it's not (yet)
- **Every California entity costs at least $800/yr** plus its own tax return.
  Five apps as five LLCs means $4,000+/yr before any revenue.
- **Start cheaper:** keep each app inside the parent company and give it its
  own **DBA** (Phase 2, step 8). Create a subsidiary only when one of the reasons
  above actually applies.

### How to set one up
1. [ ] **Get approval inside the parent.** LLC: written consent of the member.
       Corp: a board resolution authorizing the subsidiary. Save it in
       `corporate-legal/resolutions-minutes/`
2. [ ] **File formation documents for the subsidiary.** For example, Form LLC-1.
       The organizer or member listed is **ParentCo**, not me personally
3. [ ] **Subsidiary operating agreement** naming ParentCo as sole member (or
       shareholder)
4. [ ] **Separate EIN.** I'm listed as the "responsible party" with my SSN
5. [ ] **Separate bank account** and separate books. **Never mix money between
       entities.** Commingling can let a court treat them as one company and
       remove the liability protection
6. [ ] **Intercompany agreements.** If the parent owns the IP, write a license to
       the subsidiary. If the parent provides services, use a services agreement
7. [ ] Statement of Information within 90 days, a city license if required, and
       separate developer or Stripe accounts if the subsidiary sells directly
8. [ ] Create a folder for each subsidiary: `corporate-legal/subsidiaries/<name>/`

### How subsidiaries are taxed
- An LLC subsidiary owned 100% by the parent is **disregarded** for federal tax:
  its income shows up on the parent's return. **California still charges the
  $800 and requires its own Form 568.**
- A C-Corp parent that owns 80% or more of a corporate subsidiary can file
  **one consolidated return**.

### OPT note
For SEVP, my employer is the entity **I actually work for and that directs my
work**. If I move my main work to a subsidiary, I update the SEVP Portal
**within 10 days.**

---

## Phase 7: 2–3 year outlook

```
Month 0      EAD start. Company formed, SEVP reported, working 20+ hrs/week
Month 0–1    D-U-N-S, Apple and Google org accounts, Stripe, city license
Month 1–4    First app or MVP shipped under the company accounts
Month 4–9    Revenue or traction. Decide: raise money or bootstrap
~Month 9     Plan next status (STEM OPT? H-1B? O-1?) with an attorney
Month 12     12-month OPT ends
Year 2–3     Status depends on the path chosen below. Consider an S-Corp election
             or C-Corp conversion. Add subsidiaries only if needed
```

### Path A: STEM OPT extension (+24 months)
- Only possible if my degree is on the STEM designated list
- **Self-employment is not allowed on STEM OPT.** I'd need a real
  employer-employee relationship, an employer enrolled in E-Verify, and a Form
  I-983 training plan with a supervisor.
- For a company I own, that means real supervision by someone else, such as a
  board or co-founder. It's risky and needs an attorney.
- The other route is a STEM OPT job at another company while I build mine on the
  side, within the rules.
- Apply up to 90 days before OPT ends.

### Path B: H-1B through my own company
- Since January 2025, owners holding more than 50% can be sponsored by their own
  company, but approvals are limited to **18 months** for the first petition and
  the first extension.
- The company must be able to pay the prevailing wage and show it has a real
  need for the role.
- Registration opens in **March** each year, and selection is a lottery. Cap-gap
  can extend my OPT to April 1 if I'm selected.
- 2025 brought changes to selection and fees. Check the current rules before
  each March.
- **Investors help here.** A board that can hire and fire me strengthens the
  employer-employee relationship.

### Path C: O-1A (extraordinary ability)
- No lottery. Needs evidence such as press, awards, judging, high pay,
  significant funding, or apps with significant user numbers or revenue.
- Start building this evidence now: speaking, publications, open source, press,
  app metrics.

### Path D: Other
- **Cap-exempt H-1B:** part-time work at a university or nonprofit research
  organization, while running the company.
- **E-2:** only if my country of citizenship has a treaty with the US.
- **EB-2 NIW (long term, green card):** possible once the company shows
  national-level impact.

### If I raise money
- An LLC must convert to a Delaware C-Corp first
- Early rounds commonly use SAFEs
- Set up a cap table and an option pool
- Keep everything in `future/investors-fundraising/`

---

## My next 7 actions
1. [ ] Write down my EAD start date. My 90-day unemployment count starts then
2. [ ] Choose a CA LLC or a DE C-Corp (talk to a CPA or attorney this week)
3. [ ] File on bizfileOnline, then get the EIN online
4. [ ] Apply for a D-U-N-S number
5. [ ] Open the business bank account
6. [ ] Report the company in the SEVP Portal within 10 days of starting work
7. [ ] Enroll in the Apple and Google developer programs as an Organization
