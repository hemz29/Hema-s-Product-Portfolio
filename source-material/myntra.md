# Myntra concept — source notes and draft article

Sources: `myntra-phase1.pdf` (discovery), `myntra-phase2.pdf` (user research), `myntra-phase3.pdf` (solution, prototype and PRD).
Prototype: https://true-fit-visuals.lovable.app
Walkthrough: https://www.loom.com/share/21982a6985fd459fb197fb85500e8a68
**Note:** this is an independent concept, not affiliated with Myntra. The site should say so in one line and must not use Myntra's logo.

## Key facts to use
- **Phase 1 (discovery):** Hema audited the app as a 10+ year customer. Friction points: returns rejected for a brand tag that was missing on delivery, one-by-one cancellation, product-only help, chats that time out, and three confusing reward types. She studied the business model (4–5% commission, marketplace, logistics, ads, and M-Now 30-minute delivery), competitors (Nykaa, FirstCry, Amazon, Lifestyle), and segments of 200M annual, 80M monthly and 60M weekly users. She listed 15 user problems and picked 3 to probe. Goal: **retention of busy working professionals**.
- **Phase 2 (research):** a screener, then 5 interviews (3 women and 2 men, aged 35–55) and a survey (29 responses; the findings table uses /24). **[TODO: confirm 29 vs 24]**
  - **The hypothesis largely failed.** "Returns rejected for a missing tag" was only 2/5 interviewees and 0/24 survey respondents, and the one person who hit it found the ticket easy to raise.
  - **What the research found instead:**
    - 4/5 interviewees and 15/24 survey respondents don't buy anything over ₹5K online. They want to check quality, authenticity and fit in a store. "Anything more than 5000 is expensive and I prefer buying that from a (physical) store."
    - 4/5: when an item doesn't match its listing, the return process treats it as the customer's fault. "If wrong product is delivered, they don't take return saying product is different from the image."
    - 2/5: customer support has no memory across interactions. "Customer care kept asking same questions every time… Had to raise an issue on LinkedIn tagging Myntra, then got immediate reply."
    - 3/5: mismatches happen mainly with smaller tier-2 brands.
  - **Behaviour change:** shoppers stick to known brands and stop trying new ones. That hurts tier-2 sellers and Myntra's catalogue breadth.
- **Persona:** Riya, 38, a software engineer at an MNC. She cares how she presents at work. She is loyal to Myntra, but after a few disappointments she only buys tier-1 or celebrity-endorsed brands.
- **Reframed P0:** "When a delivered item doesn't match its listing, Myntra's return process puts the burden of proof on the customer… This makes the users stick to known brands and not explore any new ones."
- **Solutions scored with RICE (1–3 scale):** images under different lighting (2), **skin-tone slider on the model (3)**, a private AI avatar (1.33), **a "most returned" flag (6, the winner)**, a fit/colour comparison with past purchases (2), Try-Buy for new brands (2.66).
- **Chosen solution: Product Return Transparency Indicator.** It shows the return rate for each SKU, graded Low (0–10%), Moderate (11–30%) or High (>30%), plus the top return reasons in a tooltip. It sits in the Product Details section. Customer support sees it too, so agents resolve returns fairly and faster. Empty states: "never been returned" and "returns history unavailable". It is a pattern already proven on Amazon.
- **Prototype also includes the skin-tone slider** (idea #2), per Hema.
- **Metrics:** primary is a reduction in returns. Secondary are more browsing of tier-2 brands and fewer drop-offs when a tier-1 item is unavailable. **Guardrail:** watch sales of products flagged as high-return (the flag may kill those sales).
- **Risks:** customers may not notice the flag (50%), mitigated by A/B testing the placement (on the image vs in details). SKU-level data may be missing (10%), mitigated by launching where data exists and collecting it now.
- **Non-goal:** fixing the pick-up process.
- Small note: the grading bands in the PRD (0–10, 11–30, >31) leave gaps at 10–11% and 30–31%. The article uses ≤10 / 10–30 / >30.

## Draft feature article

**Kicker:** Commerce · Product discovery
**Headline:** My hypothesis was wrong. The research found a better problem.
**Standfirst:** I set out to fix a returns annoyance on India's biggest fashion app. Interviews showed the real cost was quieter: shoppers stop trying new brands. The result was a return-rate badge and a skin-tone slider, prototyped end to end.
**Meta:** Independent concept, not affiliated with Myntra · Discovery, research, prioritisation, PRD and prototype · 2026 · [Try the prototype →](https://true-fit-visuals.lovable.app)

**Starting point.** After ten years as a customer, I had a pet frustration. A pricey order arrived without its brand tag, and then the return was rejected *because* the tag was missing. I mapped the app, the business model, competitors and segments, and listed 15 problems. This one went to research first.

**What the research actually said.** I interviewed five busy professionals and surveyed 29 more. My problem barely registered: no survey respondent had hit it, and the one interviewee who had found the fix easy. What came up again and again was something else. When an item doesn't look like its photos, the return feels like the customer's fault. "They don't take return saying product is different from the image." Mismatches clustered on smaller brands. So shoppers adapted the safe way: **they stopped trying new brands.** 15 of 24 won't spend over ₹5,000 online at all.

**The reframe.** The problem wasn't returns. It was *confidence before purchase*, and it was quietly costing tier-2 sellers and catalogue breadth.

**Choosing what to build.** I scored six ideas with RICE, from lighting-accurate photos to a personal AI avatar. Two went into the prototype:
- *Return Transparency Indicator* (scored highest): every product shows its return rate (Low / Moderate / High) and the top reasons people sent it back. Support agents see the same data, so they can't brush off a legitimate return.
- *Skin-tone slider:* adjust the model's complexion to see how a colour will look on you, not on a studio model.

**Measuring it honestly.** Primary: fewer returns. Secondary: more browsing of tier-2 brands. Guardrail: the badge will hurt sales of high-return products, which should be watched, not hidden. The biggest risk is customers not noticing it, so the first step is an A/B test of where it sits.

**Pull quote:** "Shoppers didn't complain about returns. They quietly stopped taking risks."

**What I'd do next.** Test the badge placement with two cohorts, then try lighting-accurate images for tier-2 brands.

**[TODO: screenshots of the badge, the tooltip and the slider from the Lovable prototype.]**
