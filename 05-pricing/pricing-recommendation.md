# Pricing Recommendation · Roamly Groups

## 1. Pricing goal

- **Goal:** Grow revenue from a known audience

## 2. Pricing model

- **Model:** Subscription
- **Who pays, and for what:** Each traveler pays their own share of the trip, plus their share of a small service fee, at the moment of booking. Planning and voting are free. The fee is charged only when the group actually books through Roamly, so the cost is tied to a booked trip and split across the group instead of landing on the organizer.

## 3. Packaging

- **Tiers:**
  - Tier	| Who it’s for	| Rough price
  - Plan (Free)| 	Every group; the traveler who just wants in	| $0
  - Book ← most customers pick this	| The organizer who wants the trip booked and paid | ~5% service fee on bookings, split per person
  - Roamly Pro	| The frequent organizer / trip leader	| ~$89/year, waives the fee for their whole crew + perks

## 4. Assumption to test

- **The one assumption I would test before launch:** Will groups book through Roamly, or plan for free and book the experiences directly to dodge the fee? If that leakage is high, the transaction model collapses and the whole recommendation changes.

## 5. One-page recommendation

### Pricing Recommendation · Roamly Groups
**For:** Finance, Sales Leadership, Product Marketing

#### Recommendation
Free to plan, a small capped fee when the group books, and a Pro subscription that waives the fee for frequent organizers. Monetize the booking, which is both where value lands and where our only real cost (Plaid) fires.

#### Goal
Grow revenue from a known audience. Roamly already has travelers booking solo; Groups turns that base into higher-value group bookings. Not a new market, not a defense.

#### Model
Transaction-based core, Pro subscription on top. Group trips happen 2-3 times a year, not continuously, so a flat subscription misprices the value. The fee rides the booking; each traveler pays their own share plus their share of the fee, so nobody fronts and the organizer isn't stuck with it.

#### Tiers
| Tier | Who | Price |
|---|---|---|
| Plan (Free) | Every group; the traveler who just wants in | $0 |
| **Book** ← most pick this | The organizer who wants the trip booked and paid | ~5% fee, capped ~$8/person |
| Roamly Pro | The frequent organizer / trip leader | ~$89/yr, waives the fee for the whole crew + perks |

#### What each stakeholder needs to hear
**Finance.** Revenue scales with booked-trip GMV, and the margin floor is the per-transaction Plaid cost, so price is tied straight to the cost driver. Transaction revenue is less predictable than a subscription, so Pro is the recurring line and GMV drives the forecast. Free Plan carries almost no COGS, so it's a cheap adoption cost, not a margin drain.

**Sales Leadership.** Not a seat-based motion. The organizer is the growth engine: Pro waives the fee for their whole crew, so every Pro organizer pulls their group in. The fee is sellable because it's small, capped, and split. Self-serve, organizer as champion, no long cycle.

**Product Marketing.** Tiers map to the two audiences: Plan is the traveler on-ramp, Book is the organizer hero (mark it "Popular"), Pro is the frequent organizer. Lead with value, not the fee, and anchor the fee against the trip total ("$8 on a $600 trip"), never as a naked percentage. Pro headline: your crew books fee-free.

#### Assumption to test
Will groups book through Roamly, or plan for free and book the experiences directly to dodge the fee? High leakage collapses the model.

**Method: Conjoint (choice-based, with an outside option).** The assumption is a behavioral tradeoff, book in-platform at a fee vs. book direct for free, so you need a method that models the whole-package choice and lets you vary the fee. Include "book direct" as the outside option and read substitution as a function of fee level. Van Westendorp only finds an acceptable price band with no competing alternative; Max-Diff ranks features but never models the book-here-or-direct choice. Conjoint is the only one that simulates the actual decision.
