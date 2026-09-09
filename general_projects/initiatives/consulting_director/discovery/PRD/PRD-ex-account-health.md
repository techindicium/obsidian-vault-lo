# EX Account Health: 4D Product Requirement Document (PRD)

*This document defines the "What" and "Why" of the data product, with a focus on observability, SLAs, and exception handling.*

---

## 📇 General Information

* **Product:** EX Account Health
* **Version:** 0.2
* **Date:** 08/13/2026
* **Authorship (PM/PO):** Lorena Santos
* **Status:** Refinement

---

## 🔎 [PHASE 1: DISCOVERY]

*Focus: Problem and stakeholder alignment before the solution.*

### **1. Context and Motivation**

* **As-Is Process:** *(validated)* Account tracking today is manual and dispersed across the CRM (pipeline/contract data), a profitability system (access restricted to Operations/Finance), meeting transcripts, Slack, email and account-planning spreadsheets — organized however each Consulting Director personally works. All 8 CDs fill a monthly Delivery Scorecard with an Overall RAG + 4 blocks (Profitability, Delivery Health & Pulse, Growth, Risks); this product will **consume** that RAG, not recalculate it independently. The two prior manual leadership reports fed by these same sources are no longer this initiative's concern — they are served by a separate, parallel Delivery Dashboard initiative. *(hypothesis, partial sample)* Individual habits vary significantly across CDs — some rely on informal AI-assisted filtering of source spreadsheets, others keep most tracking in memory with a much less structured process.
* **Pain Points and Problems:** *(validated)* The core pain is **lack of forward-looking visibility into account risk and opportunity** — not primarily time spent filling reports. A recurring root cause behind that pain, raised independently by both discovery interviews, is that **the information needed to see risk/opportunity ahead of time is often hard to reach, access-restricted, or simply doesn't exist in structured form anywhere** — this is a data-access problem, not only a tooling or habit problem. Concretely: (1) risk/opportunity signal lives mostly in unstructured sources (meeting transcripts, Slack, email), with nothing structured today; (2) profitability/margin data is access-restricted to CDs, leaving that block blank most months; (3) knowledge of which people/profiles are available for allocation is tacit, concentrated in a few roles, and not shared with CDs ahead of a decision; (4) forward-looking financial status (e.g., contract billing/consumption against value, upcoming due dates) is not available in a structured, proactive way — CDs must chase it manually. Separately, (5) CRM data quality is inconsistent for cultural, not tooling, reasons — this is a data-*quality* problem, distinct from the access problem above.
* **Key Stakeholders:** **Sponsor:** undecided — candidates are the VP of Consulting or the VP of Operations (see Open Issues). **Data Owners (per source, not a single owner):** the Delivery Scorecard/RAG rubric and profitability/margin data are owned by Operations/Finance; the account-planning spreadsheet (revenue target) is owned by Commercial; CRM/pipeline data (Salesforce) is owned by Finance; ownership of meeting-transcript data is unconfirmed (open question). **Consumers:** all 8 Consulting Directors, each scoped to their own portfolio. Whether Commercial should have access to any slice of this is an open question.

### **2. Objective and JTBD**

* **Overview:** *(validated)* A personal support tool for each Consulting Director that centralizes dispersed account information — RAG status, pipeline, narrative context, finantial — into one place, so the CD can see risk and opportunity ahead of time instead of reconstructing it manually from scattered sources every cycle.
* **Persona:** Consulting Director — each of the 8 CDs, scoped only to their own portfolio.
* **Job to be Done:** *(validated)* As a Consulting Director, I need to see early signals of risk and opportunity across my accounts — spanning financial, delivery, commercial, and people dimensions — pulled together from otherwise scattered and hard-to-access sources, so I can act before a problem escalates or an opportunity is lost, instead of reconstructing that picture manually every cycle. *(validated, both interviews)* Success is centralizing that fragmented information to support decisions — allocation, new proposals, client actions — a qualitative outcome about improved decision quality, not a directly measurable financial return.

### **3. CSD Matrix**

> 💡 *Single source of certainties, assumptions, and doubts for the product. In other sections, unresolved items should be referenced here with `→ CSD` instead of repeated. Doubts are automatically candidates for Open Issues (section 9).*

---

✅ **CERTAINTIES**
* Solution serves all 8 CDs, each with access scoped only to their own portfolio.
* This product is **Americas-scoped** — Europe's parallel data/sources (Kimble, Kimble-based engagement/assignment models, Europe-only Salesforce margin fields, etc.) are out of scope for this product's own data access, even where a Delivery Dashboard reuse candidate happens to have both an Americas and a Europe version.
* RAG status (Overall + 4 blocks) is consumed from the existing Delivery Scorecard, not recalculated independently.
* CDs want risk/opportunity insight, not just raw data display.
* CDs want a space to add their own signed comments/insights on each account (human-authored, persisted).
* Two delivery channels are both wanted, not one instead of the other: an actively-accessed artifact **and** a Slack notification/nudge (how far this generalizes across all CDs is still a doubt).
* Proposal review/building is a fully separate process — explicitly out of scope.
* The CRM/commissions initiative is separate and must not share a solution/artifact with this one.
* Account-plan adherence should not be a single-owner (CD-alone) judgment.
* External-context AI opportunity-surfacing (cross-referencing account context with market/competitor data) is a formal report item, replacing the internal blind-spot-detection framing originally planned. The narrative-synthesis-of-the-period item is unaffected and stays as a separate feature.
* The JTBD as synthesized is validated by the product owner as the working objective, without requiring a separate word-for-word re-confirmation from the primary stakeholder.
* Meeting-transcript access is SSO-authenticated via the Google Drive/Slack MCP, using each CD's own credentials, searched by date and meeting name — not a manually-invited service user per recurring meeting. The CD must be added at least as an optional attendee to a meeting to have access to its transcript; this is the actual access boundary.

---

🔶 **ASSUMPTIONS**
* A per-proposal client contact field and a contract-consumption view (billed vs. total) add real value — untested beyond a single CD.
* CDs organizing their own way "each in their own style" partially holds, but there is also appetite for standardizing tooling across CDs — convergence may be more possible than initially assumed.
* A stated preference for a live artifact over a Slack alert, and skepticism toward AI-generated recommendations from meeting transcripts, may be personal habits rather than CD-wide patterns — a second interview diverged on both points.
* Generalization beyond the first interviewed CD (→ R4) is only partially tested — 2 of 8 CDs interviewed.

---

❓ **DOUBTS**
1. Profitability/margin — governance: even with technical access, should CDs see this at all? (policy call, not ours to make)
2. Profitability/margin — technical access still blocked; a parallel initiative elsewhere in the org may already be addressing this — check before duplicating.
3. Does the Delivery Dashboard expose (or plan to expose) RAG history over time? Blocks the trend/deterioration report block if not.
4. Owner/Sponsor is undecided.
5. Does Commercial get access to any part of this solution? Not asked directly.
6. Impact of an ongoing organizational restructuring affecting the CD role — scope and timing unknown.
7. Should this live as a separate product, or become a tab inside the Delivery Dashboard? Not decided.
8. Full list of consolidated open questions and risk mitigation plans: see scratchpad.

### **4. Out of Scope (Features Out)**

* Proposal review/building — a separate process, categorically confirmed out of scope.
* Weekly and monthly manual leadership reports — now served by the separate Delivery Dashboard initiative, not by this product.
* The CRM/commissions initiative — a different initiative; confirmed it must not share a solution/artifact.
* Profitability/margin display — parked pending both a technical access decision and a separate governance decision (see CSD Doubts 1–2).
* An async channel for field teams to flag incipient client discussions — judged very unlikely to be feasible: depends on transcribing/accessing chats inside the client's own environment, an access wall already confirmed to exist on at least one account. Kept only as a reflection idea, not planned into any version.
* Account-plan adherence ("Pacing") — not out of scope permanently, but deliberately deferred to a future version; see Roadmap.

### **5. Dependencies and Risks**

*(agent-led synthesis from discovery — not yet re-validated with the stakeholder as a finalized list; mitigation plans intentionally blank per discovery process)*

| # | Risk / Dependency | Evidence | Impact |
|---|---|---|---|
| R1 | Profitability (margin) owned outside Delivery, not accessible to CDs; governance question is separate from technical access | Confirmed gap; blank most months in the Delivery Scorecard | High |
| R2 | Source data largely unstructured (Slack, email, transcripts, free-text) | Confirmed: "nothing structured" | High |
| R3 | RAG rubric leaves room for subjective judgment | Rubric wording itself | Medium |
| R4 | Adoption risk: only 2 of 8 CDs' workflows/preferences captured, and they diverge on 2 of 4 compared points | Two discovery interviews | Medium |
| R8 | Coordination dependency on the separate Delivery Dashboard initiative for RAG data/history | Delivery Dashboard has its own open access-matrix blocker and delivery-data timeline | High |
| R10 | Ongoing restructuring affecting the CD role, scope and timing unknown | Raised directly by the primary stakeholder, more than once | Medium-High |

*(Earlier risks now resolved or no longer applicable are not carried into this table — see scratchpad Judgment Calls Log for their resolution history.)*

---

## 📐 [PHASE 2: DESIGN]

*Focus: Technical, functional specification and confidence metrics.*

### **6. Versions and Features (Slicing)**

*(synthesized from the roadmap draft and the mock content revision — not yet re-validated with the sponsor or the remaining CDs; acceptance criteria, telemetry, and exception handling below are placeholders pending a dedicated Design session, not yet discussed with any stakeholder)*

**V1 name:** Personal Account Health View — MVP.
**V1 objective:** the smallest useful slice — a per-CD, two-tab view (Portfolio + Account Detail) consuming existing RAG/CRM/planning data, with a Slack notification pointing to it. No independent recalculation of RAG, no proposal building, no action tracking.
**Main use case:** Trigger — the underlying data (Delivery Scorecard, CRM, transcripts) is refreshed → Logic — the product pulls and structures that data per account, scoped to the CD's own portfolio → Result — a Slack notification tells the CD the view is updated with a link; opening it shows the Portfolio grid, and any account can be opened into its Detail view.

**Feature list by version:**

**V1 (MVP):**
- Portfolio view, scoped per CD
- RAG status (Overall + 4 blocks), consumed from the Delivery Scorecard
- Narrative synthesis of the period (meeting transcripts)
- Slack notification + link, alongside direct access to the artifact
- Financial summary + contract-consumption view (billed vs. total)
- Commercial pipeline detail with per-proposal client contact
- Sources / freshness footer, including when each Databricks-sourced block (RAG, Account Plan, Squad allocation) was last refreshed upstream

**V2:**
- Opportunities and Risks sections, with a signed CD comment space (human-authored, not AI-generated from a transcript)

**V3:**
- Collapsed squad & key contacts view per account
- RAG history/trend over time per block (depends on the Delivery Dashboard exposing a time series)
- AI cross-referencing external market/competitor context to surface opportunities

**V4:**
- Account-plan/pacing adherence (must be a joint CD + Commercial evaluation when designed, not a CD-only judgment)

**Retired — not part of any version:** an action checklist (proactive next steps + stalled-action alerts) and a separate AI-generated CD recommendation.

---

**User Stories (detail)**

*(Acceptance criteria, telemetry, business rules, SLAs, and exception handling below are placeholders pending a dedicated Design session — not yet discussed with any stakeholder.)*

*V1:*
1. AS A Consulting Director, I WANT a portfolio-level view of all my accounts with their overall RAG status and key numbers SO THAT I can scan my whole book and spot what needs attention without opening each account individually.
   * *Acceptance Criteria / Telemetry / Business Rules / SLA / Exception Handling: (pending)*
2. AS A Consulting Director, I WANT to see the Overall RAG and its 4 underlying blocks for a given account, with a link back to the Delivery Dashboard SO THAT I can trust the status without re-deriving it myself.
   * *Business Rule (confirmed):* RAG is consumed as-is from the Delivery Scorecard, never recalculated independently.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*
3. AS A Consulting Director, I WANT a narrative synthesis of the period generated from meeting transcripts SO THAT I don't have to re-read or re-listen to reconstruct what happened.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*
4. AS A Consulting Director, I WANT to be notified in Slack when my report is updated, with a link to open it, in addition to being able to access it directly at any time SO THAT I don't have to remember to check it, without Slack being the only way in.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*
5. AS A Consulting Director, I WANT a financial summary per account — open/closed pipeline and contract consumption (billed vs. total value) SO THAT I can anticipate billing/contract status without chasing Finance manually.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*
6. AS A Consulting Director, I WANT commercial pipeline detail per account, including the specific client-side contact for each proposal SO THAT I know who to engage without confusing it with the internal squad assignment.
   * *Business Rule (hypothesis, depends on CRM data quality):* pipeline detail quality is bounded by CRM fill-in completeness.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*
7. AS A Consulting Director, I WANT a footer showing which sources fed this report and when each Databricks-sourced block was last refreshed upstream SO THAT I know how current each piece of information is instead of assuming it's all equally fresh.
   * *Business Rule (confirmed):* live-MCP data (Salesforce, transcripts) is fetched at generation time; Databricks-ingested data (RAG, Account Plan, Squad allocation) refreshes on its own upstream cadence — the footer must surface that gap per block, not just list source names.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*

*V2:*
7. AS A Consulting Director, I WANT dedicated Opportunities and Risks sections with a space for my own signed comment on each SO THAT I can record my own read without it being conflated with an AI-generated recommendation.
   * *Business Rule (confirmed):* comments are human-authored and attributed, never AI-generated from a transcript. No AI contribution feeds this section — external-context AI opportunity-surfacing is a separate, formal report item instead.
   * *Acceptance Criteria / Telemetry / SLA / Exception Handling: (pending)*

### **7. High-Level Architecture**

*(high-level data flow only — technical implementation, schemas, and pipeline design are out of scope for this document; one architecture decision below is explicitly undecided)*

**Data Concepts — what the product is built from:**

Everything the product shows comes out of combinations of these concepts. State legend: ✅ source and access confirmed · ⚠️ source identified, with an open caveat · 🚧 no source identified yet.

| # | Concept | Source | Owner | State | Existing table (if any) |
|---|---|---|---|---|---|
| 1 | **Account** — identification and structure | Salesforce | Finance | ✅ confirmed | `stg_salesforce__account` (Delivery Dashboard repo) |
| 2 | **CD (Person)** — who owns which accounts, portfolio scoping | Kantata or CD's own identity/session | — | ⚠️ ongoing Consultoria/CD restructuring, scope and timing unknown (→ CSD Doubt 6) | — |
| 3 | **RAG Status** — Overall + 4 blocks | Delivery Scorecard, via Delivery Dashboard | Operations | ✅ source confirmed, consumed as-is; ⚠️ history over time still open (→ CSD Doubt 3); Delivery Dashboard itself is a coordination dependency, not a data question (→ R8) | 🚧 needs fresh ingestion — bypasses dbt (Lakebase write-back), and only models 3 sub-statuses vs. the 4 blocks here (→ R11) |
| 4 | **Commercial Pipeline / Opportunity** — proposal, stage, probability, forecast, close date, client contact | Salesforce | Finance | ✅ confirmed | `stg_salesforce__opportunity` (Delivery Dashboard repo) |
| 5 | **Financial summary / contract consumption** — billed vs. total contract value | Salesforce | Finance | ✅ confirmed | Not yet checked against the Delivery Dashboard repo |
| 6 | **Account Plan / Target** — revenue target per account, engagement-level tracking | Account-planning spreadsheet | Commercial | ✅ confirmed structured and pullable | 🚧 needs fresh ingestion — no ingestion of this spreadsheet exists in the Delivery Dashboard repo |
| 7 | **Profitability / Margin (GM%)** | Spreadsheets today (this product is Americas-scoped — data exists, but this format makes automated extraction hard). **Correction (08/21/2026):** the "Salesforce planned as future source" note no longer holds as stated — the CRM field mapping confirms Salesforce's margin fields (`Sold_Margin__c`, `Margin_Amount__c`, approval workflow) are used by Europe only; whether any future Salesforce migration would extend to Americas is unconfirmed | Operations | 🚧 access-restricted to CDs — both a technical and a governance question (→ CSD Doubts 1–2) | Checked (CRM field mapping, 08/21/2026): margin fields exist in Salesforce but are Europe-only — not usable for this Americas-scoped product |
| 8 | **Narrative signal — meeting transcripts** | Google Drive, via SSO-authenticated MCP (each CD's own credentials) | Each CD, individually | ✅ access mechanism confirmed — boundary is being at least an optional attendee on the meeting; ⚠️ content itself remains unstructured (→ R2) | — |
| 9 | **Narrative signal — Slack (per-account channels)** | Slack, via the same SSO-authenticated MCP mechanism as item 8 | Each CD, individually | ✅ access mechanism confirmed; ⚠️ content itself remains unstructured (→ R2) | — |
| 10 | **Squad allocation** — who's staffed on which account | Operations allocation spreadsheet | Operations | ⚠️ confirmed as current source; being replaced by Kantata, timeline not yet defined | `stg_indicium_dbt__allocation` (Americas) / `int_kimble__assignment` (Europe), both in the Delivery Dashboard repo |
| 11 | **Key contacts** — client-side stakeholders per account/proposal | — | — | 🚧 no source identified | Checked: `stg_salesforce__contact` exists but redacts external names/emails by design — not usable |

**Delivery/consumption layer — undecided (open architecture question, not a Discovery question):** Slack's role is confirmed as notification + link only, never a rendering surface for the report itself. Where the actual two-tab artifact lives is not yet decided between two options: **(A)** a persistent, always-updated app; **(B)** a Claude skill invoked on demand, generating the same content structure when triggered from the Slack notification. This decision is deferred to a dedicated architecture discussion, not resolved by Discovery.

**Option B detailed design:** `discovery/PRD/architecture-option-b-claude-skill.md` — covers, specific to that option, the trigger flow, a per-concept access-path mapping (live MCP vs. already-ingested Databricks), a diagram, and pre-flight/failure-handling requirements. Kept out of this table since it only applies if Option B is chosen — the Data Concepts table above stays neutral between A and B.

### **8. Success Metrics (Outcome & ROI)**

*(not started — Design phase)*

---

## ⚙️ [PHASE 3: DEVELOPMENT]

*Focus: Decision backlog and delivery planning.*

### **9. Open Issues**

*(not started — Development phase)*

### **10. Roadmap and Sprints**

*(not started — Development phase)*

---

## 🚀 [PHASE 4: DELIVERY]

*Focus: Sustainability, Governance, and Real ROI.*

### **11. Governance and Access**

*(not started — Delivery phase)*

### **12. Change Management**

*(not started — Delivery phase)*

### **13. Results Capture**

*(not started — Delivery phase)*
