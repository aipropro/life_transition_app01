# App decision: Life Transition App 01

**Decision (5 Sep 2026): build Gray-Divorce Money + Admin Reset.**
A 90-day paid program for women 50+ who have just separated or received a decree.

Source: "Life-transition app opportunities" deep-research report, 3 Sep 2026 (8 ranked concepts).

## Why this one for a build-and-launch sprint

- Score 82/100, second overall, best fit for content or creator-led acquisition.
- Build shape is CRUD plus content: roadmap, checklists, document vault, deadlines, budget snapshot, PDF export. No clinical safety review, no expert video library, no institutional sales cycle.
- One-time 90-day program (test $99 vs $149). A finite event does not need a subscription.
- Whitespace: Anchor and Divorce SOS bundle emotional recovery, OurFamilyWizard owns co-parenting, Hello Divorce owns filing. Post-decree execution for older women is narrower and less crowded.

## Why not the other top picks (for a sprint)

- #1 Hospital-to-Home Caregiver Copilot (84): AI extraction of medications with human confirmation, health-data obligations (FTC Health Breach Notification Rule), B2B2C sales through discharge teams. Highest upside, slowest to launch, highest liability.
- #3 Bone-Safe Strength 50+ (81): needs expert-reviewed exercise videos and safety review. Content production is the bottleneck.
- #4 Local-language Menopause Navigator (80): needs clinicians and validated Malay instruments, lower ARPU. Good second-country play later, not a sprint app.

## Sprint multiplier: one engine, several apps

#2 Gray-Divorce (82), #5 Widows' First 100 Days (78) and #7 Solo-Ager Life Binder (76) share one product shape: stage roadmap + checklists + document vault + deadline calendar + exportable packet. Build the engine once with swappable content packs.

1. App 1: Gray-Divorce Money + Admin Reset (now).
2. App 2: Widows' First 100 Days (new content pack; funeral-home, adviser or insurer channel).
3. App 3: Solo-Ager Life Binder only if a distribution partner appears (report warns of a clone wave).

## v1 scope (ship this, nothing more)

Include:

- Onboarding: stage (pre-filing, pending, decree received, post-decree), country/state, situation flags (home, retirement accounts, business, dependants).
- Stage roadmap: generated task list with deadlines. Each task has why, how, and what to bring.
- Document inventory: required-documents checklist plus secure upload.
- Deadline calendar with email or push reminders.
- Cash-flow reset: one-page before/after budget snapshot.
- Checklists: accounts, housing, insurance, tax documents, passwords, emergency contacts, beneficiaries.
- QDRO and retirement task tracker (status only, no advice).
- Export: professional meeting packet (PDF) for a lawyer or Certified Divorce Financial Analyst.
- Paywall: one-time Reset Pass, A/B $99 vs $149, covering the 90-day program plus 12 months of vault, calendar and reminders. Optional renewal after month 12 at about $39.99 a year for the vault and long-dated reminders. Expert sessions sold separately. No document-generation add-ons (unauthorized-practice risk).

Exclude (report's explicit list): co-parenting messaging or evidence logs, therapy or crisis AI, dating, fitness, beauty or community, automated legal or investment advice.

Guardrail: the app tracks and organizes. It never advises. Every screen carries "not legal or financial advice".

## Validation in parallel with the build

The report wants a 30-day validation before software. In sprint mode run it alongside the build:

- Day 1: landing page with the promise ("In 90 days, know what you own, what must change, which deadlines matter, and which professional to call"), price cells $99 / $149, refundable deposit.
- Three problem-led creatives: "the 12 accounts people forget", "what changes when the decree arrives", "the retirement checklist after divorce".
- Gates before paid acquisition: 3+ deposits, 5+ users complete the roadmap, one CDFA or family-law partner agrees to a second conversation.

## Reality check from the report

14,700+ new subscription apps per month. Median monthly revenue one year after launch is $72. 69% of revenue goes to apps launched before 2020. Launch volume does not beat that curve; distribution and trust do. Every app in this sprint needs a channel at launch, not after.

## Multi-country strategy (5 Sep 2026)

The engine is built once for every market: stage roadmap, checklists, document vault, deadline calendar, budget snapshot, export, i18n, currency and date formats, per-jurisdiction deadline rules loaded from content files. The content is built per jurisdiction, never per language: pensions, tax, health insurance, name change and deadlines differ between countries that share a language (US vs UK, Spain vs Mexico, Germany vs Austria, Brazil vs Portugal). Each content pack needs local-language research, a local professional's review, a local privacy policy and terms, local pricing and payment methods, a localized store listing, support in the language, and maintenance when the law changes.

Launch wide with demand tests, launch the product in waves:

- Now: translated waitlist landing pages with a price test for every candidate country. They cost almost nothing and show which packs are worth building.
- Wave 1 (launch): US, UK, Canada, Australia. One language, four content packs.
- Wave 2: Japan. Own content pack, Japanese UI and support, MSCA payment setup, price about ¥4,980-9,800.
- Wave 3: Germany, France, Spain on one GDPR and DSA build. Three content packs.
- Wave 4: Brazil if the waitlist signal justifies it. Pix and boleto, LGPD, low price.
- Same-language neighbours (Austria, Switzerland, Mexico, Argentina, Ireland, New Zealand, Portugal) only after the first pack in that language ships, each as its own smaller pack.

## Research status (5 Sep 2026)

Two deep-research passes were run after this decision. Results:

- `docs/research/english-market-planning-brief.md`: competitors and pricing, demand by country, the US deadline table, UK/Canada/Australia modules, channels and legal boundaries, monetization benchmarks, and the brainstorm question list.
- `docs/research/non-english-market-pick.md`: ranking of 12 non-English markets. Pick: Japan first, Germany second, South Korea third.
- `content/checklists/us-post-decree.json`: the US checklist as structured app content (4 stages, 45 tasks).

Launch sequence: US, then UK/Canada/Australia on the same engine, then Japan (new language, content and payment stack), then Germany and the rest of the EU on one compliance build.

External runs merged on 6 September 2026: the C1 audit (corrections applied), the P1 and P3 channel maps (`docs/research/channels-english-markets.md`, `docs/research/channels-japan.md`), the P2 competitor check (Anchor exists, 3 ratings; no one-time-purchase, beneficiary or QDRO tracker in any competitor), the G9 country counts, and the G1 England and Wales pack (`content/checklists/uk-england-wales-post-decree.json`, pending audit).

Still open: keyword volumes, employer EAP and relocation partners, the C2 audit of the UK pack, and the G2-G8 packs for Canada, Australia, Japan, Germany, France, Spain and Brazil.

Assumptions: consumer-direct launch, no clinical or institutional partners yet, US market first, web-first before app stores.
