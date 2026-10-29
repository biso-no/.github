<div align="center">

# BISO – BI Student Organisation

**The student organisation for BI Norwegian Business School**

[biso.no](https://biso.no) · [App Store](#) · [Contact](#contact)

</div>

---

## About

BISO (BI Student Organisation) represents and serves students across BI's four campuses. We run events, student services, the web shop, volunteer positions and much more, and we depend on a digital platform that keeps all of it running.

This GitHub organisation is home to the code behind that platform. Everything here is built and operated in-house by BISO's IT function.

## What we build

| Project | Description | Stack |
|---|---|---|
| **BISO Sites** | The unified web platform at [biso.no](https://biso.no): news, events, products and payments, recruitment, reimbursements, a page editor and an admin center | TypeScript, React, Next.js, Appwrite |
| **BISO App** | The mobile hub for students: events, web shop, volunteer positions, membership and expense reimbursements | Flutter |
| **Kroa** | Website for the student bar at BI Oslo: venue and table booking, plus events with sign-up | Next.js |
| **Integrations & automation** | API server connecting accounting, analytics, websites and the app, plus Microsoft 365 automation (SharePoint, Power Automate, Azure Automation) | Node.js, Express, PowerShell, Microsoft Graph |

> Replace or trim this table to match the repositories you actually make public.

## How it fits together

```
        ┌──────────────┐     ┌──────────────┐
        │ BISO Sites   │     │  BISO App    │
        │ (Next.js)    │     │  (Flutter)   │
        └──────┬───────┘     └──────┬───────┘
               │   shared backend   │
               └────────┬───────────┘
                        ▼
                ┌───────────────┐
                │   Appwrite    │  auth · database · storage
                └───────┬───────┘
          ┌─────────────┼──────────────┐
          ▼             ▼              ▼
     Accounting     Vipps Checkout   Microsoft 365
   (24SevenOffice)    (payments)    (SharePoint, Teams)
```

The website and the app share one backend, so a user, an order or a reimbursement looks the same everywhere.

## Highlights

- **One platform instead of many.** Content, events, payments, recruitment and reimbursements live in a single system.
- **AI where it helps.** Receipt reading and cost-center suggestions in reimbursements, an assistant that answers questions about BISO, and an admin assistant. All run on Anthropic's Claude models, and accounting approval stays in the loop.
- **Simple payments.** Payments are consolidated on Vipps Checkout.
- **Built for students.** Used daily across all four BI campuses.

## Tech stack

**Web:** TypeScript, React, Next.js  
**Mobile:** Flutter  
**Backend:** Appwrite (auth, database, storage), Node.js / Express  
**Infrastructure:** Docker, self-hosted servers, nightly backups  
**Microsoft ecosystem:** Microsoft 365, SharePoint, Power Automate, Power BI, Azure Automation, Microsoft Graph  
**Integrations:** 24SevenOffice, Vipps, Anthropic API

## Contributing

Most repositories here are internal to BISO. If you're a BISO volunteer or board member and want to contribute, get in touch with IT first so we can get you access and walk you through the setup.

Found a security issue? Please **do not** open a public issue. Email us instead.

## Contact

- Web: [biso.no](https://biso.no)
- Email: [it@biso.no](mailto:it@biso.no) <!-- confirm address -->

---

<div align="center">
<sub>Built by students, for students. © BI Student Organisation</sub>
</div>
