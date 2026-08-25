# VendorRadar Reddit Mining Dossier: Searches 1-6

> Public-safe note: this Markdown version intentionally omits raw evidence files, signup-email PDFs, screenshots, personal identifiers, long verbatim excerpts, and detailed VendorRadar pricing/product execution strategy.

Date: 2026-08-24  
Project: VendorRadar  
Status: Discovery checkpoint before Search 7  
Canonical artifact: Developer-friendly Markdown for project documentation  

## Executive Summary

Across the first six Reddit mining searches, the evidence increasingly points away from a simple "contractor directory" thesis and toward a more complex vendor intelligence and operations problem.

The strongest recurring pattern is that property managers do not merely need names of vendors. They need access to vendors who are qualified, responsive, available, compliant enough for the job, economically willing to accept property-management work, and trustworthy in the specific operational context where the job appears.

The evidence also shows that "vendor quality" is multidimensional. A vendor can be technically skilled but poor at reports, photos, communication, invoices, scheduling, tenant interaction, or compliance. In property management, those administrative and behavioral capabilities are part of the service. A plumber who fixes the pipe but creates five follow-up calls, no service report, a vague invoice, and an owner dispute is not simply "good but disorganized." They may be expensive to manage.

The research so far supports four big conclusions:

1. Vendor management is not one problem. It includes sourcing, qualification, compliance, dispatch, access, work-order integrity, approvals, evidence of completion, invoicing, payment, owner trust, and performance history.
2. Compliance is both a risk control and a supply constraint. Requirements such as COIs, W-9s, licenses, third-party credentialing, insurance limits, renewals, and payment gating can protect a PM or HOA, but can also drive away good small vendors or reduce competition.
3. The real vendor lifecycle is dynamic. Vendors move from prospect to credentialed, approved, trialed, active, preferred, backup, restricted, or removed. "On the vendor list" is not one operational state.
4. Trade type matters. Search 6 showed that plumbing changes the problem because of urgency, diagnostic uncertainty, damage risk, after-hours pricing, authorization, access, and cost attribution.

The current evidence-backed working hypothesis is:

> VendorRadar may be more valuable as a vendor intelligence and operations layer than as a generic marketplace. The core value may be helping PMs know which vendors are usable, proven, compliant, available, appropriate for the current job, and low-friction to coordinate.

This remains discovery, not product design. The evidence is promising but not yet sufficient to choose an ICP, feature set, pricing model, or go-to-market motion.

## Should This Go In The GitHub Repo?

Yes, but selectively.

Commit a cleaned, developer-friendly research artifact like this dossier to the VendorRadar repo. It should live somewhere like:

```text
docs/research/reddit-mining/searches-001-006-vendor-operations-dossier.md
```

Recommended to commit:

- Executive summary and cross-search synthesis.
- Search-by-search logs and search terms.
- Evidence-backed hypotheses.
- Taxonomy/glossary.
- Vendor lifecycle model.
- Contradictions and limitations.
- Open questions and Search 7 checkpoint.
- Lightly anonymized paraphrases of Reddit evidence.
- Short quotes only when they are important and non-sensitive.

Keep private or in a separate non-public research notebook:

- Raw Reddit paste dumps.
- Usernames, profile details, exact screenshots, and highly specific stories that could identify a person.
- Long verbatim comment excerpts.
- Internal business speculation, pricing thoughts, or product strategy that you do not want competitors to see.
- Any notes tying specific Reddit users to outreach targets.
- Messy research logs that could be misread as validated claims.

If the repo is public, be extra careful. A public repo should contain synthesized insights and methodology, not raw scraped content. If the repo is private, you can keep a fuller appendix, but even then the better long-term habit is to separate raw evidence from cleaned analysis.

## Research Methodology

This research used iterative Reddit keyword searches related to vendor sourcing, vendor compliance, contractor reliability, and property-management maintenance operations. For each search, promising threads were selected based on evidence density rather than title match alone.

Evidence was prioritized when it contained:

- Firsthand operator testimony from property managers, maintenance coordinators, asset managers, board members, vendors, landlords, or contractors.
- Workflow details such as work orders, approvals, dispatch, estimates, NTE thresholds, invoices, payments, COIs, W-9s, insurance, and vendor onboarding.
- Economic signals such as software pricing, vendor fees, slow payment, trip minimums, markups, overtime, or willingness to pay for lower coordination burden.
- Contradictions, especially when one party's reasonable process creates another party's friction.
- Failure modes such as ghosting, wrong property, no authorization trail, vendor payment blocked, quality decay, or work completed without proper documentation.

Evidence was discounted when it was:

- Promotional, vendor-tech-led, or likely shilling.
- Tenant-only discussion with little professional property-management detail.
- Generic legal opinion without operational evidence.
- A single anecdote presented as a universal rule.

Important limitation: Searches 1-3 are represented in the referenced conversation mostly as summarized findings, not full thread logs. Searches 4-6 include richer thread-level evidence from pasted Reddit discussions and prior synthesis.

## Search-By-Search Logs

### Search 1: `property manager vendor problems`

Purpose: Initial broad scan for whether vendor pain exists and what shape it takes.

Summary-level findings from the prior conversation:

- Vendor reliability problems appear repeatedly: ghosting, not showing up, poor follow-through, inconsistent work quality, and communication gaps.
- PMs often become manual coordination hubs between tenants, owners, vendors, accounting, and internal staff.
- Generic reviews may not capture the operational behaviors PMs care about.
- Vendor replacement is not simply a price decision. Performance, trust, responsiveness, and coordination burden matter.
- Compliance appears as an issue, but Search 1 did not yet isolate it as a full workflow.

Core interpretation:

Search 1 established that the problem is not just "finding a contractor." It hinted that PMs need behavioral vendor track records: who responds, who shows up, who documents work, who invoices cleanly, and who can be trusted with tenants and properties.

Evidence strength: Medium. Strong directional signal, but less detailed than later searches.

### Search 2: `property management contractors unreliable`

Purpose: Test whether contractor unreliability is a PM complaint, a contractor-side economic problem, or both.

Summary-level findings from the prior conversation:

- Reliable contractors are hard to obtain partly because good tradespeople have other work.
- Small property-management jobs can be unattractive because they involve travel, scheduling, tenant coordination, admin, urgency, and payment friction.
- Skilled trades are supply-constrained. The best contractors often become booked, expensive, or selective.
- Referrals often outperform generic reviews.
- Trade skill and business/admin skill are different capabilities.
- PM work often consists of urgent small jobs, which many high-quality contractors do not prioritize.

Core interpretation:

Search 2 reframed "contractor unreliability" as partly structural. Some vendors may look unreliable to PMs because PM work is economically unattractive compared with larger, simpler, better-paying, or lower-admin work.

Evidence strength: Medium to strong. Strong recurring pattern, but mostly summarized in the available context.

### Search 3: `property manager find vendors contractors`

Purpose: Understand sourcing channels and how vendors enter PM networks.

Summary-level findings from the prior conversation:

- Vendor sourcing happens heavily through referrals, existing networks, Google, associations, suppliers, BOMA, IREM, NARPM, apartment associations, and direct relationships.
- Larger firms commonly use approved vendor lists.
- W-9, COI, license, insurance, and credentialing requirements appear as common gates.
- Vendors often enter during a displacement event: the incumbent fails, is unavailable, raises prices, stops responding, or no longer fits the need.
- New vendors may receive a small trial job before becoming regular or preferred.
- Cold outreach is saturated and often ignored.

Core interpretation:

Search 3 produced the first clear vendor lifecycle:

```text
Discovery -> Qualification -> Credentialing/Compliance -> Approved Vendor Pool -> Availability -> Assignment -> Coordination -> Completion -> Invoice/Payment -> Performance History -> Preferred/Backup/Removed
```

Evidence strength: Strong directional signal. The lifecycle model has been reinforced by Searches 4-6.

### Search 4: `property management vendor compliance problems`

Purpose: Determine whether vendor compliance is a real operational/economic pain or just paperwork.

Selected threads and evidence notes:

1. "Does your property management company verify vendor compliance for board-sourced vendors?"
   - Evidence value: High.
   - Showed that board-sourced vendors may still need PM verification.
   - One management company required VIVE compliance or a board waiver.
   - COI and W-9 could be required before payment.
   - A contractor reported that paperwork is sometimes requested only after work is complete.
   - Late paperwork requests created explicit friction, including a $25 fee per undisclosed notarized document.

2. "Commercial Property Managers: What are the biggest reasons you say yes or no to vendors?"
   - Evidence value: Secondary for compliance, useful for vendor access.
   - Showed that vendors may misunderstand whether they are vendors, tenants, amenities, or commercial users.
   - PMs consider lease obligations, owner value, property brand, space, rent, security, insurance, and whether the PM benefits from allowing access.
   - Cold emails are often ignored.

3. "[NC] Is it normal for a property manager to require an HOA to only use vendors pre-approved by the property manager?"
   - Evidence value: Very high.
   - Strong evidence that third-party compliance platforms and approved-vendor restrictions can frustrate HOAs and vendors.
   - Vendor onboarding could include insurance/document review and an annual fee around $200.
   - Some local vendors reportedly declined to participate because they did not want to pay or complete the process.
   - Counter-evidence: some commenters defended verification because policies can expire, lapse, or fail to meet coverage needs.
   - Key finding: compliance can reduce risk and reduce vendor supply at the same time.

4. Procurement-adjacent smaller-company compliance thread.
   - Evidence value: Contextual.
   - Not PM-specific, but reinforced that vendor risk is not homogeneous.
   - A payroll provider, high-risk contractor, small office supplier, and one-time low-risk vendor should not necessarily face the same compliance burden.

5. "Secret to getting on a vendor list?"
   - Evidence value: High.
   - Revealed that PMs value responsiveness, email follow-through, resident behavior, before/after photos, abnormal-condition reporting, prompt invoicing, fair charges, licensing, and insurance.
   - Key distinction: approved does not mean good. Compliance eligibility is only one part of vendor value.

6. "Managing vendor relationships at scale, anyone cracked the code?"
   - Evidence value: Mixed but useful.
   - Provided counter-evidence that vendor management is not universally chaotic.
   - Some operators say organization, folders, spreadsheets, email, and consistent vendors can work.
   - Promotional contamination from software vendors should be discounted.

7. "Property Managers: What's your maintenance workflow from start to finish?"
   - Evidence value: Incomplete in available context.
   - Useful prompt, but comments were not fully available in the referenced material.

8. "Maintenance Coordination" / 659-unit operation.
   - Evidence value: High.
   - A 659-unit operation with two maintenance coordinators described work orders, vendor assignment, estimates above NTE, invoices, and weekly vendor payments.
   - AppFolio remained part of the stack, but task/reminder gaps led people toward spreadsheets, Monday, Trello, Airtable, Google Calendar, or external maintenance tools.
   - A product at $6/unit/month was seen as appealing but potentially too expensive because it could roughly double software costs.

9. "Starting off - How are you tracking vendors and contractors?"
   - Evidence value: High.
   - OP wanted to track contacts, contracted rates, service history, and vendor/contractor details.
   - Responses ranged from corkboards, binders, business cards, and Google Sheets to PMS suites and dedicated systems.
   - Vendor information spans identity, commercial terms, compliance, operational status, financial records, work history, behavior, and internal procedures.
   - OP immediately raised cost concerns and asked whether vendors also had to pay.

10. PMS demo criteria thread.
   - Evidence value: Weak to secondary.
   - One substantive answer came from a CMMS vendor, so it should not be treated as organic PM validation.
   - Useful hypothesis only: maintenance routing, vendor coordination, work history, and reporting are relevant demo concerns.
   - Another commenter emphasized testing boring workflows, hidden costs, support, and data portability rather than polished dashboards.

Search 4 core conclusion:

Vendor compliance is not merely document storage. It is a risk-management workflow that affects vendor eligibility, payment eligibility, vendor participation, competition, PM labor, owner trust, and operational speed.

Refined lifecycle from Search 4:

```text
Discovery
-> Initial suitability / relationship / referral
-> Scope + risk requirements determined
-> Credential collection
-> Verification
-> Approved / Waived / Rejected
-> Availability
-> Assignment
-> Coordination
-> Completion
-> Invoice
-> Compliance/payment eligibility check
-> Payment
-> Performance history
-> Preferred / Backup / Restricted / Removed
-> Credential expiration -> renewal / suspension
```

Failure path directly supported:

```text
Work completed -> missing compliance discovered -> payment blocked -> document chase
```

### Search 5: likely around vendor sourcing/replacement and vendor lists

The exact search phrase is not fully preserved in the referenced context, but it followed Search 4 and focused on how PMs find, replace, and operationalize vendors.

Selected threads and evidence notes:

1. "How to find vendors to do basic maintenance?"
   - Evidence value: High.
   - PMs can find licensed trades more easily than reliable minor-repair vendors.
   - Small basic jobs are unattractive: contractors may flake, outgrow the work, or avoid PM companies.
   - A handyman-style contractor complained about PMs as slow payers, emergency-driven, low-budget, and unrealistic.
   - One contractor would not start a truck for less than $75 and was booked weeks out.
   - Existing vendors may be useful referral nodes: plumbers and electricians often know other trades.

2. "How do you find full service maintenance providers?"
   - Evidence value: High.
   - "Full service maintenance" may actually mean rehab, GC work, or multiple specialty trades.
   - Referrals from PMs, agents, vendors, real estate investors, social media, BiggerPockets, lumber yards, hardware stores, Google Maps, Thumbtack, Facebook groups, and local networks all appeared.
   - "There is no one-stop shop for everything" is a key operational point.

3. "Property managers that hire cleaning vendors, how often are you turning over cleaning vendors and why?"
   - Evidence value: Very high.
   - Cleaning vendors often turn over due to quality decline more than price.
   - Several comments described an early honeymoon period followed by complacency.
   - Some PMs prefer paying more for vendors that do not require hand-holding.
   - In-house cleaning can be cheaper for some larger operators, but liability, workers comp, staffing, and turnover complicate the comparison.
   - One failure case: vendor cleaned the wrong unit, then missed the second cleaning, discovered only at move-in.

4. "How do you get in front of property managers without being just another vendor?"
   - Evidence value: High.
   - Cold outreach is saturated and often ignored.
   - PMs may prefer face-to-face contact, warm introductions, association exposure, partner referrals, proof/case studies, and evidence of value.
   - Vendors may need to identify the right property type, decision-maker, and owner/brand constraints.
   - For on-site services, the vendor may need to justify value to the property owner, not only convenience to tenants.

5. Maintenance workflow / small landlord maintenance threads.
   - Evidence value: Exploratory.
   - Useful for comparing professional PMCs with small landlords, but less central in the available record.

6. "How do property management vendor lists work?"
   - Evidence value: Very high.
   - Vendor lists operate in multiple ways:
     - closed small pools of 1-2 vendors at set rates,
     - call-down lists where the first qualified vendor to answer may win,
     - rotation models designed to keep several vendors active.
   - "Being on the list" does not mean guaranteed work.
   - A vendor relationship can expand from one job to multiple properties and referrals.
   - One PM relationship can behave like many customers because the PM or ownership group controls many properties.
   - Vendor capabilities can be discovered after contact. A cleaning vendor may also handle gutters, fascia, soffit, or repairs.

Search 5 core conclusion:

Vendor discovery appears event-driven. PMs do not constantly search in a clean marketplace. They search when the incumbent fails, becomes unavailable, becomes too expensive, outgrows small jobs, cannot handle a new trade, or when portfolio/geography changes.

Search 5 also supports:

- Small jobs function as auditions.
- Responsiveness can allocate work.
- Vendor lists are operational models, not static directories.
- PMs may pay more to reduce coordination burden.
- Vendor performance can decay over time.
- The best vendors have options and must be worth serving.
- One good PM relationship can multiply into many properties and referrals.

### Search 6: `property manager plumber vendor`

Purpose: Test whether trade-specific research changes the meaning of vendor quality.

Selected threads and evidence notes:

1. "Property managers and plumbers"
   - Evidence value: Very high.
   - A commercial asset manager described small plumbers as cheaper but often weak on communication, service reports, professionalism, payment terms, and customer service.
   - Large plumbing companies may have better administration but higher cost.
   - Key paraphrase: the ideal vendor offers small-company pricing with large-company professionalism.
   - Another key quote-like idea: a PM wants to send a work order and usually hear back only when it is done and billed.

2. "Resident hired their own plumber after I told them not to. What now?"
   - Evidence value: High.
   - Exposes tenant bypass, unauthorized vendor use, liability, reimbursement, approved-vendor logic, emergency exceptions, and control of the maintenance supply chain.
   - The issue is not only whether work was needed, but who had authority to hire and charge for it.

3. "Property management company cannot identify who approved $2,500 in plumbing work"
   - Evidence value: Very high.
   - A wrong-property/work-order integrity failure allegedly led to $2,500 in work, invoice disputes, owner rent withheld, and uncertainty about who approved the work.
   - Key finding: a legitimate vendor, real labor, and an actual invoice do not guarantee legitimate authorization.
   - Work-order identity integrity is a first-class risk.

4. "How do property managers handle vendors when tenants aren't home?"
   - Evidence value: Medium to high.
   - Vendor access can be handled by PM escort, tenant coordination, lockboxes, keys, or trusted vendor access.
   - Trust changes operational cost. A trusted vendor may literally gain access to the building/unit and reduce PM escort burden.

5. "How to be a preferred vendor"
   - Evidence value: Very high.
   - Reinforced displacement events: PMs already have vendors, but openings appear when a current vendor has been lacking or unavailable.
   - One successful job can move a vendor into rotation.
   - Emergency plumbing can invert normal preference rankings if the usual vendor is unavailable or charges extreme overtime.

6. "Becoming a vendor for property managers"
   - Evidence value: High.
   - Trade-side economics: a large PM can be "500 customers in one."
   - Vendors may offer better terms because a PM relationship reduces customer acquisition cost and creates repeat volume.
   - Counterpoint: customer concentration risk if one PM becomes too large a share of revenue.

7. Tenant/handyman vs plumber thread.
   - Evidence value: Weak to medium.
   - Useful hypothesis around triage from handyman to licensed specialist, but limited professional PM evidence in the available record.

8. "Property Managers: What task still wastes the most time, even with AppFolio, Buildium, or Yardi?"
   - Evidence value: High.
   - Important counter-evidence: at least one person said they did not need more software or AI.
   - Another operator still experienced time loss from chasing contractors, schedules, updates, invoices, and relaying information despite PMS tooling.
   - Key distinction: system problem vs actor problem. Software can improve information flow, but it cannot fully make a vendor answer the phone.

9. "Property manager charging us for plumber call out"
   - Evidence value: High.
   - Introduced the "no fault found" or unable-to-reproduce problem.
   - A plumber can perform legitimate diagnostic labor even when no repair occurs.
   - Cost allocation becomes ambiguous when a tenant reports an intermittent issue that cannot be verified on arrival.

10. "High vendor bills from property management"
   - Evidence value: Very high.
   - Owner asked how to know whether vendor and handyman bills from a PM are legitimate.
   - Responses distinguished documentation, photos, approval thresholds, three quotes, PM markup, verifying work, calling vendor, and sign-in/sign-out.
   - Approval thresholds in the $300-$1,000 range appeared, with lower examples like $250-$400 in other threads. Treat as anecdotal ranges, not a universal standard.
   - A commenter claimed PMCs may mark up maintenance around 15%, but this should be treated as anecdotal evidence of markup practices, not a benchmark.
   - Key insight: "legit" can mean work happened, scope was valid, price was reasonable, and spend was authorized. These are separate questions.

Search 6 core conclusion:

Plumbing showed that vendor quality is trade-specific. The PM is buying both physical trade work and administrative/operational service. Plumbing adds urgency, risk, diagnostic uncertainty, after-hours economics, authorization complexity, tenant access, responsibility disputes, and cost-allocation ambiguity.

## Selected Thread Summaries

### Board-sourced vendor compliance and payment gates

This thread exposed a critical compliance failure mode: a vendor can perform work with permission and scheduling, then be asked for paperwork only after completion before payment is released. The PM/association wants insurance protection and W-9 documentation, but the vendor experiences late paperwork as an administrative penalty. The $25 undisclosed-notarization fee is a concrete signal that vendors monetize surprise friction.

Evidence-backed insight: Compliance status can determine payment eligibility, not just work eligibility.

### HOA pre-approved vendor restriction

The HOA thread showed the strongest compliance paradox. The HOA wanted to use local vendors, but the management company required pre-approved vendors and a third-party process with fees. Some commenters viewed the requirement as protection against uninsured or improperly verified vendors. Others viewed it as friction that pushed away local vendors and reduced competition.

Evidence-backed insight: Compliance can function as a vendor-supply gate.

### Vendor tracking systems: binder to enterprise software

The "Starting off" thread showed current-state maturity variance. Some PMs use paper, binders, corkboards, business cards, and spreadsheets. Others use PMS suites, COI trackers, or vendor-specific platforms. The OP wanted contacts, rates, and service history, while replies expanded the data model to compliance, invoices, work orders, communication, scheduling, and procedures.

Evidence-backed insight: Vendor data is not a single table. It is a mixed operational memory system.

### Cleaning vendor turnover

Cleaning vendor threads showed that quality decay is a repeated failure mode. Vendors may start strong, then decline after months or years. PMs replace cleaners mostly for quality, not price. Some PMs would rather pay more for a vendor that does not require hand-holding.

Evidence-backed insight: Performance history must include trend/decay, not only initial qualification.

### Vendor list operating models

The vendor-list thread showed that lists can mean closed pools, call-down lists, rotations, or contact repositories. A vendor may be registered but not active, active but not preferred, preferred for one job type but not another, or only used when the main vendor fails.

Evidence-backed insight: "Approved vendor" is a weak status unless paired with behavior, usage, and context.

### Plumber professionalism gap

The plumber thread showed that small vendors may be cheaper but operationally frustrating, while large vendors may be administratively polished but expensive. The attractive gap is a small plumber who behaves like a larger professional service organization: good communication, reports, invoices, photos, and no excessive hand-holding.

Evidence-backed insight: Operational maturity is a vendor attribute separate from trade skill.

### $2,500 plumbing authorization failure

This thread is one of the clearest operational-risk cases. The issue was not simply a bad vendor. It was uncertainty about which work order, property, owner, issue, vendor, and approver were linked to a large spend.

Evidence-backed insight: Authorization provenance and work-order identity integrity are core vendor-management data.

### High vendor bills and owner trust

This thread shifted the lens from PM trust in vendor to owner trust in PM vendor decisions. The owner wanted to know whether bills were "legit." The evidence showed that legitimacy involves proof of work, valid scope, fair price, documented approval, possible PM markup, and whether the vendor was properly vetted.

Evidence-backed insight: Trust cascades from owner to PM to vendor. If owner trust breaks, PM coordination burden increases.

## Recurring Problems

- Vendors ghost, delay, or fail to respond.
- PMs must chase updates, invoices, photos, reports, and schedules.
- Small jobs are hard to staff economically.
- Good contractors are booked and selective.
- PM work can be unattractive because of urgency, admin, small scope, slow payment, and owner/tenant coordination.
- Approved-vendor and compliance requirements can repel good small vendors.
- Vendor data lives across binders, spreadsheets, PMS tools, email, accounting systems, and memory.
- Owner approvals and NTE thresholds create conditional authorization.
- Vendors may be technically good but administratively poor.
- Quality can decay after initial success.
- Generic reviews do not capture PM-specific operational performance.
- Vendor status is contextual, not binary.
- Emergency work changes vendor-selection priorities.
- Diagnostic work can produce real cost without a clear repair.
- Work-order/property/owner mismatches can create expensive downstream disputes.

## Contradictions Worth Preserving

| Tension | Side A | Side B |
|---|---|---|
| Compliance | Reduces liability and verifies insurance | Shrinks vendor pool and adds friction |
| Third-party vetting | Saves PM labor and monitors renewals | Vendor/HOA may pay fees and lose flexibility |
| Approved list | Creates trusted known options | Can create lock-in, suspicion, or fewer bids |
| Standard requirements | Easier to administer | Risk differs by vendor, job, scope, and frequency |
| Small vendors | Cheaper and flexible | Often weaker admin and communication |
| Large vendors | Professional systems and reports | More expensive |
| Lowest bid | Owner-friendly on paper | May increase callbacks, PM labor, or risk |
| Software | Can organize workflows | Cannot fully solve actor non-responsiveness |
| Binder/spreadsheet | Cheap and familiar | Fragile as scale, turnover, and complexity increase |
| Emergency speed | Prevents larger loss | Can bypass quotes and normal approval discipline |
| Credentialed | Eligible to work | Not necessarily good to work with |
| Preferred vendor | Trusted default | May be wrong for after-hours, geography, specialty, or price context |

## Workflows Observed

### Generic vendor lifecycle

```text
Discovery
-> Qualification
-> Credentialing / compliance
-> Approved / waived / rejected
-> Trial job
-> Active usage
-> Performance history
-> Preferred / rotational / backup / inactive / removed
-> Renewal, re-verification, or suspension
```

### Maintenance work order lifecycle

```text
Issue reported
-> Triage
-> Internal maintenance vs external vendor decision
-> Vendor selection
-> Authorization / NTE check
-> Access coordination
-> Dispatch
-> Diagnosis
-> Scope confirmation or escalation
-> Repair / no-fault-found / callback / project conversion
-> Evidence captured
-> Invoice
-> Owner/tenant/PM/insurance allocation
-> Payment
-> Performance record updated
```

### Expense confidence chain

```text
Who requested the work?
-> Why was it necessary?
-> Who authorized it?
-> What scope was approved?
-> What did the vendor actually do?
-> What evidence exists?
-> What did it cost?
-> Was the price reasonable in context?
```

### Compliance and payment failure path

```text
Work completed
-> Missing compliance discovered
-> Payment blocked
-> Vendor chased for documents
-> Vendor adds fee, refuses future work, or delays participation
```

### Displacement event lifecycle

```text
Incumbent vendor trusted
-> PM ignores most cold outreach
-> Incumbent becomes unavailable, expensive, slow, overextended, or low quality
-> Alternative vendor becomes relevant
-> Small trial job
-> Performance observed
-> Vendor enters rotation or preferred pool
```

## Economic Incentives

### PM incentives

PMs want responsive, insured, competent, reasonably priced vendors who accept work orders, coordinate with residents, document work, invoice cleanly, and do not require constant management. PMs are often trying to reduce time spent chasing people.

### Vendor incentives

Vendors want profitable work, clear scope, predictable scheduling, prompt payment, low admin, and enough future volume to justify PM-specific friction. PM relationships are attractive when one relationship unlocks many properties. They are unattractive when small jobs, strict windows, low pay, slow payment, compliance fees, and multiple portals outweigh expected value.

### Owner/board incentives

Owners and boards want fair pricing, proof of work, insurance protection, approval controls, and confidence that the PM is not mismanaging or marking up costs without transparency.

### Tenant incentives

Tenants want speed and resolution. Tenant urgency can conflict with PM approval processes, owner controls, vendor availability, and compliance rules.

### System-level feedback loop

```text
Slow/annoying PM payment and admin
-> vendors charge more or avoid PM work
-> owners see expensive bills
-> owners demand more approval, quotes, and documentation
-> PM workload increases
-> vendor admin increases
-> PM work becomes less attractive
-> prices rise or vendor supply shrinks
```

## Willingness-To-Pay Signals

Positive or suggestive signals:

- PMs already pay for AppFolio, Buildium, Yardi, Rentvine, PropertyMeld, Monday, Trello, Airtable, Google Calendar, Prism/Building Engines, NetVendor, VIVE-like systems, and other tools.
- A 659-unit operator saw value in maintenance coordination software, though price was a concern.
- Some HOAs reportedly subsidize vendor onboarding fees to preserve preferred vendor supply.
- PMs may pay more for vendors who reduce hand-holding.
- Vendors may offer better terms to PMs because one PM relationship can create repeat volume across many properties.

Negative or cautionary signals:

- $6/unit/month was seen by one operator as possibly too expensive because it could roughly double software costs.
- Thin margins and OpEx concerns appeared immediately in response to vendor-management software.
- Two-sided vendor adoption is a serious risk if vendors must create accounts, learn platforms, pay fees, or monitor another system.
- Manual binders and spreadsheets are counter-evidence: low-tech systems can be "good enough" for some operators.
- At least one comment explicitly rejected more software or AI.

Interpretation:

There is willingness to pay around this problem space, but it appears conditional. The product would need to create obvious operational value, avoid creating vendor-side friction, and beat existing cheap/manual workflows for the target segment.

## Vendor Lifecycle Evolution

### Initial lifecycle after Search 3

```text
Discovery -> Qualification -> Credentialing/Compliance -> Approved Vendor Pool -> Availability -> Assignment -> Coordination -> Completion -> Invoice/Payment -> Performance History -> Preferred/Backup/Removed
```

### Revised lifecycle after Searches 4-6

```text
Discovery
-> Initial suitability / source trust
-> Risk and scope classification
-> Credential collection
-> Verification
-> Approved / waived / rejected
-> Availability and access check
-> Assignment with NTE or approval context
-> Coordination with tenant/PM/vendor
-> Diagnosis and possible escalation
-> Completion, partial completion, no-fault-found, or callback
-> Evidence and service report
-> Invoice and cost allocation
-> Compliance/payment eligibility
-> Payment
-> Behavioral performance history
-> Preferred / active / rotational / backup / restricted / removed
-> Renewal / expiration / re-verification / suspension
```

### Vendor status taxonomy

- Prospect: known but not evaluated.
- Credentialed: paperwork collected.
- Verified: paperwork checked.
- Approved: eligible for some work.
- Waived: allowed despite normal requirements, usually for one-time or special cases.
- Trialed: has completed first/small job.
- Active: receiving work.
- Preferred: default for a context.
- Rotational: receives some work to keep relationship active or compare performance.
- Backup: used when preferred vendor fails or is unavailable.
- Restricted: limited due to scope, risk, pricing, or behavior.
- Removed: no longer used.
- Expired/suspended: blocked by lapsed documents or compliance status.

## Evidence-Backed Hypotheses

1. VendorRadar's strongest opportunity is probably not raw discovery. It is operational vendor intelligence: who is usable, proven, available, compliant, and low-friction for a specific job.
2. A PM-specific vendor record should track behavior, not just contact info and documents.
3. The cost of coordination may be as important as the vendor's invoice price.
4. Approved-vendor status is insufficient because credentialed does not mean trusted.
5. Vendor relationships are context-specific: preferred for routine work may differ from preferred for emergency, after-hours, specialty, geography, or owner-sensitive work.
6. Compliance should be risk-adjusted. A one-time low-risk event vendor and a sewer contractor do not require identical handling.
7. Vendor supply is partly endogenous to PM process. Slow payment, portals, fees, and paperwork can make the PM market less attractive.
8. Property-management software may remain system of record while operational coordination spills into auxiliary tools.
9. Vendor discovery is often triggered by displacement events rather than continuous marketplace browsing.
10. Trade-specific intelligence matters. Plumbing, cleaning, landscaping, locksmithing, handyman work, and general contracting have different risk/economic profiles.

## Falsification And Limitations

The research should not yet claim:

- That all PMs have severe vendor-management pain.
- That every PM would pay for VendorRadar.
- That Reddit comments represent the whole market.
- That any quoted fee, markup, or approval threshold is an industry benchmark.
- That compliance platforms are bad.
- That software alone can fix vendor non-responsiveness.
- That generic reviews are useless in every case.
- That property managers are the only buyer or decision-maker.

Counter-evidence already observed:

- Some operators say basic organization solves the problem.
- Binders and spreadsheets may work for smaller or simpler operations.
- Some PMS suites already include compliance, invoicing, W-9, COI, work-order, and vendor modules.
- Some comments defending third-party verification are reasonable and operationally valid.
- A software-led thread is weak evidence of organic buyer demand.
- Search 1-3 source detail is limited in the accessible referenced conversation.

Next falsification targets:

- Find PMs who are satisfied with current PMS/vendor workflows and understand why.
- Find operators who tried vendor-management tools and churned.
- Find vendor-side reactions to portals, PM payment terms, and compliance systems.
- Quantify whether coordination burden creates measurable labor cost.
- Test whether PMs would switch from spreadsheet/binder when only vendor intelligence, not accounting, is improved.

## Trade-Specific Plumbing Findings

Plumbing is not just another vendor category.

Search 6 showed that plumbing changes the vendor-management problem because:

- Problems can be urgent and damage-sensitive.
- Diagnosis may change scope after dispatch.
- The correct vendor may depend on capabilities such as camera inspection, jetting, sewer replacement, fixture repair, or emergency response.
- The PM may not be able to verify technical recommendations easily.
- After-hours availability can exist only at a major price premium.
- Emergency work can override normal quote-shopping or approval processes.
- Cost responsibility may shift after diagnosis: owner, tenant, HOA, insurance, PM, or vendor callback.
- Tenant access can determine whether an available plumber is actually usable.
- "No fault found" can still create a legitimate invoice.

Plumbing-specific vendor intelligence likely includes:

- Routine service capability.
- Emergency availability.
- After-hours pricing behavior.
- Drain/sewer specialty.
- Diagnostic honesty.
- Equipment/capability profile.
- Tenant professionalism.
- Photo/report quality.
- Callback rate.
- NTE discipline and approval behavior.

Key distinction:

The PM is not only buying pipe repair. The PM is buying diagnosis, urgency response, trust, documentation, resident coordination, and reduced operational risk.

## Key Quotes And Paraphrased Evidence

These should be treated as directional evidence, not universal claims.

- PM wants a vendor where they can send a work order and usually not hear again until the work is done and the bill arrives.
- Small plumbers are often cheaper, but some PMs find them weak on service reports, communication, professionalism, and payment process.
- A vendor who combines small-company pricing with large-company professionalism would become a favorite.
- A board/HOA vendor may need VIVE compliance or a board waiver, plus COI and W-9 before payment.
- A contractor reported that about a third of paperwork requests come after the work is already done.
- Some local vendors do not want to pay for the privilege of getting onto a third-party approved list.
- Compliance certification does not guarantee work quality.
- PMs often care more about a vendor who answers, schedules, behaves well with residents, sends photos, invoices promptly, charges fairly, and stays licensed/insured.
- For cleaning vendors, quality decay after the first months or years appeared repeatedly.
- For some PMs, quality matters more than price when replacing cleaning vendors.
- Some PMs call down a list and hire the first acceptable vendor who answers.
- One PM relationship can represent many properties and therefore many future jobs.
- A vendor can perform real work and submit a real invoice while the expense is still invalid because authorization or property linkage was wrong.
- Photos serve as expense evidence, not merely nice documentation.
- Three quotes may be the best pricing check, but can be a nightmare operationally and irrational during emergencies.
- Reliable, licensed, insured people are not cheap.
- PM maintenance markup may exist and should be disclosed, but a single Reddit estimate should not be treated as a benchmark.

## Cross-Search Synthesis

Searches 1-3 established the broad shape: PMs experience vendor reliability, communication, quality, sourcing, compliance, and coordination problems. Referrals and networks matter more than generic directories, and vendor discovery often occurs when existing vendors fail or cannot serve the need.

Search 4 deepened the compliance layer. Compliance is not just paperwork; it can determine whether a vendor is eligible to work or get paid. It protects the PM/HOA but can also reduce vendor supply, create resentment, increase prices, and require waivers.

Search 5 showed that sourcing and vendor lists are not stable directory problems. The vendor list can be a call-down list, rotation, closed pool, or loose contact repository. Vendor performance changes over time, and PMs may pay more for vendors that need less management.

Search 6 proved that trade-specific research is necessary. Plumbing revealed authorization, diagnostic trust, urgency, after-hours price, access, and cost-allocation issues that were not visible in generic vendor searches.

The strongest integrated model:

```text
VendorRadar problem space =
vendor supply access
+ compliance/risk eligibility
+ operational coordination
+ contextual dispatch intelligence
+ behavioral performance history
+ invoice/payment/authorization confidence
```

## Research Glossary And Taxonomy

Approved vendor: A vendor eligible to receive some work, usually after compliance or internal review. Not equivalent to preferred.

Preferred vendor: A vendor favored for a specific context. Preference may depend on trade, urgency, geography, price, owner, property, or history.

Backup vendor: A vendor used when a preferred vendor is unavailable, too expensive, or inappropriate for the job.

Displacement event: The moment an incumbent vendor becomes vulnerable because of failure, unavailability, price, quality decay, or changed needs.

Trial job: A first or small job used to observe whether a vendor can perform before being trusted with more work.

Operational maturity: A vendor's ability to communicate, document, invoice, schedule, coordinate access, follow procedures, and reduce PM workload.

Coordination burden: The number and cost of PM touches required to move a work order forward.

Authorization provenance: Who approved the work, when, for what scope, at what amount, and under which authority.

NTE: Not-to-exceed amount. Often tied to owner approval thresholds.

Expense confidence chain: The evidence required to trust that a vendor expense was necessary, authorized, completed, documented, and fairly priced.

Compliance gate: A requirement that determines whether a vendor can work or be paid.

Vendor friction cost: The administrative, financial, and behavioral burden imposed on a vendor by PM processes.

No-fault-found: A vendor visit where the reported issue cannot be reproduced or confirmed, but diagnostic labor still occurred.

Work-order identity integrity: Confidence that the correct vendor, property, unit, owner, issue, authorization, and invoice are linked.

Two-sided adoption friction: Resistance created when software requires both PMs and vendors to use, pay for, or monitor another system.

## Open Questions

1. Which PM segment feels this pain most acutely: small residential, scattered-site SFR, multifamily, HOA/condo, commercial, student housing, or mixed portfolios?
2. Is the best buyer the PM owner/operator, maintenance coordinator, asset manager, accounting/compliance team, HOA board, or vendor?
3. What is the minimum vendor data model that creates value beyond a spreadsheet?
4. How much does vendor coordination burden cost in labor hours per month?
5. What workflows are already solved well by AppFolio, Buildium, Yardi, Rentvine, PropertyMeld, NetVendor, VIVE, Prism, and similar tools?
6. Where do these tools fail: vendor adoption, reminders, renewals, communication, mobile use, owner transparency, or analytics?
7. Would vendors cooperate with a VendorRadar-like system if it helped them get work and reduce payment/admin friction?
8. How often do PMs override approved-vendor lists during emergencies?
9. What evidence do owners most need to trust vendor bills?
10. Is "vendor intelligence" more valuable for high-risk trades like plumbing, HVAC, electrical, roofing, and restoration than for cleaning or landscaping?
11. How often does performance decay occur, and can PMs detect it before failure?
12. How do PMs handle vendor knowledge when employees leave?
13. Can PM-to-PM referral trust be captured ethically and practically?
14. How does in-house maintenance change the need for external vendor intelligence?

## Checkpoint For Search 7 Tomorrow

Search 6 is complete. Tomorrow should start with Search 7.

Recommended direction for Search 7:

```text
property manager vendor performance tracking
```

Alternative search phrases:

```text
property management contractor performance tracking
property manager vendor scorecard
property management vendor reviews contractors
property manager maintenance vendor quality
property management contractor callbacks
property manager vendor not responding
```

What Search 7 should test:

- Do PMs explicitly track vendor performance, or is it mostly memory?
- What performance dimensions matter: response time, show rate, completion rate, callback rate, invoice accuracy, resident complaints, photos, reports, price, cleanup, professionalism?
- Do teams maintain scorecards or only informal preferred lists?
- What causes a vendor to be demoted, paused, or removed?
- How do PMs detect quality decay?
- Do existing PMS tools capture performance history in a usable way?
- Do PMs compare vendors across properties, regions, or teams?
- Can vendor performance be separated from tenant behavior, owner constraints, property condition, or bad work orders?

Suggested thread selection criteria:

- Prioritize firsthand PM/maintenance comments describing how they decide to keep, replace, or rank vendors.
- Preserve contradictions between "we track everything" and "we just know who is good."
- Watch for measurable fields that appear organically.
- Discount promotional software comments unless corroborated by organic operator testimony.

## Final Position At This Checkpoint

The research is worth saving and continuing. It should be committed as cleaned project documentation, not as raw Reddit dumps. The evidence is strong enough to justify further discovery and increasingly points toward a nuanced operational problem. It is not yet strong enough to justify building.

The next research stage should focus on performance tracking, then move to another forum to reduce Reddit bias and test whether the same patterns appear in different professional communities.
