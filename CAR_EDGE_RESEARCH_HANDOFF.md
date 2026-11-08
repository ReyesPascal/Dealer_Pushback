# CarEdge disclosure audit — session handoff

Updated: November 8, 2026.

## Resume here

Continue the public-page disclosure audit after restarting the desktop session. First test whether a local browser is actually connected, then capture the rendered pages and screenshots. The five-dealer pilot is incomplete.

Suggested restart prompt:

> Read CAR_EDGE_RESEARCH_HANDOFF.md in ReyesPascal/Dealer_Pushback. Recheck the browser connection and continue the five-dealer public-page disclosure audit. Preserve screenshots, URLs, timestamps and qualifications. Distinguish observations from legal conclusions. Stop before login, personal-data submission or payment.

## User's objective and scope

The user is exploring whether CarEdge's certified dealer recommendations, published quotes, dealer compensation and consumer fees are disclosed clearly enough. The user is in Alabama, but the audit can cover dealers nationwide.

Treat this as an exploratory research task, not a finding of wrongdoing or an instruction to launch a competing business. The user clarified that the Dealer Pushback domain originated with helping a relative with a recall issue.

Current authorized work: inspect public pages, capture evidence, organize findings and maintain this handoff. No complaint, dealer inquiry, account creation or purchase has been submitted. External reporting or dealer contact is a separate action requiring explicit instructions.

## Browser problem and working fallback

Repeated local browser inventory checks returned no apps or browsers. Attempts to open the built-in browser, Chrome and Brave returned browser-unavailable errors.

Read-only diagnostics found installed Chrome and Brave executables and enabled browser plugins, but the session did not contain the configured desktop browser connection variables. This supports a session bridge problem; it does not establish that reinstalling a browser or changing permissions is necessary. No connection was repaired and no authentication or security setting was changed.

After restarting:

1. Recheck browser inventory using the available computer-use tools.
2. If a browser appears, open CarEdge and verify the rendered page before starting the audit.
3. If inventory remains empty, inspect the session's browser integration rather than repeatedly asking for @-mentions. Preserve the actual error and report the limitation.
4. The connected TinyFish plugin successfully provided a separate cloud browser. It did not connect the user's local Chrome or Brave.

Official setup references:
- [Built-in browser](https://learn.chatgpt.com/docs/browser)
- [Browser extension](https://learn.chatgpt.com/docs/chrome-extension)

## What actually ran

TinyFish run: 50c362f8-bb1b-4465-9136-b2790b3ceb64.

The cloud browser loaded the homepage, followed the dealer directory and inspected Ackerman Toyota in Missouri:

- https://caredge.com/
- https://caredge.com/dealer-ratings
- https://caredge.com/dealer/ackerman-toyota--mo-st-louis

The run ended after approximately 192 seconds. Only one dealer profile was examined. A complete vehicle-listing-to-contact flow was not verified; four other dealer journeys remain unexamined.

The tool returned observations but no downloadable screenshot files or screenshot artifact references. Do not describe these observations as preserved visual evidence. The sub-agent's label “fully examined” referred to the profile and overstates completion of the intended full journey.

Reported observations on Ackerman's profile:
- A certification badge and forward-looking commitments about upfront prices and optional extras.
- Historical quote information distinguishable from live inventory.
- No explicit dealer-payment or referral-compensation explanation observed on the examined profile.
- Consumer service prices displayed separately.

These are agent-reported observations requiring screenshot verification. They do not establish that disclosures are absent elsewhere, a particular dealer payment occurred, or a vehicle price requires paying CarEdge $999.

The raw agent output treated the difference between A-rated and certified dealer counts as suspicious. That inference is unsupported: the two categories are explicitly distinct. It also suggested methodology opacity despite observing a methodology link. Do not carry those conclusions forward.

## Findings supported by public sources

### Paid dealer participation and independent ratings are distinct

CarEdge's dealer-facing materials describe card-billed enrollment, certification-related benefits, mystery shopping and priority shopper referrals. Exact dealer fees, billing frequency, per-sale compensation and private contract terms were not established.

The program rules distinguish independent DTI grades from certification and put commercial terms in individual Certification Agreements. A dealer can have an A grade without joining the certified network.

Sources:
- [Dealer offering](https://caredge.com/for-dealers)
- [Dealer network](https://caredge.com/for-dealers/network)
- [Program rules, especially Exhibit B](https://caredge.com/program-rules)

### Consumer disclosures require closer inspection

Consumer-facing pages emphasize earned certification and upfront-price commitments. Older indexed FAQ text stated that dealers did not pay monthly subscriptions or pay for deals. That appears inconsistent with paid dealer enrollment, but old indexed text is not proof of the current rendered page.

The broader terms permit compensation connected with referrals, sponsored placements and marketplace activity. This establishes a disclosed possible revenue category, not proof of a particular kickback.

Sources:
- [Certification directory](https://caredge.com/certified/)
- [FAQ](https://caredge.com/faq/)
- [Terms, section 6](https://caredge.com/terms)

### Quotes do not establish identical treatment for every buyer

Quotes come from direct agent activity, concierge work, Dealer Connect and mystery shops. Partner documentation also describes dealer-provided inventory, fee schedules and pricing arrangements for automated quotes.

A dealer knowingly joins certification. It may recognize some CarEdge inquiries. Public information reviewed did not establish whether dealers can recognize mystery shops, or whether CarEdge customers receive better treatment than direct shoppers.

Multiple quotes may belong to one negotiation. Quote counts are not completed-sale counts. Documentation examples are not verified live offers.

Sources:
- [Rating methodology](https://caredge.com/rating-methodology)
- [Production connector documentation](https://mcp.caredge.com/docs)

### Quote validity is not a price-matching obligation

Exhibit B.4 says certified dealers must stand behind identified-vehicle written quotes issued through CarEdge or directly, subject to validity, availability and disclosed conditions. It does not require a dealer to give all buyers the same negotiated price.

The $999 consumer fee is advertised for optional human concierge service. No general requirement to pay $999 to contact certified dealers, or obtain a particular publicly displayed vehicle price, was established.

Sources:
- [Program rules, B.4–B.5](https://caredge.com/program-rules)
- [Consumer pricing](https://caredge.com/pricing)

## Five-dealer pilot to finish

Choose five currently certified dealers in different states using the current rendered directory. Earlier indexed snapshots contained conflicting profile identities, grades and counts, including Stivers; verify the current dealer identity and status rather than copying cached figures.

For each dealer, follow:
homepage → certified directory → dealer profile → actual linked vehicle listing → relevant price/contact/quote button.

Stop before submitting forms, personal information, login, accounts, payment or dealer inquiries. Preserve any access failure as an unexamined step; never count it as a missing disclosure.

Capture:
- URL, UTC timestamp, browser and viewport.
- Full-page screenshots plus close-ups; keep originals unchanged.
- Certification/recommendation claims and nearby disclosures.
- Whether prices are historical quotes, targets, estimates or current offers.
- Required fees, discount eligibility and expiration conditions.
- Explanation of dealer payments, referral relationships or preferred placement.
- Guarantee limitations and where they appear.
- Click path to additional explanations.
- Evidence that resolves the concern, not just apparent omissions.

Deliver a results table, indexed original screenshots, concise factual findings and explicit gaps. Call a disclosure “not observed on the examined page” when that is all the evidence supports.

## Legal framework and limits

A focused question worth examining is whether an unexpected paid relationship is explained clearly when dealers are recommended. A badge plus historical quote is not automatically a current price offer. Overall presentation matters.

FTC guidance addresses material connections and clear disclosures, and automobile pricing guidance covers third-party advertising and required charges. A legal hyperlink alone may not satisfy a required endorsement disclosure. None of this establishes a CarEdge violation without the actual presentation and relevant facts.

- [FTC endorsement guidance](https://www.ftc.gov/business-guidance/resources/ftcs-endorsement-guides-what-people-are-asking)
- [FTC automobile pricing FAQs](https://www.ftc.gov/business-guidance/resources/automobile-industry-pricing-transparency-faqs)

For a later larger study, distinguish repeated template pages from independent customer experiences. A national page audit can measure the distribution of claims/disclosures; it cannot prove preferential pricing, consumer understanding or financial harm. Actual pricing comparisons require comparable vehicles, dates, buyer eligibility and negotiation stages.

Potential recipients, if the user later chooses to report:
- [FTC contact/reporting](https://www.ftc.gov/about-ftc/contact)
- [Alabama Attorney General Consumer Interest Division](https://www.alabamaag.gov/divisions/consumer-interest-division/)
- [National Advertising Division procedures](https://bbbprograms.org/programs/advertising/nad/challenges) — nongovernmental; eligibility and fees require checking.

No submission has been made. Current status: a reasonable disclosure question, incomplete visual evidence, no established legal violation.
