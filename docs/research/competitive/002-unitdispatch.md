# UnitDispatch Competitive Teardown Dossier

> Public-safe note: this Markdown version intentionally omits raw evidence files, signup-email PDFs, screenshots, personal identifiers, long verbatim excerpts, and detailed VendorRadar pricing/product execution strategy.

Vendor sourcing, bid comparison, and vendor performance sidecar for property maintenance

| Field | Detail |
| --- | --- |
| Prepared for | VendorRadar strategy and product development |
| Prepared on | August 24, 2026 |
| Evidence basis | Prior research notes, user-provided screenshot text, and public UnitDispatch pages available during review |
| Analysis posture | Observed facts are separated from inferences and VendorRadar implications |
| Competitor stage classification | Early demo / concierge pilot, conceptually relevant; operating maturity unconfirmed |

| Bottom line UnitDispatch is the closest competitor examined so far because it attacks the same messy vendor-sourcing pain for small and mid-sized property operators. Its center of gravity is reactive job-to-vendor sourcing and bid comparison. VendorRadar's strongest available white space is upstream: portfolio-level vendor coverage, market intelligence, redundancy planning, and proactive vendor recruitment before a work order exists. |
| --- |

# Evidence Discipline

This dossier separates what was observed from what is inferred. Treat UnitDispatch's public metrics and scores as product-design evidence, not validated commercial traction, unless independently verified.

| Evidence label | Meaning |
| --- | --- |
| Observed fact | Visible copy, screen text, pricing, navigation, metric labels, forms, statuses, disclaimers, and workflow language. |
| Inference | A reasoned conclusion from multiple observed facts, such as concierge operating model or bid-request-centered architecture. |
| VendorRadar implication | A strategic or product requirement that VendorRadar should consider because of the observed pattern. |
| Open question | A claim that needs more proof before it can be used as a planning assumption. |

# Executive Summary

- Category: property-maintenance vendor sourcing and bid-comparison sidecar.

- ICP: small landlords and growing property managers, explicitly framed around 3-500 doors with a 50-250 door pilot sweet spot.

- Core loop: create bid request, source/invite vendors, compare bids, select vendor, export summary back to the existing PM system, and retain vendor performance memory.

- Business model: subscriptions for landlords, PM teams, and contractors; optional 5% success fee and Stripe Connect are described as later-stage.

- Maturity: the site is labeled Demo, references a Cleveland pilot, exposes multiple personas publicly, and states that concierge workflows fill gaps before automation and integrations are live.

- Strategic threat: high conceptual overlap, moderate strategic threat, lower immediate execution threat based on visible demo/manual operations.

- VendorRadar opportunity: own vendor-market intelligence, portfolio coverage requirements, trade/geography redundancy, source confidence, and proactive candidate discovery.

# Product Positioning

Observed: UnitDispatch positions itself as a vendor sourcing layer for AppFolio, Buildium, and spreadsheets. It promises reliable property maintenance vendors, bid comparison, and vendor performance tracking without replacing existing property management software.

Observed: It explicitly says it does not replace rent collection, leases, owner statements, full accounting, or tenant portals.

Inference: The product is intentionally a sidecar, not a system of record. This lowers adoption friction and lets the company monetize a narrow pain without challenging entrenched PMS platforms.

VendorRadar implication: Do not use 'we do not replace AppFolio or Buildium' as a unique differentiator. UnitDispatch already owns that language. VendorRadar needs a sharper upstream thesis.

# ICP

| Segment | Evidence | Status |
| --- | --- | --- |
| Small landlords | Free and $49/month tiers for organizing a small vendor bench and bid requests. | Observed |
| Growing PM teams | $149/month Growth tier; up to 250 doors; team members, imports, private notes, analytics. | Observed |
| Larger local portfolios | $299/month Pro tier; larger portfolios, custom workflows, verification dashboard, priority support, integration-lite workflows. | Observed |
| Contractors | $39/month Contractor Pro; claimed profile, verified badge, bid alerts, performance dashboard, recurring PM opportunities. | Observed |
| Pilot geography | Cleveland-area PM pilot context, with sample properties in Cleveland, Lakewood, Parma, Strongsville, Shaker Heights, Avon Lake, North Olmsted, and Tremont. | Observed |

# Business Model And Pricing

| Plan | Price | Observed feature intent |
| --- | --- | --- |
| Free Landlord | Free | 1 user, limited bid requests, manually add vendors, basic bid comparison. |
| Landlord Pro | $49/month | Up to 10 properties, unlimited bid requests, preferred vendor list, PDF/CSV exports, vendor performance tracking. |
| Property Manager Growth | $149/month | Up to 250 doors, team members, vendor import, advanced bid comparison, private notes, performance analytics. |
| Property Manager Pro | $299/month | Larger portfolios, custom vendor workflows, verification dashboard, priority support, integration-lite workflows. |
| Contractor Pro | $39/month | Claimed profile, verified badge, priority bid alerts, performance dashboard, recurring maintenance opportunities. |
| Platform fee | Optional 5% later | Stated as later-stage; Stripe Connect structured for completed-job fees and contractor payouts. |

Inference: UnitDispatch is testing whether PM-side workflow value plus contractor-side recurring-demand access can support two-sided subscription economics before transaction fees are live.

Risk: Contractor-paid visibility can create trust tension if paid status influences ranking, alerts, or perceived recommendation quality.

# Full Workflow

1. Existing work order or maintenance need appears in AppFolio, Buildium, Rent Manager, Propertyware, spreadsheet, or manual process.

1. PM creates a UnitDispatch bid request with property, unit, trade, urgency, photos/access notes, external work order ID, budget range, and target date.

1. UnitDispatch sources or invites vendors across preferred vendors and new vendors.

1. Contractors submit lightweight bids with price, start/completion dates, warranty, notes, and materials-included signal.

1. PM compares bids, selects a vendor, stores status, and exports a clean summary back to the current system.

1. The platform accumulates response history, quote history, completion history, private PM notes, preferred status, verification state, and performance scores.

Inference: The primary object is the bid request, not the portfolio. UnitDispatch starts when a job exists; VendorRadar can start when a portfolio's vendor network is under-covered.

# PM-Side Features

| Feature area | Observed behavior |
| --- | --- |
| Dashboard | Open bid requests, quotes received, response rate, vendors contacted, estimated savings, preferred vendors, pending verifications, export-ready summaries. |
| Bid request intake | Property/unit, trade/job/urgency, photos/access notes, external ID/current system, budget range, target date. |
| Bid table | Request, type, system, vendor count, bid count, budget, status. |
| Export workflow | Export bid comparison as PDF, work order summary as CSV, copy summary to clipboard. |
| Vendor bench | Preferred vendors, verification gaps, private PM notes, last-used dates, preferred relationship context. |
| Performance panel | Reliability and quote accuracy by vendor; source and claim status displayed. |
| Property context | Properties and unit counts stored only enough to route vendor requests and export useful summaries. |

# Vendor-Side Features

- Contractor portal is positioned as a lighter workflow for vendors who want repeat property work rather than generic leads.

- Profile signals include verified profile, emergency readiness, priority job alerts, license verified, insurance verified, reliability score, completed jobs, typical job size, repeat PM rating, and pre-bid fit score.

- The visible contractor example, Cleveland Pipe Rescue, shows response in 28 minutes, reliability score 94, 318 completed jobs, $165 typical job size, 9.4 repeat PM rating, and pre-bid fit score 87.

- Bid request cards show trade, urgency, status, and budget ranges. The bid form asks for price, start date, completion date, warranty, bid notes, and whether materials are included.

- Contractor dashboard preview shows monthly earnings, completed jobs, profile completion checklist, reliability dashboard, and completed-job-only reviews.

Inference: UnitDispatch's vendor-side promise is anti-lead-marketplace: get recurring PM work, build operational reputation, and respond quickly to qualified requests.

# Admin And Concierge Operations

Observed: The Admin page says it supports concierge workflow for the first 5-10 Cleveland PM pilots: create requests, add vendors, send invite links, track responses, and verify documents manually.

Observed: Pilot Mode keeps customers successful before email automation, PDF generation, and AppFolio or Buildium integrations are live.

Observed: Admin operations include manually creating bid requests, manually adding vendors, sending invite links, tracking responses, marking bids received, exporting comparisons, approving contractors, marking license/insurance verified, resolving disputes, and suspending contractors.

Inference: The software is likely an operational wrapper around human sourcing, verification, and marketplace-management work during pilot validation.

VendorRadar implication: manual validation may be useful before building expensive discovery infrastructure.

# Vendor Acquisition Paths

| Path | Evidence | Confidence |
| --- | --- | --- |
| Referral | Observed in unclaimed leads and vendor source examples. | High |
| Existing vendor | Observed as a vendor source and PM relationship path. | High |
| Google / Google Places Lead | Observed in Admin page source examples and teardown notes. | High |
| Admin imported | Observed in unclaimed leads. | High |
| Contractor self-signup | Observed as a source type. | High |
| Association | Observed in performance/source examples in the dashboard teardown. | Medium |
| Manual directory import | Recorded in teardown findings as a source path. | Medium |
| Autonomous continuous market scan | No visible evidence. | Low / not observed |

Inference: UnitDispatch is input-driven: vendors enter through human action, imports, referrals, Google enrichment, or self-signup. It does not visibly behave like an always-on market discovery engine.

# Scoring And Reputation Model

- Observed score labels include Reliability, Vendor Fit Score, Pre-bid Fit Score, Quote Accuracy, Repeat PM Rating, response time, completed jobs, and completed-job-only reviews.

- Reliability is described as based on completed-job reviews, response time, and repeat property manager feedback.

- The dashboard frames vendor reliability as a workflow, not a star rating, with reliability and quote accuracy shown as separate dimensions.

- Teardown notes recorded event-style score adjustments such as no-show penalty, bid-submitted improvement, and completed-job improvement.

Inference: The scoring model appears heuristic and event-driven in the demo, not proven predictive intelligence.

Open question: Exact formulas, weightings, recency treatment, dispute handling, and whether paid Contractor Pro affects visibility remain unknown.

VendorRadar implication: Use decomposed, explainable scores. Distinguish responsiveness, quote accuracy, completion reliability, compliance confidence, job-size fit, emergency fit, and PMC-specific relationship quality.

# Integrations

| System / path | Observed integration posture |
| --- | --- |
| AppFolio | Named in positioning and bid request/system examples; live integration explicitly not yet available in pilot text. |
| Buildium | Named in positioning and examples; live integration explicitly not yet available in pilot text. |
| Rent Manager | Named as compatible current workflow/source system. |
| Propertyware | Named as compatible current workflow/source system. |
| Spreadsheets | Named repeatedly; CSV export and spreadsheet-safe summaries are key fallback path. |
| Clipboard | Copy summary to clipboard for AppFolio, Buildium, email, or internal notes. |
| PDF | Export bid comparison as PDF; admin text says PDF generation not live yet, so treat as demo/future workflow. |

Strategic read: UnitDispatch's integration philosophy is interoperability before integration: source-system label, external ID, export, and clipboard first; native PMS integration later.

# Data Model Clues

| Object | Likely fields / relationships |
| --- | --- |
| Organization | PM team, users, private notes, preferred-vendor relationships, source system context. |
| Property | Name, address, unit count, source system, external IDs; deliberately thin context. |
| Bid request | Property/unit, trade, job type, urgency, budget, vendors contacted, bids, status, source system, external ID. |
| Vendor record | Name, trade, service areas, source, claim status, approval status, verification status, minimum/job-size signal, reliability, quote accuracy. |
| Vendor account | Claimed contractor profile, verification docs, bid alerts, performance dashboard, subscription plan. |
| Org-vendor relationship | Preferred status, private PM notes, repeat-hire history, last-used date, conditional preferences. |
| Verification | License, insurance, municipal registration, COI expiration, optional W-9, optional bond, reviewer/date/notes. |
| Performance event | Bid submitted, completed job, no-show, dispute, response time, quote-vs-final cost. |
| Export summary | PDF, CSV, clipboard content mapped back to current PM system. |

Key architecture harvest: Vendor record and vendor account must remain separate. A vendor can exist as a discovered, unclaimed market entity before the contractor joins.

# Strengths

- Clear, right-sized positioning between messy referrals and heavy enterprise credentialing.

- Strong sidecar posture: keep the PMS as system of record.

- Real understanding of PM vendor memory: private notes, preferred vendors, response history, repeat-hire history.

- Unclaimed vendor model supports messy real-world contractors before they sign up.

- Provenance/source labels are first-class enough to guide trust and workflow.

- Completed-job reviews and quote accuracy are more operationally relevant than generic star ratings.


- Contractor portal gives supply-side users a reason to care: recurring PM work and reputation tied to completed jobs.

- Export fallback ladder is practical for early adoption.

# Weaknesses And Risks

- Visible maturity is demo/pilot, not established SaaS: demo labels, public role switching, seeded data, and explicit concierge language.

- Major automation and integrations are described as not live yet: email automation, PDF generation, AppFolio, and Buildium integrations.

- Scoring formulas and savings methodology are unclear; 1% response rate conflicts with 40 quotes from 106 vendors unless definitions differ.

- Manual verification and admin flags can create trust theater if presented too strongly.

- No visible portfolio coverage intelligence, trade redundancy analysis, ZIP-level gap analysis, market map, or proactive vendor recruiting plan.

- Vendor-paid visibility can create recommendation-trust risks.

- Concierge operations may be labor-intensive and hard to scale without automation.

- Dispute and suspension workflows imply real marketplace trust burdens that require operational capacity.

# UX And Product Observations

- The public demo exposes Home, Dashboard, New bid request, Vendors, Pricing, Contractor, Admin, Switch role, and Alerts in one environment. This is useful for investor/demo storytelling but weakens the feel of a production SaaS.

- The PM dashboard is operationally legible: open work, quotes, vendors contacted, export-ready summaries, preferred vendors, pending verification, and properties all map to real PM work.

- The contractor flow is lighter than a full procurement tool and likely better suited to routine repairs and emergency maintenance.

- The language is unusually clear for a pilot: it names what it replaces, what it does not replace, and where manual workflows still exist.

- The product uses strong domain nouns: vendor bench, completed-job reviews, quote accuracy, preferred vendors, unclaimed leads, integration-lite, and vendor performance memory.

# Evidence Of Demo / Pilot Status

| Signal | Evidence | Status |
| --- | --- | --- |
| Demo label | Site and navigation visibly labeled Demo. | Observed |
| Cleveland pilot | Homepage and admin contexts reference Cleveland pilot properties and PM orgs. | Observed |
| Pilot PM orgs | Homepage shows 5 pilot PM orgs and 30 vendors in bench. | Observed |
| Concierge operations | Admin page says first 5-10 Cleveland PM pilots use concierge workflow. | Observed |
| Automation gaps | Admin page says email automation, PDF generation, AppFolio and Buildium integrations are not live yet. | Observed |
| Seeded context | Bid request page says app contains 15 legacy maintenance jobs plus new pilot workflow. | Observed |
| Public multi-persona nav | PM, contractor, admin, and switch-role surfaces visible publicly. | Observed |
| Verification disclaimer | Verification support is not a guarantee; PMs remain responsible for selection. | Observed |
| Patterned demo data | Teardown noted repeated scores, sequential-looking data, and demo buttons. | Observed in conversation |

# Threat Assessment

| Dimension | Rating | Rationale |
| --- | --- | --- |
| Conceptual overlap | High | Same PM vendor-sourcing pain, same sidecar logic, similar ICP, vendor bench, private notes, unclaimed records. |
| Near-term product threat | Low to moderate | Visible demo/pilot state, manual workflows, integrations not live. |
| Strategic learning threat | High | They validate many of the same problem assumptions and could evolve upstream. |
| Pricing validation | Medium | $149-$299 PM tiers suggest belief in paid operational value, but traction unverified. |
| Data moat threat | Medium later | If they accumulate completed-job, quote accuracy, and repeat PM feedback data, they can build proprietary performance intelligence. |
| VendorRadar differentiation room | High | No strong evidence of portfolio coverage intelligence, redundancy analysis, market maps, or continuous discovery. |

Overall: Moderate threat now; potentially serious later if UnitDispatch automates sourcing, deepens scoring, and moves upstream from bid requests to portfolio network planning.

# Repeatable Competitor Analysis Pattern

| Lens | Question |
| --- | --- |
| 1. Product center of gravity | What object drives the product: portfolio, work order, bid, vendor, compliance record, transaction? |
| 2. ICP and urgency | Who is it for, what scale, what pain, what buying moment? |
| 3. Workflow trigger | Does the product start before the job, at the work order, during bidding, after completion, or at compliance renewal? |
| 4. Data model clues | Which nouns recur in the UI and what states do they expose? |
| 5. Automation boundary | What is software-driven, manual, demo-only, or future-roadmap? |
| 6. Trust model | What does verified mean, who is responsible, and what disclaimers exist? |
| 7. Monetization tension | Who pays, what incentives are created, and could payment distort trust? |
| 8. White space | Which valuable customer questions are not answered by the competitor's current center of gravity? |

# Source Notes

- Prior VendorRadar research notes.

- Public UnitDispatch homepage reviewed: https://www.useunitdispatch.com/

- Public pricing page reviewed: https://www.useunitdispatch.com/pricing

- Public bid request page reviewed: https://www.useunitdispatch.com/bid-requests/new

- Public verification disclaimer reviewed: https://www.useunitdispatch.com/verification-disclaimer

- Dashboard, contractor, admin, and vendor details are primarily based on user-provided screenshot text in the referenced conversation.

- This dossier should be refreshed if UnitDispatch changes from demo/pilot posture to a production SaaS with live integrations, verified customer traction, or automated discovery.
