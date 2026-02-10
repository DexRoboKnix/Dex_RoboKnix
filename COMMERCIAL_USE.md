# Commercial Use & Licensing Guide

## TL;DR

DEXSPINE is **free for open source** and **paid for proprietary SaaS**. The AGPL v3 license requires that if you run DEXSPINE on a server and let users interact with it over a network, you must **open-source your entire backend**—or buy a commercial license.

This is intentional. It's called **the AGPL trap**.

---

## The Two Licenses

### 1. Open Source: GNU AGPL v3

**You can use DEXSPINE for free if:**

- ✅ Your project is open source (any OSI-approved license)
- ✅ You use it internally in your company (no external users)
- ✅ You're doing research or education
- ✅ You're willing to open-source your entire backend if you offer network access

**The AGPL Network Clause:**

> If you run DEXSPINE on a server and users interact with it over a network (web app, API, SaaS), you must provide the **complete source code** of your application to those users.

**Example scenarios:**

✅ **Allowed without source disclosure:**

- Running DEXSPINE locally on your laptop
- Using it in internal company tools (no external users)
- Building an open-source application that includes DEXSPINE
- Academic research and publication

❌ **Requires source disclosure OR commercial license:**

- Building a SaaS product that uses DEXSPINE on the backend
- Offering DEXSPINE as a paid API
- Embedding DEXSPINE in a proprietary web application
- Creating a "DEXSPINE as a Service" platform

---

### 2. Commercial License

**You need a commercial license if:**

- You want to embed DEXSPINE in a proprietary product
- You're building a SaaS/web app and don't want to open-source your code
- You're offering DEXSPINE-powered services to customers
- You need legal protection and indemnification

**What the commercial license gives you:**

- ✅ No source code disclosure requirement
- ✅ Use in proprietary/closed-source products
- ✅ Sublicensing rights
- ✅ Commercial support and updates
- ✅ Legal indemnification
- ✅ Custom modifications allowed

**Pricing:** Contact danielcheeseman@me.com for quote.

We offer:

- **Startup License** - For companies <10 employees
- **Enterprise License** - For larger organizations
- **OEM License** - For resellers and integrators

---

## Understanding the AGPL "Trap"

The AGPL v3 is the "strongest" open-source license. It's designed to prevent the **SaaS loophole** where companies take open-source software, run it on their servers, and never contribute back.

### How it works:

**Regular GPL (v2/v3):**

> "If you distribute the software, you must provide source code."

**Problem:** SaaS companies don't "distribute" anything—they just run it on their servers.

**AGPL v3 Solution:**

> "If users interact with the software over a network, that counts as distribution. You must provide source code."

**Result:** You can't build a proprietary SaaS product on top of AGPL code without either:

1. Open-sourcing your entire application, or
2. Buying a commercial license

This is why companies like MongoDB, Elastic, and others use AGPL for their core products.

---

## Real-World Examples

### ✅ Example 1: Internal Company Use

**Scenario:** Your company uses DEXSPINE to audit internal systems. Only employees access it.

**License:** AGPL v3 (free)  
**Why:** No external users = no network distribution = no source disclosure required.

---

### ✅ Example 2: Open Source Project

**Scenario:** You build an open-source documentation tool that uses DEXSPINE. You publish it on GitHub.

**License:** AGPL v3 (free)  
**Why:** Your entire project is open source anyway. AGPL requirements already met.

---

### ❌ Example 3: SaaS Product (Requires Commercial License)

**Scenario:** You build "ArchitectAI.com" - a paid web app where users upload documents and DEXSPINE analyzes them.

**License:** Commercial License (paid)  
**Why:** Users access DEXSPINE over the network. AGPL requires you to open-source your entire backend (pricing, user management, database, everything). You don't want to do that, so you need a commercial license.

**Alternative:** Open-source your entire application and use AGPL.

---

### ❌ Example 4: API Service (Requires Commercial License)

**Scenario:** You offer `api.yourcompany.com/dexspine` as a paid API that runs DEXSPINE on the backend.

**License:** Commercial License (paid)  
**Why:** API access is network distribution. AGPL requires source disclosure. Commercial license removes this requirement.

---

### ✅ Example 5: Academic Research

**Scenario:** You use DEXSPINE in a research paper comparing cognitive frameworks.

**License:** AGPL v3 (free)  
**Why:** Research and education are explicitly allowed. Just cite the software (see CITATION.cff).

---

### ⚠️ Example 6: Consulting Service (Gray Area)

**Scenario:** You're a consultant. You run DEXSPINE locally and deliver reports to clients.

**License:** AGPL v3 (free) - but be careful  
**Why:** You're not providing network access to DEXSPINE itself. You're using it as a tool and delivering the _output_. This is similar to using Photoshop to make graphics—you don't need to license Photoshop to sell the graphics.

**However:** If you build a web portal where clients can run DEXSPINE themselves, that's network distribution → commercial license required.

---

## FAQ

### Q: Can I modify DEXSPINE?

**A:** Yes, under AGPL. But if you distribute your modifications (including network access), you must open-source them.

### Q: Can I use DEXSPINE in a startup?

**A:** Yes. If it's internal-only or open source, use AGPL. If you're building a SaaS product, you need a commercial license.

### Q: What if I just use the DEXSPINE _output_, not the protocol itself?

**A:** The output is not covered by AGPL. The protocol/software is. If you run DEXSPINE once, save the output, and use that output elsewhere, you're not distributing DEXSPINE.

### Q: Can I fork DEXSPINE and rename it?

**A:** Yes, under AGPL. But:

1. You must keep the AGPL license
2. You must provide source code if you offer network access
3. You must credit the original (see LICENSE)

### Q: What counts as "network distribution"?

**A:** Any scenario where a user interacts with DEXSPINE through a network:

- Web applications (users access via browser)
- APIs (users call your API which runs DEXSPINE)
- Mobile apps connecting to your server running DEXSPINE
- Desktop apps connecting to your backend running DEXSPINE

**Does NOT count:**

- Running DEXSPINE on your laptop
- Running it on company servers for internal use only
- Sending DEXSPINE output (reports, documents) to others

### Q: Is the AGPL enforceable?

**A:** Yes. The Free Software Foundation actively enforces AGPL violations. Companies have been sued and forced to either:

1. Open-source their entire codebase
2. Settle for significant payments
3. Switch to a commercial license

Notable cases: Artifex Software (Ghostscript), MongoDB (before license change), various compliance lawsuits.

### Q: Why not use MIT or Apache license?

**A:** Because those licenses allow companies to take the work, wrap it in proprietary software, and never contribute back. AGPL ensures that improvements benefit the community OR the author gets compensated.

### Q: Can I use DEXSPINE with other AGPL software?

**A:** Yes, AGPL is compatible with AGPL. You can combine DEXSPINE with other AGPL projects.

### Q: Can I use DEXSPINE with GPL (non-AGPL) software?

**A:** Generally yes, but consult a lawyer. AGPL is compatible with GPL v3, but the AGPL network clause applies to the combined work.

### Q: Can I use DEXSPINE with proprietary software?

**A:** Only with a commercial license. Mixing AGPL with proprietary code requires the entire combined work to be AGPL (including the proprietary parts)—which defeats the purpose of proprietary software.

---

## When You Need a Commercial License

You definitely need a commercial license if:

1. **SaaS Product:** Users access DEXSPINE via your web application
2. **API Service:** You offer DEXSPINE via API (paid or free)
3. **Proprietary Integration:** You embed DEXSPINE in closed-source software
4. **OEM/Resale:** You want to resell DEXSPINE as part of your product
5. **Source Code Protection:** You can't or won't open-source your backend

---

## How to Get a Commercial License

**Step 1:** Email danielcheeseman@me.com with:

- Brief description of your use case
- Expected user volume (if SaaS/API)
- Company size and revenue (for pricing tier)

**Step 2:** We'll send you:

- Commercial license agreement
- Pricing quote
- Terms and conditions

**Step 3:** Sign and pay, receive:

- Commercial license file
- Legal indemnification
- Support SLA (optional)
- Custom modifications (optional)

**Typical turnaround:** 3-5 business days

---

## Compliance Best Practices

### If using AGPL (free):

1. ✅ Include LICENSE file in your distribution
2. ✅ Credit DEXSPINE in your documentation
3. ✅ If offering network access, provide source code link
4. ✅ Document any modifications you make
5. ✅ Keep the copyright notices intact

### If using Commercial License:

1. ✅ Keep license file private (it's your proof of purchase)
2. ✅ Follow terms of the commercial agreement
3. ✅ Credit DEXSPINE in "About" or documentation (optional but appreciated)
4. ✅ Renew annually if subscription-based
5. ✅ Contact us before major modifications

---

## The Author's Philosophy

DEXSPINE is the result of hundreds of hours of research, testing, and refinement. The dual-license model ensures:

1. **Open source benefits the community** - Students, researchers, and open-source projects can use it freely
2. **Commercial use funds development** - Companies that profit from DEXSPINE contribute back, enabling continued improvement
3. **No proprietary gatekeeping** - Anyone can see the source code, learn from it, and modify it
4. **Sustainable development** - The author can invest time in improvements without relying on donations

This model has worked for MongoDB, Redis, Elasticsearch, and many others. It balances openness with sustainability.

---

## Contact

**General Questions:** GitHub Discussions  
**Commercial Licensing:** danielcheeseman@me.com
**Legal/Compliance:** danielcheeseman@me.com
**Support (License Holders):** danielcheeseman@me.com

---

**Last Updated:** February 2026  
**License Version:** AGPL v3 / Commercial v1.0

_Not legal advice. Consult a lawyer for your specific situation. This document explains the license terms in plain language but the actual LICENSE file is the legally binding text._
