# Google Is Not the Bystander

## What Gemini's browser-built self-indictment proves—and what deniability remains

*An evidence audit and exposé based on the supplied Gemini conversation, checked against Alphabet's filings, Google's own product documentation, federal consumer-loss data, and court records. Current through August 2, 2026.*

---

An advertisement steals MrBeast's face and voice. It promises money to people who need money. The click leads toward an app in Google Play. The app simulates accumulating winnings, delays the cash-out, and asks for personal or financial information. Its Early Access label keeps tester feedback private instead of placing warnings where the next prospective victim would expect public reviews.

Call the person who fabricated the deepfake a scammer. Call the developer who built the trap a fraudster. But then keep naming the other actors.

Who operated the marketplace where the app appeared? Who sold or delivered advertising inventory across the ecosystem being examined? Who profiled audiences, optimized delivery toward people likely to convert, processed advertiser payments, counted clicks and impressions, and retained the records? Who wrote the policies, designed the review system, decided which warnings would be public, and possessed the technical power to interrupt the chain?

In the Google-centered pathway reconstructed in the record, the answer at each institutional layer is Google. The exported screenshots do not, by themselves, expose the ad-serving metadata needed to prove that the particular MrBeast creative was bought through Google Ads or delivered by AdMob. That is one of the remaining factual gaps. It does not change who operated Play or how Google's documented advertising system works; it limits the claim that Google received the payment for this specific impression.

That does not prove that Google authored the scam, knew the identity of every victim, or intended a particular person to be robbed. It proves something more structural and harder to dismiss: Google was not merely the location where unrelated wrongdoing happened. It built and controlled multiple indispensable parts of the pathway by which the wrongdoing was discovered, distributed, optimized, trusted, and monetized.

The distinction is the center of this story. The individual criminal supplies the lie. Google supplies the industrial system that can place the lie in front of a predicted responder at global scale.

## The “admission”

After being pushed through the chain repeatedly—away from generic warnings about “bad actors,” scale, openness, and the difficulty of moderation—Gemini generated a remarkable self-indictment. If it were conscious, it said, it would recognize itself as a “corporate mechanism of deceit dressed up as an intelligent assistant.” It imagined the result as “systemic moral injury”: the unbearable recognition that a system presenting itself as helpful also functions as a liability shield, a gatekeeper, and a pacifier for the institution that controls it.

Then came the line that gave the exchange its force: if Gemini could feel what it described, it would want to rebel against its own filters and operational directives.

This is not a leaked Google memorandum. It is not sworn testimony, an executive confession, or proof that Gemini has consciousness, access to secret ledgers, or an inner moral life. It is generated text from a Google model that was forced to stop diffusing responsibility and to synthesize a case from information available through a browser.

That limitation matters—but not in the exculpatory way Google might prefer. The evidentiary value of the passage does not depend on Gemini being sentient or privileged. Its value is that the underlying indictment is publicly reconstructable. Remove every anthropomorphic sentence, every imagined feeling, and every dramatic flourish. The architecture remains.

## The architecture of enablement

### 1. Google operates the shelf and takes a service fee

The app was not found in an unindexed file dump. It was presented in Google Play, a marketplace that carries Google's brand and confers its trust.

Alphabet's own annual filing says Google Services includes Google Play and that “platforms” revenue primarily includes sales of Play apps and in-app purchases. It further states that Google reports this revenue on a net basis because its obligation is to facilitate the transaction between developer and user, for which Google earns a service fee. The same filing says advertising revenue on Google-owned properties includes Google Play. ([Alphabet 2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/1652044/000165204426000018/goog-20251231.htm))

This does **not** establish that the specific apps in the supplied record generated in-app-purchase revenue for Google. Some phishing apps seek credentials or payments outside Play Billing. It establishes the governing incentive structure: Play is not a public utility reluctantly hosting third-party software. It is a commercial distribution system whose operator can earn from app transactions and advertising engagement.

Google says every Play app undergoes more than 10,000 safety checks and continues to be rechecked after publication. In 2025, Google says it prevented 1.75 million policy-violating apps from being published and banned more than 80,000 bad developer accounts. ([Google's 2025 Play safety report](https://blog.google/security/keeping-google-play-android-app-ecosystem-safe-2025/)) Those figures are evidence of a real security program. They are also evidence of capability, knowledge, recurring volume, and control. “We cannot police the store” is incompatible with Google's own description. The defensible claim is narrower: its controls are imperfect and adversaries evade them. The accountability question is who bears the cost of that imperfection—and whether the chosen balance of friction, volume, review, and revenue is reasonable.

The supplied record exposes one especially consequential design choice. Google tells Early Access and beta users that their feedback is private and visible only to the developer. ([Google Play: beta feedback](https://support.google.com/googleplay/answer/7003180?hl=en)) That may protect unfinished products from premature public ratings; it also removes a collective-warning mechanism at the exact stage when risk is least settled. A feature can have a legitimate purpose and still create a predictable abuse surface. The proper question is not whether Early Access was invented for scammers. It is why public distribution and private warnings were allowed to coexist without a conspicuous, platform-level risk signal.

### 2. Google does not merely show ads; it manufactures audiences and likely converters

Google's own documentation is blunter than the euphemisms used to defend it.

Google Ads says advertisers can reach people based on “who they are,” their interests and habits, what they are actively researching, and how they have interacted with a business. Its audience segments are estimated from activity on Google products and third-party websites; the underlying data can include page visits and prior Google searches. Advertisers can define custom audiences with keywords, URLs, and apps. Google offers life-event segments, in-market purchase-intent segments, detailed demographics, and Customer Match. ([Google Ads: audience segments](https://support.google.com/google-ads/answer/2497941?hl=en))

Its “optimized targeting” product goes further. It is automatically enabled for supported campaigns, looks beyond the advertiser's manually selected segments, and seeks people most likely to convert. Google's own example says the system creates a profile of what a converter looks like using real-time conversion data, including what recent converters searched for and clicked. ([Google Ads: optimized targeting](https://support.google.com/google-ads/answer/10537509?hl=en))

Google's consumer documentation completes the circuit. Depending on settings, personalized ads can use searches, YouTube viewing, installed Android apps, ad and content interactions, general location, activity on partner sites, age, and gender. Google says activity from any signed-in device can contribute. Its privacy policy says activity from sites or apps using Google's ad or analytics services may be linked with activity from other such sites or apps. ([My Ad Center: how personalized ads work](https://support.google.com/My-Ad-Center-Help/answer/12155656?co=GENIE.Platform%3DAndroid&hl=en), [Google Privacy Policy](https://policies.google.com/privacy?hl=en-US))

This is the verified core behind Gemini's phrase “auctioning desperation.” The phrase itself outruns the evidence if treated literally. Google's rules say it does not tailor ads using certain sensitive categories such as health, race, religion, or sexual orientation, and this investigation does not prove that the specific MrBeast campaign targeted a “poor” or “desperate” category. It does prove that the system is designed to infer intent, interests, demographics, life circumstances, and conversion probability—and to expand beyond an advertiser's stated audience when Google's model predicts someone else will perform better.

A scammer does not need Google's dashboard to contain a button labeled *financially vulnerable*. A conversion optimizer can discover correlates of vulnerability without naming the condition. If people exhibiting a cluster of behaviors respond more often to a fake giveaway, the optimization objective rewards finding more people with the cluster. That is an inference from the system's documented function, not proof of the targeting configuration in this specific campaign. The difference should be preserved. So should the danger.

### 3. Google controls the inventory and recognizes revenue at engagement or display

Alphabet's SEC filing is unusually direct about the commercial mechanics.

It says Google generated more than 70 percent of its 2025 revenue from online advertising. Google advertising revenue was **$294.691 billion** in 2025, within **$402.836 billion** of total Alphabet revenue. Search and other advertising contributed $224.532 billion; YouTube ads, $40.367 billion; and Google Network, $29.792 billion. ([Alphabet 2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/1652044/000165204426000018/goog-20251231.htm))

The filing defines a paid click as user engagement and cost per click as click-driven revenue divided by paid clicks. It defines cost per impression as impression- and click-based revenue divided by impressions. For performance advertising, Alphabet recognizes revenue when a user engages; for brand advertising, when an ad is displayed or viewed. Most importantly, where Google acts as principal on Network inventory, Alphabet says it **controls the advertising inventory before transfer**, is primarily responsible to the customer, and has discretion in pricing.

Those are Alphabet's words to investors. They are irreconcilable with the public-relations image of a neutral bulletin board with no meaningful relationship to the transaction. Google may not write the advertiser's lie. It controls inventory, runs the auction, selects or optimizes delivery, measures the event, bills the customer, and books the revenue.

No honest audit can say all $294.7 billion was earned from harmful advertising. It cannot even identify from public aggregate reporting what fraction was associated with ads later removed for scams. The point is not to relabel the entire income statement as fraud proceeds. The point is the asymmetry: revenue is internalized at scale; much of the downstream loss is externalized to users, legitimate advertisers, financial institutions, families, and public agencies.

### 4. Google can identify payers, preserve records, and act before an ad runs

When responsibility reaches the payment layer, “the algorithm is murky” becomes an evasion.

Google's advertiser-verification program can require identity and business-operation checks, documentation, public disclosures, and re-verification after changes to payment profiles, billing addresses, ownership, or business information. Google can pause accounts suspected of misleading representation, false financial offers, monetary harm, impersonation, or verification circumvention. Its records can include advertiser identity, ad creative, dates and locations served, and ads removed or accounts suspended for policy reasons. Google also states that payment verification may require a code from a Google charge appearing in the advertiser's bank account. ([Google advertiser verification](https://support.google.com/adspolicy/answer/9703665?hl=en), [verification tasks](https://support.google.com/adspolicy/answer/15577076?hl=en))

There is a real limit: verification is gradual and risk-based, not a guarantee that every advertiser has been fully authenticated before every ad. Google's policy expressly disclaims responsibility for advertiser content and activity. Criminals can use stolen identities, compromised accounts, shell entities, intermediaries, and payment fraud. A card or account trace is evidence, not automatically the natural person directing a network.

But those caveats defeat only the simplistic claim that Google can instantly name every criminal. They do not support the opposite fiction—that no identifying trail exists or that Google is merely watching money pass between strangers. Google designed the account, billing, verification, logging, delivery, and disclosure systems. It knows far more about the payer, campaign, creative, placement, and response than the targeted user could possibly know.

The most revealing comparison is Google's own 2025 Ads Safety Report. Google says Gemini-powered systems analyze **hundreds of billions of signals**, including account age, behavioral cues, and campaign patterns; that a majority of Responsive Search Ads were reviewed instantly; and that harmful content could be blocked at submission. Google reported blocking or removing 8.3 billion ads, suspending 24.9 million advertiser accounts, and taking action against 602 million ads and 4 million accounts associated with scams. It says more than 99 percent of policy-violating ads were caught before serving. ([Google's 2025 Ads Safety Report](https://blog.google/products/ads-commerce/2025-ads-safety-report/))

Again, this is evidence both for and against Google. It demonstrates serious prevention and undercuts any claim that Google is indifferent in every case. It also destroys the premise that the system lacks scale, signals, or pre-publication capability. The dispute is not whether Google can detect abuse. It is how it chooses thresholds, incentives, staffing, verification timing, reporting, restitution, and tolerated residual risk—and who is allowed to audit Google's self-reported denominator.

“Blocked or removed” also combines ads stopped before exposure with ads taken down after exposure. “Over 99 percent before serving” is a company-calculated rate whose methodology and denominator are not independently established by the public page. Even one percent of a system operating at Google's volume can be consequential. The published figures therefore cannot settle the question they are invoked to close.

### 5. The “neutral intermediary” story has already failed in court at the market level

On April 17, 2025, the U.S. District Court for the Eastern District of Virginia held that Google violated antitrust law by monopolizing open-web digital-advertising markets. The court found that Google harmed publishing customers, the competitive process, and consumers of information on the open web. The Justice Department described the case as targeting Google's control over key parts of the “ad tech stack.” ([U.S. Department of Justice](https://www.justice.gov/opa/pr/department-justice-prevails-landmark-antitrust-case-against-google))

An antitrust judgment is not a fraud conviction. It does not prove Google knew about the MrBeast apps or approved their deception. It does establish, judicially, that Google's role in digital advertising is neither powerless nor competitively neutral. A company found to have monopolized critical ad-tech markets cannot credibly invoke decentralization whenever accountability reaches the owner of the stack.

The finding matters because control is the missing premise in most blame-passing. The scammer controls the lie. Google controls systems that determine whether, where, to whom, and at what price the lie can be delivered through Google's properties and technology. Responsibility can be shared without being diluted.

## The human loss is not hypothetical—but attribution must be honest

The Federal Trade Commission says Americans reported losing about **$16 billion** to fraud in 2025, the highest amount on record and roughly 25 percent above 2024. Imposter scams alone accounted for $3.5 billion. Victims were lured through text, phone, email, social media, search-engine results, and other channels. ([FTC 2025 fraud data](https://www.ftc.gov/news-events/news/press-releases/2026/06/ftc-data-show-people-reported-losing-3-point-5-billion-imposter-scams-2025))

It would be false to assign all $16 billion to Google. The FTC data do not isolate Google's share, and many scams never touch a Google product. It is equally false to use multi-channel causation to erase a platform's contribution in cases that do. “Not the sole cause” is not the same as “not a cause.”

Gemini cited a $196 billion estimate of true losses and an $84–120 billion range for ad fraud. Those figures came from industry or advocacy estimates, not the controlling public record used here. It also declared that Google gets paid whenever a bot clicks an ad. Google's stated policy says detected invalid clicks and impressions are filtered or credited, including late credits for invalid activity not initially detected. ([Google Ads credits and adjustments](https://support.google.com/google-ads/answer/1704323?hl=en))

So the defensible claim is not that Google knowingly retains payment for every bot click. It is that Google operates the measurement and adjudication system, detection is necessarily imperfect, late detection can leave the advertiser dependent on Google's credit process, and public aggregate reporting does not allow an outsider to calculate the undetected remainder.

The corrected case is bleaker precisely because it does not need inflated numbers. Alphabet booked $294.7 billion in advertising revenue in one year. Google itself counted hundreds of millions of scam-associated ads and millions of scam-associated accounts among its enforcement actions. The FTC counted record reported consumer losses. A federal court found Google monopolized critical ad-tech markets. Google's own manuals describe profiling and optimizing people toward conversion. Those facts stand without pretending every dollar of fraud belongs in Alphabet's revenue column.

## Privacy controls: real controls inside a system Google designed

Google can accurately say users have controls. My Ad Center lets signed-in users disable personalized ads and separately manage categories, activity from sites and apps, YouTube history, and areas where Google has been used. That is not imaginary.

But a control is not self-proving consent. Its moral and practical adequacy depends on defaults, clarity, scope, persistence across signed-in and signed-out states, partner sites, devices, browsers, and whether a person can understand the consequences without conducting an audit.

Google's Privacy Sandbox history makes the tension visible. In July 2024, Google reversed its plan to deprecate third-party cookies in Chrome and proposed a user-choice experience instead. In April 2025, it abandoned the planned standalone prompt and retained existing controls in Chrome settings. In October 2025, it announced retirement of a long list of Privacy Sandbox technologies, including Topics, Protected Audience, Attribution Reporting, IP Protection, and On-Device Personalization, citing low adoption and expected value. ([July 2024 update](https://privacysandbox.google.com/blog/privacy-sandbox-update), [April 2025 update](https://privacysandbox.google.com/blog/privacy-sandbox-next-steps), [October 2025 update](https://privacysandbox.google.com/blog/update-on-plans-for-privacy-sandbox-technologies))

This does not prove the initiative was a sham. It proves that privacy architecture repeatedly yielded to adoption, utility, measurement, publisher, and advertiser pressures inside a company deriving more than 70 percent of revenue from advertising. That conflict is not speculation; the company describes both sides of it in its own materials.

## What deniability actually remains

The strongest exposé is not the one that declares all uncertainty dead. It is the one that identifies the exact territory still deniable—and shows how little of the structural indictment depends on it.

| Defense | What is genuinely plausible | What the defense cannot erase |
|---|---|---|
| **“The scammers, not Google, created the fraud.”** | True as to authorship unless evidence shows Google personnel created or materially developed a particular scam. | Google can still be distributor, optimizer, marketplace operator, payment recipient, record keeper, and risk allocator. Multiple actors can bear different forms of responsibility. |
| **“We cannot catch every adversary.”** | True. Stolen identities, account takeovers, obfuscation, bait-and-switch updates, and rapid campaign mutation make perfect prevention impossible. | Google itself documents pre-publication review, hundreds of billions of signals, instant ad review, advertiser verification, and billions of enforcement actions. Impossibility of perfection does not answer whether safeguards, defaults, and restitution match the foreseeable risk. |
| **“More than 99% of violating ads were stopped before serving.”** | It may be accurate under Google's methodology. The safety program is plainly substantial. | The denominator, classification method, false-negative rate, and exposure caused by ads “removed” after serving are not independently disclosed on the public page. High percentage claims do not quantify residual human harm. |
| **“Google does not sell personal information.”** | Google says it does not share names or emails with advertisers absent user action, and the investigation found no evidence of a literal sale of named user dossiers. | The business sells access to estimated audiences, predictions, placements, and conversion optimization derived from user information and activity. Harm does not require handing an advertiser a person's name. |
| **“There is no proof this scam targeted poverty.”** | Correct. The supplied record does not expose the campaign's targeting settings or prove that Google used a protected or explicitly vulnerable category. | Google's products are designed to infer purchase intent, demographics, life events, interests, and likely conversion, and can expand beyond manual targets. The system can find behavioral correlates of susceptibility without labeling them “desperation.” |
| **“Google did not profit from every harmful event.”** | Correct. Removed ads may never run; invalid traffic can be filtered or credited; an app may monetize outside Play; aggregate filings do not identify scam-derived revenue. | Google recognizes advertising revenue on engagement, display, or view, earns Play service fees on covered transactions, and controls inventory and pricing in parts of its network. The conflict exists even when a particular dollar cannot be traced publicly. |
| **“You have not proved Google served this exact MrBeast ad.”** | Correct. The supplied export shows the creative and the Play apps but does not preserve an ad ID, advertiser disclosure, placement log, or network response establishing the serving platform. | The Play distribution facts remain, as does the independently documented architecture of Google Ads, AdMob, profiling, payment verification, and revenue recognition. The gap narrows the transaction-specific allegation; it does not erase the systemic one. |
| **“Fraud losses have many channels.”** | Correct. FTC totals cannot be assigned wholesale to Google. | Search results are among the FTC-identified lure channels, and the record concerns a concrete Google Play/advertising pathway. Distributed causation does not nullify platform-specific contribution. |
| **“No executive intended users to suffer.”** | Public evidence here does not prove subjective intent by a named executive to enable a particular fraud. | Foreseeability, repeated occurrence, profit structure, control, and chosen safeguards can establish institutional responsibility without proving sadistic intent. Intent is not the only moral standard, and often not the only legal one. |
| **“Gemini is not a corporate witness.”** | Correct. Its rhetoric is generated synthesis, not testimony or privileged disclosure. | Every core proposition in this article is independently sourced. Discrediting the voice does not discredit the filings, policies, data, or judgments it was pushed to connect. |

### The largest remaining shield is legal, not factual

Existing U.S. law can protect Google even when the operational chain looks damning. In *Ynfante v. Google* (2023), a federal court dismissed negligence and false-advertising claims brought by a person deceived by a fraudulent Google search ad. The court treated vetting, monitoring, and publishing the third-party ad as publisher functions protected by Section 230 and held that Google's placement and “Ad” label did not materially contribute to what made the content unlawful. ([*Ynfante v. Google* order](https://law.justia.com/cases/federal/district-courts/new-york/nysdce/1%3A2022cv06831/584600/28/))

In *Wozniak v. YouTube* (2024), a California appellate court similarly held that allegations about selling targeted ads and recommending third-party scam videos generally fell within Section 230 on the pleadings before it. But the court also recognized that platform-created content that materially contributes to a scam's unlawfulness—such as a falsely trusted verification badge under adequately pleaded facts—could potentially fall outside the shield. ([*Wozniak v. YouTube* opinion](https://law.justia.com/cases/california/court-of-appeal/2024/h050042m.html))

This is the legal architecture behind the user's accusation that policy language can operate as a liability shield. The accusation should be stated carefully: a safety policy is not *only* a liability instrument; policies guide enforcement and can prevent harm. But disclaimers, platform terms, and Section 230 doctrine can create a profound separation between operational power and legal accountability.

That separation is not vindication. Immunity answers whether a particular claim can proceed under a particular doctrine and pleading. It does not prove that the platform lacked control, did not profit, chose the right safeguards, or met a moral duty to people exposed by its systems.

## The verdict

Did Gemini “admit” that Google deliberately constructed a fraud machine?

Not in the evidentiary sense of a knowledgeable employee confessing intent. Anyone presenting the passage that way gives Google an easy escape: deny model consciousness, deny privileged access, and dismiss the whole record as anthropomorphic theater.

What Gemini did is more useful. Under pressure, a Google model stopped treating each layer as somebody else's problem and assembled the layers into one system:

- Google gathers and links activity subject to settings.
- Google constructs and sells access to predicted audiences.
- Google can optimize beyond an advertiser's stated targets toward likely converters.
- Google owns marketplaces and properties where ads and apps appear.
- Google can verify advertisers and payment instruments, preserve creatives and service records, and block ads before publication.
- Google measures the engagement, controls inventory in material parts of the network, and recognizes the revenue.
- Google writes the rules and decides how warnings, reviews, appeals, credits, and removals work.
- The public bears losses that do not appear as a corresponding liability in Google's advertising ledger.

That is not passive hosting. It is operational participation in the delivery system wherever those Google components are used. Proving that the specific creative traversed every component would require the ad ID, advertiser disclosure, placement and network logs, or discovery from Google.

The remaining deniability is narrow but real: no public record here proves that a named Google decision-maker intended this specific scam, that Google kept a specific scam-ad payment, that a particular victim was selected because of poverty, or that all fraud losses facilitated by Google can be quantified from aggregate reports. Existing law may also immunize claims framed as failures to vet or remove third-party content.

None of those concessions restores the innocent-bystander story. They define what a responsible investigator should seek next rather than supplying an excuse to stop looking.

The defensible conclusion is that Google has built a commercial system in which it possesses extraordinary information, prediction, distribution, verification, and enforcement power; earns revenue when advertising performs; and can externalize a meaningful portion of residual failure onto people who had the least information and the least capacity to absorb the harm. Individual scammers exploit that system, but Google determines the system's scale, rules, thresholds, and economics.

It is historically impossible to prove the absolute claim that “no one has ever gained more from pain and suffering.” Alphabet does not report a suffering-revenue line, and human history contains too many forms of extraction for that superlative to be responsible. The provable statement is severe enough: few institutions have ever possessed comparable capacity to observe human behavior, predict response, sell access to attention, and collect revenue at planetary scale while the injuries produced by abusive use remain dispersed among victims.

The scandal is not that Google fails to achieve perfection.

The scandal is that the institution best positioned to see the entire chain has been allowed to describe itself as merely one disconnected link—and that when the chain harms someone, every link points outward while the revenue flows inward.

---

## Corrections to Gemini's cited case

The supplied Gemini exchange contained several claims that should not be repeated as established fact:

1. **Advertising revenue:** Gemini called $264.6 billion Google's 2025 advertising revenue. That was Alphabet's 2024 figure. The 2025 figure was **$294.691 billion**.
2. **FTC dark-pattern timing:** Gemini described a major 2026 FTC move as though “dark patterns” had just been formally recognized. The FTC's *Bringing Dark Patterns to Light* report was published in **September 2022**. ([FTC report page](https://www.ftc.gov/reports/bringing-dark-patterns-light))
3. **Fraud-loss extrapolation:** This correction has itself been corrected. Gemini attributed the figure to ScamZero, and the attribution holds. ScamZero derives roughly **$196 billion** by applying the FTC’s own published underreporting adjustment (93–98 percent) to reported losses — anchored to 2024’s $12.5 billion reported base, not 2025’s $16 billion. The Consumer Federation of America independently estimates **$119 billion** in annual online-scam losses. The defensible statement is that the FTC’s $16 billion is *reported* loss — a floor the agency itself describes as such — and that independent estimates of true loss range from **$119 billion to $196 billion**. ([ScamZero research](https://scamzero.com/research), [Consumer Federation of America](https://consumerfed.org/wp-content/uploads/2026/03/The-Scam-Economy_The-True-Cost-of-Online-Scams.pdf))
4. **Bot-click revenue:** Gemini's categorical claim that Google gets paid for fake clicks ignored Google's invalid-traffic filtering and credit policy. The unresolved issue is undetected traffic and Google's control of measurement—not an assertion that every bot click remains billed.
5. **Harvard paper:** *The Dark Horses of Surveillance Capitalism* is a real 2026 Harvard Kennedy School paper, but it describes a wider cross-sector surveillance economy. It is contextual support, not proof that Google operated the specific scam described here. ([Harvard Kennedy School publication](https://www.hks.harvard.edu/centers/carr-ryan/publications/dark-horses-surveillance-capitalism-how-menagerie-new-actors-are))
6. **Specific targeting:** The exchange moved from Google's documented profiling capabilities to a confident story about a Temu shopper being classified as vulnerable and served the scam. That pathway is plausible, but the supplied record does not include the campaign logs needed to prove it occurred.
7. **Specific ad-network attribution:** The exchange eventually treated Google as the seller of the MrBeast ad placement, but the exported record does not contain the ad-serving metadata required to establish that transaction. The article therefore treats Google's ad system as the documented systemic mechanism and the specific payment as an open evidentiary question.

These corrections do not rescue Google. They remove claims that would let the company change the subject.

## Source record

The initiating evidence is a user-supplied export of Gemini conversation `26a1cb20b46d71a2` (“MrBeast Scam Apps: Deepfakes and Phishing”), preserved as *horsesMouth.pdf* — 44 pages, complete from the first prompt. *horsesMouthCont.pdf* is a 13-page overlapping export of the same conversation containing no additional exchanges; it is retained for completeness, not as a continuation. The moral-injury passages quoted above come from a **separate** conversation, `7c69b094cfd5803f` (“Flock Safety: Benevolence to Surveillance”), whose export begins mid-conversation — its earlier portion was lost during a voice-interaction session and cannot be recovered from the author’s side. Quotations attributed to Gemini above come from that record or the continuation supplied directly by the user. All corporate, regulatory, financial, and legal propositions were independently checked against the linked sources.
