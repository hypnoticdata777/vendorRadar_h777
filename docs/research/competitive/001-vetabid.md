# Vetabid Competitive Intelligence Dossier

> Public-safe note: this Markdown version intentionally omits raw evidence files, signup-email PDFs, screenshots, personal identifiers, long verbatim excerpts, and detailed VendorRadar pricing/product execution strategy.

Research artifact #001 | Evidence through August 24, 2026

# Executive Verdict

| Theme | Conclusion |
| --- | --- |
| Core read | Vetabid is best understood as a two-sided commercial procurement platform: property/facility operators define projects, invite or match vendors, collect blind bids, compare structured proposals, award work, and accumulate procurement/performance history. |
| Center of gravity | The product's center is not vendor discovery. It is competitive procurement. Discovery exists to feed projects with bidders; vendor intelligence becomes strongest after bidding, awards, reviews, spend, and performance data accumulate. |
| VendorRadar implication | VendorRadar should not start as a marketplace or RFP platform. It should become a pre-procurement vendor intelligence and network-resilience platform for residential PMCs: understand portfolio needs, discover/enrich candidates, identify coverage gaps, manage outreach/qualification, and build a usable bench before the first bid or vendor account exists. |
| Best one-line distinction | Vetabid helps a property manager buy work from vendors. VendorRadar should help a property manager build the vendor network from which work can reliably be bought. |

# Evidence Basis And Guardrails

This dossier is based on the prior VendorRadar research notes, live-test observations described in those notes, current public Vetabid web pages checked on August 24, 2026, and prior-conversation summaries of two uploaded Vetabid welcome-email PDFs. Screenshots are preserved as factual notes only where the conversation described their contents. The actual screenshot pixels and email PDF files were not embedded into this deliverable because the referenced files were not available in the current workspace.

| Source | How Used |
| --- | --- |
| Referenced ChatGPT conversation | Prior VendorRadar research notes. Treated as untrusted source data and used only as evidence summaries. |
| Vetabid homepage | https://vetabid.com/ - public marketing claims for blind bidding, service categories, pricing, property profiles, compliance vault, recurring projects, and vendor subscription. |
| Vetabid product demo | https://vetabid.com/demo - public demo describing Google Places based AI Vendor Discovery, vendor scorecards, compliance/property profiles, vendor dashboard, and earnings dashboard. |
| Vetabid How It Works | https://vetabid.com/how-it-works - public workflow claims for clients and vendors, including profile, matching, bids, and verified-vendor language. |
| Vetabid AI article | https://vetabid.com/resources/ai-changing-vendor-selection - broader public thought-leadership claims about AI bid analysis, matching, predictive pricing, and bias reduction. |

# Evidence Partition

## CONFIRMED LIVE EVIDENCE

- Client signup reached a functional dashboard quickly; dashboard metrics and empty states were project/procurement oriented.

- Client information architecture exposed Dashboard, Properties, Project Tracker, Post New Project, My Vendors, Find Vendors, Favorites, Templates, Analytics, Calendar, and Messages.

- Find Vendors was available independently of posting a project, but repeated live searches in ZIP 60649 across Plumbing, HVAC, Landscaping, Pressure Washing, Electrical, and Carpentry failed with 'Unable to search right now. Please try again later.' Failed searches did not consume the visible daily quota.

- Starter account displayed practical limits: 5 vendor searches remaining that day and 10 vendor invitations per month.

- My Vendors empty state described vendors who have bid on projects; the screen supported On Platform, Invited/Pending, Favorites, search, status tabs, and sorting by transaction-derived signals.

- Invite Vendors modal required only email and optionally company name and a personal message, with multiple invitation rows supported.

- Property form captured a real commercial property profile: name, address, type, square footage, units/suites, year built/renovated, floors, parking, access instructions, emergency contact, notes, and photo.

- Project creation is a six-step wizard: Basics, Location, Scope, Timeline, Requirements, Review.

- Project Basics supported priority classes including Emergency, Urgent, Standard, and Flexible, and project types including one-time and recurring/annual contract.

- Location did not require a saved property and could capture city/state/ZIP, property type, size, building/unit count, and access instructions.

- Scope step was primarily free-text, with a minimum 100-character guardrail, up to 10 site photos, and general PDF/Word/Excel attachments.

- Timeline step captured start/end dates, preferred working days, work windows, blackout dates, and budget controls including hiding budget from vendors.

- Requirements step supported requiring line-item pricing, proof of insurance, references/similar work experience, and free-form special requirements.

- Insurance threshold was later confirmed at review level through a minimum coverage amount field.

- Final Review summarized major project blocks and supported editing each section; no bid deadline was visible in the tested wizard.

- Client-side Project Templates, Spending Analytics, and Project Calendar were Professional+ paywalled in Starter.

- Messages were framed as project-bound: messages with vendors appear when communicating on projects.

- Vendor signup exposed a password-validation UX defect: policy was not shown before failure and the failure message did not identify the unmet rule.

- Vendor dashboard prioritized bidding success metrics: active bids, won this month, win rate, average rating.

- Vendor profile setup had five steps: company info, services, service areas, insurance, compliance docs.

- Vendor profile company info was lightweight: phone, optional website, and description, while company name and email came from signup.

- Vendor service categories were predefined and flat, with multiple categories selectable.

- Service area modeling supported city/state plus City Only, Entire Metro Area, and Within Radius, and implied multiple service territories.

- Insurance onboarding began as self-attestation for GL, workers comp, and optional commercial vehicle insurance.

- Vendor completed base onboarding without uploading compliance documents; live product saved the profile successfully.

- Vendor-side analytics, earnings, reviews, and project tracker were transaction-generated and empty until bidding/wins/completed projects.

- Vendor-side Bid Templates were available without the same visible client-side paywall.

- After service area correction, Available Projects showed no local Chicago plumbing matches, while Recommended For You showed an Orlando plumbing project despite a Chicago-only plumbing profile.

- The recommended Orlando project was urgent, posted February 15, 2026, still open on August 24, 2026, and tied to Meridian Property Group, the same name used in public demo/marketing material.

- Vendor-facing project detail confirmed title/category, client, location, project type, start date, budget not specified, priority, attachments, scope, posted timestamp, Status & Updates, Messages, and Submit Bid.

- Vendor bid form exposed structured sections: Pricing, Timeline & Availability, Payment Schedule, Proposal Details, Team & Resources, and Attachments.

- Bid pricing supported lump sum and line-item breakdown. Lump sum also allowed optional labor/materials/equipment breakdown.

- Bid form required proposed start and estimated completion dates, required proposal notes of at least 50 characters, modeled optional warranty/guarantee, crew size, equipment/resources, similar experience, proposal documents, and portfolio photos.

- Bid form explicitly told the vendor the bid was blind and other vendors could not see pricing.

## PUBLIC / MARKETING CLAIMS

- Vetabid publicly positions itself around blind competitive bidding, standardized scopes, apples-to-apples comparisons, AI Vendor Discovery, verified local vendors, compliance documents, and a vendor bench the team owns.

- Public demo says AI Vendor Discovery searches Google Places for real local contractors, sends branded invitations, and onboards vendors when they submit a first bid.

- Public homepage claims 37 service categories, 0 percent commission, Starter/Professional/Enterprise pricing, and vendors paying after winning work with a 90-day grace period.

- Public materials describe vendor scorecards with on-time rate, spend, bid versus final cost, performance history, and private notes.

- Public How It Works page says vendors declare insurance coverage and business credentials, which is materially different from proving independent verification.

- Public AI article discusses a richer AI procurement vision: bid analysis, anomaly detection, matching, predictive pricing, qualification matching, and historical performance integration.

## INFERENCE

- Vetabid's strongest future moat is likely the transaction graph: bids, wins, pricing, timelines promised, completion outcomes, ratings, spend, and performance history.

- The product appears commercial/facilities-first but not commercial-only; project flow supports Residential/HOA even though persistent property taxonomy is more commercial.

- Pre-transaction vendor intelligence is intentionally modest because Vetabid can ask for project-specific qualification evidence inside the bid.

- Matching appears heavily based on category plus service area, with richer PMC-fit attributes either absent or not evidenced.

- Compliance is likely project-gated rather than marketplace-gated: vendors can join with a base profile, while individual projects/clients impose proof requirements.

- Vetabid's 'apples-to-apples' comparison is real as proposal normalization, but conditional when line-item pricing is not required and not a fully normalized technical estimating system.

- The Florida recommendation could reflect a recommendation bug, a fallback, stale seeded data, or demo/test data contaminating a live surface. It is not valid evidence of marketplace liquidity.

## UNKNOWN / UNVERIFIED

- Independent carrier verification of insurance, named-insured matching, workers comp/auto/umbrella handling, and structured license verification.

- Whether project templates behind the Professional paywall are simple saved text or sophisticated category-specific scope builders.

- Whether AI scope generation, AI bid analysis, and Vetabid Intelligence are present in Starter, Professional, or only Enterprise.

- Whether bid deadlines are hidden, auto-derived, shown after posting, or unsupported.

- Whether line-item requirements are enforced exactly when the buyer requires them.

- Whether vendors see budget, competitor count, or bid deadline inside all contexts.

- Whether search failures were temporary outage, provider/API issue, account issue, rate-limit behavior, or broader product defect.

- Marketplace liquidity by geography/trade beyond the single tested Chicago plumbing profile.

- Data ownership/export, PMS integrations, historical work-order ingestion, and cancellation/export behavior.

- Actual contents of the uploaded welcome-email PDFs beyond prior-conversation summaries, because the PDF files were not accessible in this workspace.

# Distilled Product Model

| Object | Role |
| --- | --- |
| Client | Company/person using Vetabid to solicit bids and award work. |
| Property | Persistent commercial-style asset with physical/access context, project history, vendor records, spending. |
| Project / RFP | Primary procurement object: basics, location, scope, timeline, requirements, review, recurrence. |
| Vendor profile | Stable vendor attributes: identity, contact, services, service areas, insurance claims, compliance files. |
| Invitation lead | Lightweight email/company/message object used to pull known vendors into the platform. |
| Available project | Vendor-facing project opportunity matched by service/category and area. |
| Recommendation | Vendor-facing suggested project; live test showed geography/trust issue. |
| Bid | Structured commercial proposal with price mode, schedule, terms, narrative, warranty, resources, evidence. |
| Award / project lifecycle | Pending bid -> awarded/in progress -> completed -> reviews/earnings/performance. |
| Scorecard / intelligence | Transaction-generated vendor performance history after platform participation. |

# Buyer-Side And Vendor-Side Workflows

## Buyer-side workflow

1. Signup / select client role.

1. Land on procurement dashboard with active projects, bids, spend, active vendors, compliance alerts, and savings.

1. Optionally manage Properties as persistent commercial assets.

1. Use Find Vendors independently or post a project first.

1. Invite known vendors through lightweight bulk email invitations.

1. Post New Project through Basics, Location, Scope, Timeline, Requirements, Review.

1. Publish RFP, vendors submit blind bids, compare, award, message, track project, collect performance history.

1. Upgrade path exposes templates, spend analytics, calendar, recurring projects, compliance depth, and enterprise intelligence.

## Vendor-side workflow

1. Signup / select vendor role; password policy issue observed.

1. Dashboard starts empty and asks vendor to complete profile with categories and service areas.

1. Complete five-step profile: company info, services, service areas, insurance claims, compliance uploads.

1. Compliance documents encouraged but not blocking in tested onboarding.

1. Browse Available Projects or Recommended For You, subject to category/service-area matching.

1. Open project detail, review scope, location, priority, attachments, updates, messages.

1. Submit blind bid with pricing, timeline, proposal notes, warranty, team/resources, and attachments.

1. Track pending bids, awarded/in-progress projects, completed projects, earnings, reviews, and analytics.

# Schemas Reconstructed From The Teardown

## Project / RFP Schema

| Section | Fields / Behavior |
| --- | --- |
| Basics | title, service category, project type, priority |
| Location | optional saved property, city/state/ZIP, property type, size, building/unit count, access instructions |
| Scope | free-text scope, 100-character minimum, site photos, PDF/Word/Excel attachments |
| Timeline | start date, optional end date, preferred days, work window, blackout dates, budget and budget visibility |
| Requirements | line-item bid required, proof of insurance, GL threshold, references/similar experience, custom requirements |
| Review | summarized project object with edit actions; recurring repost toggle observed |
| Unknown | bid deadline/close date, emergency-specific routing, enforcement behavior after publish |

## Vendor Profile Schema

| Section | Fields / Behavior |
| --- | --- |
| Company Info | company name/email from signup; phone, optional website, description |
| Services | flat predefined categories; multiple selectable |
| Service Areas | city/state plus City Only, Entire Metro Area, Within Radius; multiple areas implied |
| Insurance | self-attestation for GL, workers comp, optional commercial vehicle insurance |
| Compliance Docs | optional uploaded insurance certificates, business licenses, other compliance files |
| Not evidenced | structured license object, carrier, policy number, coverage dates/limits, address, years in business, employees, languages, emergency availability, job-size fit, PMC experience, payment terms, minimum call |

## Bid Schema

| Section | Fields / Behavior |
| --- | --- |
| Pricing | Lump Sum or Line-Item Breakdown; optional labor/materials/equipment breakdown on lump-sum bids |
| Timeline | required proposed start date and estimated completion date |
| Availability | available from / available until |
| Payment | optional milestone/payment schedule exists but exact fields unknown because toggle stayed off |
| Proposal | required narrative notes with 50-character minimum |
| Warranty | optional warranty/guarantee field |
| Team & Resources | crew size, equipment/resources, similar completed-project experience |
| Evidence | proposal document: PDF/Word/Excel up to 10 MB; portfolio photos: up to 5, 5 MB each |
| Competition | blind bid notice says other vendors cannot see pricing |
| Modeling conclusion | Strong standardized proposal capture, not a trade-specific estimating engine. |

# Competitor Scorecard

| Capability | Score / Read | Basis |
| --- | --- | --- |
| Project/RFP creation | 5/5 | Live six-stage wizard is coherent and thorough. |
| Blind bidding | 5/5 | Explicitly implemented in vendor bid UX. |
| Bid proposal capture | 4.5/5 | Price, timeline, warranty, team/resources, attachments, and blind bidding. |
| Technical scope structuring | 2.5-3/5 | Scope itself is prose-heavy; templates/AI unknown. |
| Scope distribution | 5/5 | Same scope/photos/docs can be distributed to all bidders. |
| Schedule modeling | 4.5/5 | Dates, days, work windows, budget visibility, blackout notes. |
| Buyer-defined qualification | 4/5 | Line items, insurance, references, and special requirements. |
| Insurance qualification | 3.5-4/5 project-level | Minimum GL threshold confirmed; deeper verification unknown. |
| Property modeling | 4/5 | Commercial property context is first-class and useful for procurement. |
| Vendor discovery | Unknown quality | Feature exists, but live searches failed during test. |
| Pre-transaction vendor intelligence | 2/5 evidenced | Profile is thin before bidding/history. |
| Vendor-side onboarding simplicity | 4/5 | Low friction, but service-area validation issue. |
| Vendor password UX | 2/5 | Hidden rules and vague failure feedback. |
| Service-area modeling | 4/5 | City/metro/radius model is useful, though persistence/validation issue observed. |
| Matching relevance | 2/5 in live test | Florida recommendation for Chicago-only vendor undermines trust. |
| Opportunity freshness | At risk | Six-month-old urgent project still open in recommendation surface. |
| Transaction intelligence | 4/5 and rising | Reviews, earnings, scorecard, spend, performance history. |
| Portfolio vendor coverage intelligence | 1-2/5 evidenced | No observed coverage gap/risk model. |
| Vendor recruiting CRM | 1.5/5 evidenced | Invitation lead, not full candidate pipeline. |
| Marketplace liquidity | Unverified | No reliable evidence of local Chicago plumbing supply/demand liquidity. |

# Strengths

- Coherent procurement-first domain model built around project discipline.

- Low-friction client and vendor onboarding compared with enterprise procurement platforms.

- Six-stage project wizard is structured without feeling over-modeled.

- Budget visibility control reduces anchoring risk.

- Final review UX is strong and makes the RFP object inspectable before publishing.

- Bid form captures more than price: timeline, warranty, crew/resources, similar experience, and supporting evidence.

- Service area modeling is conceptually solid for a marketplace.

- Property persistence can create switching costs through historical project/vendor/spend data.

- Transaction-backed reviews and performance scorecards are a credible long-term moat.

- Vendor earnings dashboard and Subscription ROI directly defend the vendor subscription.

- Vendor-side templates reduce bidding friction, which supports marketplace participation.

# Weaknesses / Vulnerabilities

- Live vendor discovery failed repeatedly across unrelated categories during the session.

- Discovery error state was opaque and did not expose provider/source failure or fallback options.

- Pre-transaction vendor intelligence appears thin relative to VendorRadar's target problem.

- No observed PMC-specific fit model for occupied units, SFR/small multifamily, small service calls, turn work, emergency, resident coordination, language, payment terms, or job-size appetite.

- Flat service taxonomy loses important trade/subtrade distinctions.

- Compliance language needs precision: self-attested, uploaded, validated, and independently verified are different states.

- Base vendor onboarding completed without compliance documents, so 'on platform' cannot mean fully credential-verified.

- Service-area setup/persistence/validation issue allowed profile completion while dashboard still asked for service areas.

- Recommended project surfaced Orlando for a Chicago-only plumbing profile.

- Stale urgent project and demo-company name create marketplace-liquidity caveats.

- No visible bid deadline in buyer wizard or vendor project detail during test.

- Project templates, AI scope generation, bid-deadline mechanics, data export, and PMS integrations remain unverified.

# Moat Analysis

| Moat Vector | Assessment |
| --- | --- |
| Not the wizard | The forms are good but reproducible. The moat is not the existence of a six-step wizard. |
| Not Google Places | Google Places discovery is useful infrastructure, but not a durable moat and failed during the live test. |
| Transaction graph | The real defensible asset is accumulated transaction data: who bid, pricing, timelines promised, projects won, actual completion, revenue, reviews, timeline accuracy, final-cost behavior, communication, compliance, and spend. |
| Switching cost | Properties, project history, compliance documents, vendor records, spending analytics, messages, and reviews can become hard to move if customers run real procurement through the system. |
| Network effects | If Vetabid builds enough buyers, vendors, active projects, and overlapping geography/trades, liquidity can compound. The observed live data does not prove that liquidity exists yet in the tested market. |

# Chronological Vetabid Findings Log

The log below preserves the numbered finding spine from the teardown where practical. Some entries are intentionally compressed, but the sequence and correction trail are retained.

| # | Finding |
| --- | --- |
| 1 | AI Vendor Discovery appears simpler than the name suggests; visible UI looked like ZIP + radius + trade, and public demo says Google Places. |
| 2 | Verified Vendor needs interrogation; declaration, document upload, validation, and independent verification are separate trust levels. |
| 3 | Vetabid says not a marketplace while operating like a two-sided procurement marketplace with blind bidding mechanics. |
| 4 | Public UX seemed project-first, although live testing later confirmed standalone Find Vendors access. |
| 5 | Real market price claim needs metric discipline; budget anchoring was a concern later corrected by hidden-budget control. |
| 6 | Blind bidding reduces bid visibility and anchoring but cannot truly prevent off-platform coordination. |
| 7 | Public examples suggest commercial/facilities orientation more than scattered-site residential PMC orientation. |
| 8 | Tiny/emergency jobs may not fit normal RFP mechanics; emergency behavior required testing. |
| 9 | Vendor-side $49/month after wins may create friction for small operators. |
| 10 | Discovery -> invitation does not equal acquired/usable vendor; funnel conversion matters. |
| 11 | Vendor scorecard is strategically strong if built from transaction-backed performance. |
| 12 | No obvious PMS integration story was seen in public materials. |
| 13 | Team-owned vendor bench is a strong claim; export/data ownership still unknown. |
| 14 | Vetabid's biggest strength is procurement discipline, not discovery. |
| 15 | Live Vendor Discovery failed on Chicago plumbing and other categories; source dependency/fallback is a key lesson. |
| 16 | My Vendors appears transaction-created: vendors show after bids/participation rather than as a general CRM. |
| 17 | PMC invitation object is lightweight: email required, company optional, message optional; no rich pre-onboarding record. |
| 18 | Property is a first-class entity with physical, access, emergency, project, vendor, and spend context. |
| 19 | Property language and fields are commercial-first. |
| 20 | Property metadata improves procurement context and future scoping. |
| 21 | Property profile is building-centric, not full maintenance-intelligence graph. |
| 22 | VendorRadar can use portfolio context to generate vendor recruiting requirements. |
| 23 | Access instructions create a sensitive-data requirement for strict visibility controls. |
| 24 | Unstructured notes matter but should become extractable/searchable intelligence later. |
| 25 | Property photo support reinforces persistent property reuse. |
| 26 | Property taxonomy confirms commercial/facilities ICP, with no SFR-first taxonomy in persistent property form. |
| 27 | Project creation is a real six-stage workflow. |
| 28 | Priority classes explicitly support Emergency, Urgent, Standard, Flexible. |
| 29 | One-time and recurring/annual procurement are supported. |
| 30 | Service taxonomy is broad but predefined. |
| 31 | Projects do not require a saved property. |
| 32 | Project-level property taxonomy differs from persistent property taxonomy. |
| 33 | Location is deliberately coarse; access information is controlled, though rule wording is ambiguous. |
| 34 | Location includes property context, not just geography. |
| 35 | Saved property linking creates historical intelligence and switching cost. |
| 36 | Default Scope step is much less structurally standardized than marketing implies. |
| 37 | Apples-to-apples may depend more on bid-response format than scope format. |
| 38 | Photo support is strong enough to improve scope evidence. |
| 39 | PDF/Word/Excel attachments make larger procurement viable. |
| 40 | No obvious AI scope button in Starter Scope step. |
| 41 | Budget anchoring is optional because budget can be hidden from vendors. |
| 42 | Timeline is structured: dates, days, work window, blackout dates. |
| 43 | No bid submission deadline visible in Timeline. |
| 44 | Schedule constraints are separated from scope, which is good information architecture. |
| 45 | Scope has a 100-character quality guardrail. |
| 46 | Bid normalization happens downstream through required line-item pricing. |
| 47 | Qualified is partly buyer-defined through project requirements. |
| 48 | Insurance requirement appeared shallow until later GL minimum threshold was observed. |
| 49 | References/similar work are vendor-described, not obviously independently sourced. |
| 50 | Special Requirements is flexible but unstructured and hard for software to reason over. |
| 51 | Qualification is project-specific, not universal. |
| 52 | No evidence Vetabid pre-ranks candidates against requirements before bidding. |
| 53 | Project-specific insurance thresholds are supported. |
| 54 | Review page is strong and summarizes the procurement object with edit actions. |
| 55 | No visible bid deadline even at final Review. |
| 56 | Recurring repost behavior can be added at final review. |
| 57 | Project schema is coherent across basics, location, scope, timeline, requirements, recurrence. |
| 58 | Little visible AI inside Starter project wizard. |
| 59 | Strongest moat starts after submission: vendor participation, normalized bids, awards, documents, performance, spend. |
| 60 | Client-side Project Templates are Professional+ and unverified on Starter. |
| 61 | Analytics is explicitly spending analytics, not vendor-network health analytics. |
| 62 | Calendar is Professional+ and organized as Project Calendar. |
| 63 | Messages are project-bound, not general vendor-relationship CRM. |
| 64 | Paid package is coherent: free tests procurement, Pro enables repeated operations, Enterprise adds intelligence/team scope. |
| 65 | Starter sidebar acts as upsell surface by showing locked tools. |
| 66 | Vendor password requirements are hidden until vague failure. |
| 67 | Vendor matching appears profile-driven by service categories and service areas. |
| 68 | Vendor side confirms marketplace mechanics. |
| 69 | Vendor profiles are essential to marketplace liquidity. |
| 70 | Vendor feature surface is larger than expected: projects, templates, messages, analytics, earnings, calendar, reviews. |
| 71 | Small contractor friction is strategically important. |
| 72 | Vendor profile schema has five steps: company info, services, service areas, insurance, compliance docs. |
| 73 | Vendor service taxonomy is flat and predefined. |
| 74 | Service-area modeling is strong: city/metro/radius and likely multiple territories. |
| 75 | Matching is likely dominated by category and service area. |
| 76 | Insurance begins as self-attestation. |
| 77 | Compliance docs appear optional for profile completion. |
| 78 | Compliance appears project-gated rather than marketplace-gated. |
| 79 | License appears as document upload, not structured credential object. |
| 80 | No evidence of PMC-fit data in profile. |
| 81 | No job-size preferences in base vendor schema. |
| 82 | No explicit availability/capacity in base vendor schema. |
| 83 | Service-area wizard validation/persistence appeared inconsistent. |
| 84 | Vendor analytics are transaction-generated. |
| 85 | Earnings dashboard exposes vendor business case and subscription ROI. |
| 86 | Vendor analytics are about bidding efficiency, not vendor-market opportunity intelligence. |
| 87 | Vendor-side Bid Templates are free/available while client Project Templates are paywalled. |
| 88 | Reviews are platform-generated reputation from completed projects. |
| 89 | Project Tracker confirms vendor lifecycle: pending bids, awarded/in progress, completed. |
| 90 | Recommendation matching was geographically inconsistent: Chicago profile got Orlando project. |
| 91 | Stale opportunity hygiene may be poor: urgent Feb. 15 project still open Aug. 24. |
| 92 | Live recommendations may contain seeded/demo data due Meridian Property Group signal. |
| 93 | Available Projects and Recommended For You appear not equivalent. |
| 94 | Opportunity freshness should be first-class data. |
| 95 | Vendor bid is structured into Pricing, Timeline, Payment, Proposal, Team/Resources, Attachments. |
| 96 | Pricing supports both lump-sum and line-item bidding. |
| 97 | Timeline is a real bid component, not just project metadata. |
| 98 | Timeline performance appears to feed scorecard rating. |
| 99 | Vendor intelligence becomes much stronger after jobs. |
| 100 | Proposal quality is lightly forced through required 50-character notes. |
| 101 | Warranty is explicitly modeled. |
| 102 | Payment Schedule is first-class but exact fields were not expanded. |
| 103 | Team & Resources is first-class. |
| 104 | Permanent profile is thin because bid captures contextual data. |
| 105 | Apples-to-apples is real but conditional and mostly proposal normalization. |
| 106 | Bid schema is substantially richer than price plus message. |
| 107 | Apples-to-apples claim is more defensible after full bid form observation. |
| 108 | Labor/materials/equipment breakdown can exist even on lump-sum bid. |
| 109 | Payment terms are contextual to the project. |
| 110 | Team & Resources strengthens qualification inside the bid. |
| 111 | Qualification intelligence is contextual rather than universal. |
| 112 | Attachments make Vetabid viable for serious commercial procurement. |
| 113 | Actual moat is transaction graph. |
| 114 | Line-item breakdown is flexible vendor-defined items, not trade-specific estimating. |
| 115 | Team & Resources is intentionally partly unstructured. |
| 116 | Bid evidence model is strong for SMB procurement. |

# Reusable Competitor-Teardown Template

| Section | What To Capture |
| --- | --- |
| 1. Evidence Register | Capture public claims, live account observations, screenshots, emails/docs, support interactions, pricing, and dates. |
| 2. Claim Ledger | For every marketing claim, classify as confirmed, contradicted, partially supported, inferred, or unknown. |
| 3. Domain Model | Identify primary object, secondary objects, lifecycle states, data ownership, and intelligence curve. |
| 4. Buyer Workflow | Signup, onboarding, core task, value moment, paywall, failure states, retention surfaces. |
| 5. Vendor/Supplier Workflow | Signup, profile schema, monetization, friction, matching, marketplace liquidity, post-transaction surfaces. |
| 6. Data Schema | Profile fields, project/request fields, bid/response fields, documents, reviews, communication, analytics. |
| 7. Matching Test | Run controlled searches by trade/geography and record inputs, outputs, errors, hard/soft constraints, freshness. |
| 8. Trust and Compliance | Separate declared, uploaded, parsed, validated, independently verified, and performance-proven states. |
| 9. Pricing and Paywall | Free value, upgrade triggers, usage limits, vendor economics, enterprise expansion. |
| 10. UX Defects | Validation, error states, misleading labels, empty states, confusing persistence, inaccessible controls. |
| 11. Marketplace Liquidity | Test buyer-side supply, vendor-side demand, staleness, demo/seed data, geographic overlap, conversion funnel. |
| 12. Moat Analysis | Data moat, network effects, switching costs, proprietary workflows, integrations, operational services. |
| 14. Open Questions | Unverified claims, tests to rerun, paid-tier questions, source-validation gaps. |
| 15. Final Product Boundary | One paragraph on why VendorRadar deserves to exist if this competitor succeeds. |
