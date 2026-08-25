# VendorRadar Reddit Mining Dossier: Searches 7-10

> Public-safe note: this Markdown version intentionally omits raw evidence files, screenshots, Reddit usernames, identifying anecdotes, long verbatim excerpts, and sensitive pricing/product strategy. The repo is private as of this checkpoint, but this dossier is still written in a clean, shareable research style.

Date: 2026-08-25  
Project: VendorRadar  
Status: Discovery checkpoint after Reddit Searches 7-10  
Canonical artifact: Developer-friendly Markdown for project documentation  

## Executive Summary

Searches 7-10 materially sharpen the VendorRadar thesis.

Searches 1-6 already showed that property-management vendor pain is larger than "find me a contractor." Searches 7-10 complete the first vendor lifecycle pass. They show how vendors are found, how they enter vendor lists, how they become operationally usable, and how their performance either earns more work or creates replacement pressure.

The strongest integrated finding:

```text
VendorRadar should not be a public contractor directory. It should be a private vendor operating layer that helps PM teams know which vendors are usable, compliant, responsive, proven, and appropriate for the current job.
```

The key change is that "vendor quality" is no longer a static reputation score. The evidence points to an event-driven model:

```text
Vendor quality = compliance freshness + PM-fit + dispatch reliability + communication behavior + work-order proof + invoice discipline + recent performance trend.
```

This creates a concrete product spine:

```text
Find -> Qualify -> Approve -> Onboard -> Assign -> Track -> Renew / Reward / Downgrade / Replace
```

Search 7 showed that contractor recommendations are relationship and trust-transfer workflows. Search 8 showed that approved vendor lists are access infrastructure, not guaranteed work. Search 9 showed that onboarding is operational readiness across documents, finance, compliance, and ownership. Search 10 showed that vendor performance must be tracked as a living trail of assignments, compliance, communication, quality, invoices, renewals, and exceptions.

## Research Methodology

The user manually ran Reddit searches, selected result screenshots, opened chosen threads, and pasted the relevant content into the research session. Threads were selected for operational detail rather than title match alone.

Evidence was prioritized when it contained:

- Firsthand operator testimony from property managers, landlords, contractors, maintenance coordinators, board/HOA participants, or procurement workers.
- Concrete workflow details: vendor lists, work orders, approvals, COIs, W-9s, vendor agreements, net terms, invoices, photos, reminders, scorecards, and maintenance ledgers.
- Contradictions between PM needs and vendor incentives.
- Failure modes: slow payment, no-shows, quality decay, expired insurance, unclear ownership, overbearing portals, incomplete proof, owner distrust, and vendor silence.
- Technical product clues: status states, data fields, workflow gates, alert schedules, role ownership, and integration points.

Evidence was discounted when it was promotional, thin, off-topic, unsupported by comments, or not PM-specific.

## Searches Integrated

| Search | Search Phrase | Primary Question | Evidence Strength |
| --- | --- | --- | --- |
| 7 | `property manager contractor recommendations` | How do PMs and landlords find contractor recommendations, and why do vendors struggle to enter those networks? | High |
| 8 | `property management approved vendor list` | What does it mean to be on a vendor list, and how does list status translate into work? | Very high |
| 9 | `vendor onboarding property management` | What makes a vendor operationally ready to receive work and get paid? | Very high |
| 10 | `property manager vendor performance tracking` | How do PMs know whether a vendor remains safe, responsive, and worth assigning? | Very high |

## Search 7: Contractor Recommendations

Search 7 revealed a two-sided matching problem.

Contractors want repeat PM work because one PM relationship can represent many properties and years of jobs. But many contractors experience PM work as low-margin, slow-pay, tenant-scheduling-heavy, and admin-heavy. PMs and landlords want reliable contractors, but they often rely on referrals, Google, supplier recommendations, associations, parent-company vendor lists, or vendors already inside a system.

The central insight:

```text
PM-fit is not the same as contractor quality.
```

A contractor can be technically skilled and still be a poor PM vendor if they dislike small-ticket work, net terms, tenant scheduling, fast turns, work-order software, photos, NTE limits, or professional invoices.

### Key Evidence Patterns

- PMs and landlords commonly use word of mouth, Google, supplier referrals, known local vendors, and company-approved lists.
- Individual PMs may not have authority to add vendors if the parent company controls approved lists.
- Vendors may need references, a portfolio, W-9, COI, insurance documents, and sometimes third-party credentialing before they become usable.
- Cold outreach is saturated. Vendors who bring useful context, compliance knowledge, or local problem awareness stand out more than generic pitches.
- Contractors repeatedly describe PM work as steady but price-sensitive and sometimes slow to pay.
- Small recurring jobs, emergency repair, exterior maintenance, carpet cleaning, turnovers, and overflow work can be better entry points than large speculative projects.
- PMs sometimes prefer one-person shops or small local teams over large companies, but the same small vendors may be least able to tolerate net 30 material float.
- A vendor can break into a network when an incumbent fails to answer, cannot take the job, becomes too expensive, or declines in quality.

### Product Implications

VendorRadar should not treat discovery as a simple search result. It should model the context around a recommendation:

- Who referred the vendor?
- What property type did they serve?
- What trade/category did they perform?
- What work type did they succeed at?
- Were they used as preferred, backup, overflow, emergency, or trial?
- Did they tolerate PM terms?
- Did they reduce or increase PM workload?
- Did they communicate, document, and invoice cleanly?

Suggested data fields:

| Field | Purpose |
| --- | --- |
| `source_type` | Referral, supplier, association, web search, owner suggestion, vendor self-submission, incumbent failure. |
| `relationship_stage` | Prospect, trial, approved, backup, active, preferred, restricted, removed. |
| `pm_fit_notes` | Payment terms, small-job tolerance, tenant coordination, software willingness, documentation quality. |
| `first_job_trigger` | Incumbent failed, overflow, emergency, referral, trial, bid win. |
| `portfolio_fit` | Multifamily, scattered SFR, HOA, commercial, small landlord, condo, hotel/motel, senior living. |

## Search 8: Approved Vendor Lists

Search 8 deepened the gatekeeping layer. "Getting on the vendor list" is not one thing. It may mean being remembered by an onsite manager, accepted by a corporate vendor coordinator, verified in a third-party credentialing system, added to a backup list, entered into accounting, included in a resident perks program, or awarded a recurring contract.

The central insight:

```text
Being on the list is not the same as getting work.
```

Vendor lists are access infrastructure. They make a vendor usable when the PM needs them, but they do not guarantee priority, exclusivity, or volume.

### Key Evidence Patterns

- Vendors often misunderstand the difference between getting approved, getting preferred, and getting assigned.
- Signing a vendor agreement usually means "now you are in the system," not "now you will receive work."
- Some PM companies have closed vendor pools; others like backup vendors because preferred vendors get busy.
- Vendors become valuable when they make the PM's job easier: predictable pricing, quick bids, professional invoices, reachability, reasonable pricing, and low nonsense communication.
- For fast-turn work such as cleanouts or junk removal, PMs value clear price menus or estimates by unit/job type.
- Vendor lists can work as closed pools, call-down lists, rotations, annual contracts, multi-year contracts, backup rosters, or loosely maintained contact lists.
- Third-party credentialing can protect PMs and boards, but it can also deter small local vendors.
- Some vendor categories belong to maintenance supervisors, regional managers, corporate procurement, resident amenity programs, owners, or insurance lists rather than onsite PMs.

### Product Implications

VendorRadar needs more than a boolean `approved` field.

Suggested status model:

| Status | Meaning |
| --- | --- |
| `prospect` | Known candidate, not yet usable. |
| `packet_requested` | PM requested documents or setup info. |
| `pending_compliance` | Documents submitted but not cleared. |
| `approved` | Vendor can be used under some conditions. |
| `backup` | Usable if primary vendor fails, is unavailable, or is out of scope. |
| `preferred` | Favored for a specific category/property/context. |
| `restricted` | Can be used only for certain work or after review. |
| `blocked` | Cannot receive work or payment until issue is resolved. |
| `removed` | No longer eligible due to performance, compliance, cost, or relationship issues. |

Suggested relationship fields:

- `list_model`: closed pool, call-down, rotation, contract, backup, ad hoc.
- `buyer_role`: onsite PM, maintenance supervisor, regional manager, procurement, board, owner, accounting.
- `vendor_list_type`: maintenance dispatch, compliance/payment list, resident amenity list, owner-recommended list, backup list.
- `approval_scope`: portfolio-wide, property-specific, trade-specific, job-specific.
- `known_gate`: W-9, COI, license, ACH, vendor agreement, third-party platform, board waiver.

## Search 9: Vendor Onboarding

Search 9 showed that onboarding is where vendor discovery becomes operational reality. The visible pain is W-9s, COIs, insurance certificates, portals, vendor packets, finance handoffs, and spreadsheets. The deeper pain is ownership.

The central insight:

```text
Vendor onboarding fails when the process lives across email, spreadsheets, memory, finance handoffs, and unclear ownership.
```

Onboarding determines whether a vendor can actually receive work and get paid. A vendor can be capable, known, and desired, but still unusable if insurance is missing, ACH is incomplete, Finance rejects the packet, or nobody owns the renewal process.

### Key Evidence Patterns

- PM staff onboarding can be weak, which matters because vendor workflows depend on internal process discipline.
- Vendor onboarding in adjacent procurement contexts often becomes "email plus Excel" across W-9s, tax forms, bank details, insurance certificates, and Finance review.
- Large-company portals can create excessive burden for small vendors.
- Not every vendor should face the same onboarding depth. A one-time junk removal vendor, HVAC contractor, software vendor, licensed trade, and high-risk contractor have different risk profiles.
- COI tracking is a recurring pain: spreadsheets, manual reminders, missed sorts, absent owners, and expiration-date drift.
- Operators with discipline may solve much of the problem with searchable vendor lists, email folders, master contracts, property-specific billing inboxes, and spreadsheets.
- Strong vendors stand out through promptness, scheduling reliability, photos, clean invoices, realistic ETAs, mistake recovery, and PM-specific awareness.
- Vendor coordinators and maintenance coordinators may be the true workflow owners.

### Product Implications

VendorRadar should support tiered onboarding and clear process ownership.

Suggested onboarding object:

| Field | Purpose |
| --- | --- |
| `risk_tier` | Low, standard, high, emergency-only, restricted. |
| `required_docs` | W-9, COI, workers comp, auto, license, MSA, ACH, references, platform registration. |
| `owner` | Person responsible for completing or reviewing onboarding. |
| `finance_status` | Not started, pending vendor, pending finance, approved, rejected, blocked. |
| `compliance_status` | Current, expiring soon, lapsed, missing, waived, not required. |
| `dispatch_eligibility` | Can work, cannot work, can work only with waiver, can work only for low-risk jobs. |
| `payment_eligibility` | Can pay, hold payment, missing tax/payment docs, owner funds pending. |
| `renewal_schedule` | 90/60/30/14/7-day reminder windows, depending on document type. |

Technical note:

Onboarding should not be a static checklist. It should be a state machine. Each vendor moves through states based on submitted documents, review outcomes, expiration dates, payment setup, and assignment rules.

Example state machine:

```text
prospect
-> invited
-> packet_started
-> packet_submitted
-> compliance_review
-> finance_review
-> approved_for_work
-> active
-> expiring_soon
-> renewal_requested
-> lapsed
-> blocked
-> reapproved
```

## Search 10: Vendor Performance Tracking

Search 10 moved the thesis from onboarding into ongoing operations. It showed that a vendor has to remain usable after they are approved.

The central insight:

```text
Vendor performance is not a single score. It is a trail of dispatch, compliance, communication, work quality, invoice, and renewal events.
```

PMs do not just need to know whether a vendor is "good." They need to know whether the vendor is safe to assign today, for this type of work, at this property, under current insurance, payment, response, and quality conditions.

### Key Evidence Patterns

- COI tracking is often handled with spreadsheets, folders, manual reminders, or one named person.
- One expiry field is too shallow. GL, workers comp, auto, endorsements, licenses, W-9s, and MSAs can have different renewal dates and different eligibility effects.
- Software becomes more valuable when renewals must be chased across multiple staff or expired vendors can still accidentally receive work.
- Operators care about whether a vendor can work and whether a vendor can be paid.
- Cleaning-vendor discussions show performance decay: vendors may perform well early, then decline as small details slip, crews overextend, or quality standards drift.
- PMs want proof and updates, but too much vendor update burden can backfire.
- For small jobs, PMs may only want accept, complete, photos, invoice. For larger jobs, status updates and before/after photos are more reasonable.
- Owners want visibility into maintenance charges, disbursements, invoices, vendor names, photos, tenant satisfaction, and repair proof.
- Cross-industry procurement patterns point to scorecards based on on-time delivery, quality, cost, support, risk, and corrective actions.

### Product Implications

VendorRadar should generate vendor performance from operational evidence before asking users to manually rate vendors.

Suggested event model:

| Event | Description |
| --- | --- |
| `vendor_assigned` | Vendor selected for a work order or job. |
| `work_order_accepted` | Vendor accepted or acknowledged dispatch. |
| `schedule_confirmed` | Vendor provided appointment or ETA. |
| `no_response` | Vendor failed to answer within expected window. |
| `arrival_confirmed` | Vendor arrived or checked in. |
| `tenant_access_failed` | Job blocked by tenant/property access. |
| `approval_requested` | Vendor requested owner/PM approval above threshold. |
| `photos_submitted` | Vendor submitted proof or before/after photos. |
| `job_completed` | Work marked complete. |
| `invoice_received` | Invoice submitted. |
| `invoice_exception` | Invoice mismatch, missing detail, wrong property, or unclear charge. |
| `callback_required` | Repeat issue or rework after completion. |
| `complaint_logged` | Tenant, owner, board, or PM complaint. |
| `compliance_expiring` | Document approaching expiration. |
| `compliance_lapsed` | Required document expired. |
| `payment_blocked` | Vendor cannot be paid because required setup/compliance is missing. |

Suggested scorecard:

| Dimension | Possible Inputs |
| --- | --- |
| Responsiveness | Dispatch acknowledgment time, no-response count, reminder count. |
| Scheduling reliability | On-time arrival, reschedules, no-shows. |
| Completion reliability | Completion rate, overdue work orders, abandoned jobs. |
| Quality | Rework, callbacks, tenant/owner complaints, PM notes. |
| Documentation | Photos, service notes, diagnosis clarity, invoice detail. |
| Cost discipline | Bid vs final, NTE adherence, market spot-checks, outlier charges. |
| Compliance freshness | COI/license/W-9/MSA status and renewal response. |
| PM burden | Number of touches required per job, clarification loops, invoice corrections. |

Technical note:

Recent performance should carry more weight than old performance. A vendor who performed well for four years but failed the last three move-ins should not look identical to an actively reliable vendor.

Example trend logic:

```text
vendor_score = weighted_recent_events + compliance_gate + risk_adjustment
recent_90_days > trailing_12_months > historical_average
blocked_compliance overrides positive performance score
```

## Cross-Search Synthesis

Searches 7-10 form a complete first-pass lifecycle:

```text
Vendor discovery
-> trust transfer
-> vendor-list entry
-> compliance/payment setup
-> dispatch eligibility
-> work-order execution
-> evidence and invoice
-> performance memory
-> renewal, reward, downgrade, or replacement
```

The important shift is from "Who do I call?" to "Who can I trust in this specific operating context?"

### Synthesis 1: VendorRadar Should Model Eligibility, Not Just Identity

The core PM question is not just:

```text
Who are the HVAC vendors?
```

It is:

```text
Which HVAC vendor can be assigned today, in this area, for this property type, with valid coverage, acceptable payment terms, recent good performance, and a tolerable coordination burden?
```

### Synthesis 2: Approved, Preferred, And Available Are Different States

Approved means the vendor is allowed into the system. Preferred means the PM chooses them first in a context. Available means the vendor can take the work now. Compliant means the vendor is safe/eligible under current requirements. These should not be collapsed into one status.

### Synthesis 3: Vendor Facts Expire

Compliance, insurance, availability, contacts, pricing, service area, quality, and PM preference all decay. A vendor profile needs freshness dates and reminder logic.

### Synthesis 4: PM Burden Is A Hidden Cost

A cheap vendor can become expensive if they create calls, tenant complaints, invoice corrections, owner disputes, missing photos, unclear diagnoses, or scheduling chaos.

### Synthesis 5: Vendor Portals Are Risky If They Add Work

Vendors may resist extra portals, update links, or repeated manual steps. The minimum viable product should capture useful signals with the least vendor burden possible.

### Synthesis 6: The Best Data Comes From Work-Order Exhaust

Ratings and notes are useful, but timestamps, dispatches, acceptances, photos, invoices, exceptions, compliance dates, and callback events are stronger signals.

## Proposed VendorRadar Technical Model

This is not a full spec. It is a research-derived technical model.

### Core Entities

| Entity | Description |
| --- | --- |
| `Vendor` | Business or individual service provider. |
| `VendorContact` | People, roles, phone/email, escalation path. |
| `ServiceCategory` | Trade or service type: HVAC, plumbing, cleaning, junk removal, roofing, locksmith, etc. |
| `Property` | Building/unit/portfolio context where vendors are used. |
| `VendorRelationship` | PM-specific relationship state: approved, backup, preferred, restricted, removed. |
| `ComplianceDocument` | COI, workers comp, auto, license, W-9, MSA, endorsement, etc. |
| `WorkOrder` | Maintenance/job object connected to vendor, property, issue, tenant/owner context, approvals, proof, and invoice. |
| `VendorEvent` | Time-stamped behavioral/compliance/payment event. |
| `Invoice` | Vendor charge with property, work order, line-item, approval, and exception data. |
| `Scorecard` | Derived summary of vendor performance by context and period. |

### Key Status Enums

Vendor relationship:

```text
prospect | invited | pending_packet | pending_review | approved | backup | preferred | restricted | blocked | removed
```

Compliance:

```text
not_required | missing | submitted | under_review | current | expiring_soon | lapsed | waived | rejected
```

Dispatch eligibility:

```text
can_work | can_work_with_waiver | emergency_only | blocked_by_compliance | blocked_by_payment | blocked_by_performance | inactive
```

Payment eligibility:

```text
can_pay | missing_w9 | missing_ach | owner_funds_pending | compliance_hold | invoice_exception | manual_review
```

### Operational Gates

VendorRadar should be able to answer:

- Can this vendor receive a work order?
- Can this vendor be paid?
- Is this vendor approved for this property, region, or trade?
- Is the vendor blocked only for one document or blocked everywhere?
- Is the vendor appropriate for emergency work?
- Is the vendor's recent performance declining?
- Has the vendor been paid without a valid compliance record?
- Is this vendor missing from the official list but appearing in invoices?

### Alert Logic

High-value alerts:

- COI expires in 60/30/14/7 days.
- Workers comp expired.
- Vendor assigned while required document is missing.
- Vendor paid without valid compliance record.
- Vendor no-response after dispatch.
- Work order open too long without update.
- Invoice received without closeout proof.
- Repeat issue after completion.
- Vendor quality trend declining.
- Preferred vendor not used recently.
- Off-system vendor detected in invoice/payment history.

### MVP Wedge

The narrowest useful wedge appears to be:

```text
Private vendor register + compliance freshness + dispatch/payment eligibility + lightweight performance memory.
```

This wedge is stronger than a generic marketplace because it:

- Fits PM workflow.
- Reduces risk.
- Creates immediate utility from existing vendor lists.
- Avoids depending on a public two-sided marketplace from day one.
- Can import spreadsheets and improve them with reminders, status, and evidence.

## Competitive Connection

The competitive research already shows that this space has adjacent players:

- Vetabid: project/RFP and bid comparison orientation.
- UnitDispatch: concierge/vendor sourcing and dispatch orientation.
- VendorPM: enterprise vendor procurement, compliance, RFX, and contract management orientation.

Searches 7-10 suggest VendorRadar's sharper angle should be:

```text
Vendor intelligence for PM operations: knowing who is usable, why, and whether their recent behavior supports another assignment.
```

This is distinct from:

- only sourcing new vendors,
- only credentialing vendors,
- only running bids,
- only tracking contracts,
- only storing contacts,
- or only showing public reviews.

## Risks And Counter-Evidence

Important things this research does not prove:

- That every PM has this pain.
- That Reddit represents the broader market.
- That PMs will pay for a separate tool.
- That vendors will cooperate with another workflow.
- That AppFolio, Buildium, Yardi, PropertyMeld, VendorPM, NetVendor, VIVE, Jones, MyCOI, Billy, BCS, or similar tools do not already solve enough of the problem for specific segments.
- That a lightweight tool beats an organized spreadsheet for small operators.
- That compliance automation alone is a large enough wedge.
- That performance scoring can be fair without context from bad tenants, bad scopes, owner delays, poor work-order details, or property condition.

Counter-evidence already observed:

- Some operators say vendor management is basic organization, not a product problem.
- Small portfolios may work fine with spreadsheets and a single clear owner.
- PMs may reject vendor-facing update requirements if they add friction.
- Some PMS or vendor-management suites already include compliance, onboarding, invoicing, and vendor modules.
- Some PMs view owner verification as micromanagement.
- Vendors may reject PM work if payment terms and admin burden are unattractive.

## Open Questions

1. Which PM segment has the strongest willingness to pay: small residential, scattered-site SFR, multifamily, HOA/condo, commercial, mixed portfolio, or self-managing investors?
2. Who is the buyer: owner/operator, maintenance coordinator, regional manager, accounting/compliance, HOA board, asset manager, or vendor?
3. How many vendors or documents create the breaking point where spreadsheets fail?
4. What workflows do existing PM software products already solve well?
5. Do PMs care more about compliance freshness, performance memory, owner auditability, or vendor discovery?
6. Can VendorRadar create value without requiring vendors to log into another portal?
7. What data can be imported from spreadsheets, email, invoices, and PMS exports?
8. How should scorecards adjust for job type, urgency, tenant access, owner approval delay, and property condition?
9. Can "can work / can pay" become the simplest wedge?
10. How often do PMs use vendors who are not actually in the official vendor register?

## Next Research Channel

The prior Searches 1-6 dossier ended with this instruction:

```text
The next research stage should focus on performance tracking, then move to another forum to reduce Reddit bias and test whether the same patterns appear in different professional communities.
```

Search 10 completed the performance-tracking pass. The next step should therefore leave Reddit.

The documentation does not name one exact forum as the next destination. It does repeatedly mention professional channels and association-style contexts such as apartment associations, BOMA, IREM, NARPM, local real estate associations, LinkedIn, vendor events, and property-management communities.

Recommended next channel:

```text
BiggerPockets forums or another investor/property-management community where owners, landlords, and small operators discuss vendors and maintenance.
```

Current spot-check examples:

- BiggerPockets has a recent maintenance-scaling thread where a small landlord describes contractor photos, tenant requests, spreadsheets, folders, and scattered work history as the operational pain.
- BiggerPockets has owner/PM oversight threads where repairs, photos, contractor updates, maintenance charges, and the line between visibility and micromanagement are central concerns.
- BiggerPockets has property-manager screening threads that discuss PM maintenance processes, contractor licensing/insurance, invoice markup, repair documentation, spending limits, and owner reporting.

Why this should be next:

- It reduces Reddit-only bias.
- It can test owner/operator language, not only PM staff language.
- It may reveal how self-managing landlords and small portfolio owners track vendors before they become formal PM companies.
- It can stress-test whether VendorRadar is a PM-only tool or a broader landlord/vendor-ops tool.

Suggested next searches outside Reddit:

```text
BiggerPockets property manager vendor recommendations
BiggerPockets contractor property manager maintenance
BiggerPockets property management maintenance vendors
BiggerPockets landlord contractor reliability
BiggerPockets property manager maintenance markup vendor
BiggerPockets approved vendor list property management
```

Alternative professional channels to check after that:

- LinkedIn posts/comments from property managers and maintenance coordinators.
- BOMA or apartment-association vendor/event discussions.
- NARPM-adjacent public resources or community discussions.
- Property-management software review comments mentioning vendor workflow.
- Vendor-side forums for trades that work with PMs.

## Current Position

The evidence is now strong enough to justify a product discovery brief and a sharper MVP hypothesis. It is still not strong enough to build the final product without external validation beyond Reddit.

The best current VendorRadar hypothesis:

```text
Property managers do not primarily need another place to find contractors. They need a private, current, evidence-backed way to know which vendors are usable, compliant, responsive, and appropriate for each job.
```

The next research stage should validate that hypothesis in non-Reddit communities and compare it directly against existing PM software/vendor-compliance tools.
