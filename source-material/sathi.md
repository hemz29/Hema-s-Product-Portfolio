# Sathi — source notes and draft article

Sources: `sathi-prd.pdf` (Final MVP PRD), `sathi-research-deck.pdf` (research and strategy deck, Sept 2026).
Live: https://sathi.today
Walkthrough: https://www.loom.com/share/c1a01be807234efb892fb9b59db5e2b8
PRD (Drive): https://drive.google.com/file/d/1nZm_xj76WhBA5_9rWWMsBQWU4kzo1E9U/view?usp=drive_link

## Key facts to use
- **What it is:** a mobile-first digital scam-safety companion for Indian senior citizens. Tagline: "Safer with every tap".
- **Problem:** seniors make up 4.5% of reported frauds but 18% of losses by value, at a life stage with no income. Official guidance exists but is scattered, formal, and not designed for mobile or for seniors.
- **Scale of fraud (national, from deck):** 2024 ~19.19 L complaints / ~₹22,848 Cr; 2025 ~24.03 L / ~₹22,495 Cr; 2026 H1 ~12.71 L / ~₹10,178 Cr.
- **Research:** 5 in-depth interviews (1 woman, 4 men, 60+), then a survey for validation. The deck says 52 responses but the findings table uses /57. **[TODO: confirm which number is correct]**
  - 47/57 stay independent by following scam news in their social circles, and 17 of them have scams in their network.
  - 13/57 rely on family for some online tasks. 5/57 were scared after receiving a suspicious SMS or call. Some wouldn't even open the survey link: "Better not to take a chance."
  - 45/57 block or ignore unknown numbers, so genuine calls get lost in the noise.
  - Real quote: "Got a thorough briefing from my son on online payments… Large amount transfer only through Bank Trf NEFT or IMPS."
- **Segments:** affluent retirees, seniors with low tech literacy, seniors living alone, community leaders, caretakers. Pitfalls: fear and urgency, greed, lack of awareness, emotional manipulation, excessive trust.
- **Persona:** Mr Palani Swami, a retired Indian Air Force veteran who does most online tasks himself.
- **Competitors:** Truecaller Family Protection (Swedish company, not senior-specific), Khyaal (senior community with 50L+ users, but not focused on security), and the National Cyber Crime Portal (authoritative, but PDFs are hard to consume).
- **Prioritisation:** RICE. Bite-sized daily lessons from government sources scored 6. A live fact-check scored 9 but depends on an outside service, so it went on the roadmap.
- **Product principles:** trustworthy (government sources only), respectful (addresses users as "Name Ji"), reassuring rather than fear-based, one idea at a time, accessible, companion-led ("a reassuring Indian grandmother" voice).
- **MVP:** companion onboarding, time-aware greeting, 6 topics (WhatsApp, SMS and links, UPI, phone/vishing, digital arrest, investment), lesson cards with voice narration, MCQs with gentle feedback, a rotating 5-question knowledge check drawn only from completed lessons, streaks, a scam-avoidance journal, official reporting (cybercrime.gov.in and helpline 1930), and referrals.
- **Deliberate design choices:** no childish gamification, no fear imagery, confetti only for a perfect score and respecting reduced motion, no account needed, data stays on the device, no claims to auto-detect scams.
- **Out of scope:** real-time detection, reading messages or calls, bank integrations.
- **Roadmap:** live fact-check, a 1–5 "scare score" from red flags, alerts when the portal or helpline is back up, AI-enacted scenario videos, Indian languages, a family/caregiver experience.
- **Market:** 15 Cr senior citizens (10.5% of India), about 41% with smartphones, so roughly a 6 Cr addressable market.

## Draft feature article

**Kicker:** Society · Cyber safety
**Headline:** Teaching India's grandparents to spot a scam before it spots them
**Standfirst:** Seniors file fewer than 5% of India's fraud complaints but lose 18% of the money. Sathi turns scattered government advice into calm, daily lessons that seniors actually finish.
**Meta:** Personal project · Product, research, design and build · 2026 · [Try Sathi →](https://sathi.today)

**The problem.** A "CBI officer" calls with your name, your Aadhaar number and an arrest warrant, and tells you not to hang up or tell your family. Digital-arrest scams like this have taken life savings from retirees in Bengaluru, Hyderabad and Goa. The official advice that would have helped does exist, but it sits in government PDFs, written in formal language, and was never designed for a 70-year-old reading on a phone.

**What I heard.** I interviewed five seniors and then validated what I learned with a survey [52/57] responses. The surprise wasn't ignorance. Most respondents (47) actively follow scam news in their circles. The real cost was *fear*: 45 now ignore every unknown number, genuine ones included, and some wouldn't open my survey link at all. "Better not to take a chance." The goal changed from "warn seniors" to "give seniors back their confidence".

**The decisions.**
- *Government sources only.* Every lesson carries a credibility badge and a source link. Sathi never invents statistics or claims.
- *Respect over gamification.* No cartoons, no leaderboards. Users are greeted as "Name Ji" by a companion who sounds like a reassuring grandmother. Confetti appears only for a perfect score.
- *Learning before detection.* A live fact-checker had the highest RICE score (9), but it depends on outside services and risks false confidence. I shipped the education layer first and kept detection on the roadmap.
- *Privacy by default.* No account, progress stays on the device, and Sathi never reads messages or calls.

**What shipped.** Six topics drawn from real Indian cases (WhatsApp, SMS links, UPI, vishing, digital arrest, investment). Each has voice narration, practice questions with gentle feedback, and a rotating knowledge check built only from completed lessons. A scam-avoidance journal records the times you *didn't* fall for it. One tap reaches cybercrime.gov.in or the 1930 helpline.

**Pull quote:** "The goal changed from warning seniors to giving them back their confidence."

**What's next.** A red-flag "scare score" for live situations, short scenario videos, Indian-language support, and a caregiver view for adult children.

**Outcomes:** [TODO: any usage numbers, user feedback, or testimonials since launch?]
