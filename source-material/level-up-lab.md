# Level-Up Lab — source notes and draft article

Sources: repo https://github.com/hemz29/Level-up-Lab (README and docs, read 13 Nov 2026), plus the Claude Code build session.
Live: https://levelup-lab.vercel.app
Earlier name in the PRD: "Raaga's Study Companion". **[TODO: Hema to share the PRD if she wants it quoted. Should the child's name appear publicly? The draft says "my daughter".]**

## Key facts to use
- **What it is:** an installable, laptop-first PWA that helps school kids build a consistent, careful study habit on their own. First built for a Grade 6 ICSE student (Hema's daughter).
- **Core principle:** "The app does not teach content. It makes her show up, focus, work carefully and remember." The child studies from their own books, and the app is the coach and the game layer.
- **Game layer:** choose a world (Emberwick Academy, Lumenwood Sanctuary, The Drift Isles), get an egg, and grow a creature through Egg → Hatchling → Juvenile → Teen → Adult → Mythic using Growth Points. It hatches after the first 2 gated blocks. Missed days only make the creature sleepy. **GP is never lost**, so there's no punishment loop. Consistency is a rolling 5-of-7-day window. Play time earned (15 min base, up to 40 min a day, 1-day carry-over) unlocks creative rooms like an art studio where kids can redraw their own creature.
- **Plan builder:** 10 subjects and their chapters, each marked In portion / Probably / Not in portion, plus test dates. It auto-spreads a draft plan: max 3 blocks a day, Maths daily, revision touches for memory subjects, a Sunday "boss fight". Moved blocks survive a re-spread. Parents get a read-only "Want Mum to take a look?" view. Families can paste or upload the school's portion list.
- **Daily session:** a recall quiz when one is due, then up to 3 blocks, a detective briefing, a 25-minute focus timer (abandoning a block doesn't count), and 5-minute breaks.
- **"The gate" (the signature mechanic):** to finish a block, the child writes 5 takeaways (3 on a light day). Each needs ≥6 words and a concrete anchor: a name, number, year, place, "because", a unit, or a chapter key term. No pasting, no near-duplicates. The creature coaches gently when a point is vague. The aim is to stop "I studied" from meaning "I sat with the book open".
- **Mistake log:** 5 categories, with bonus play time for logging slips, plus a notebook showing "which slip costs you most".
- **Recall:** spaced repetition at 1, 3, 7 and 21 days, using the child's own questions or auto-generated fill-in-the-blanks. Answer first, then self-rate. Memory-heavy subjects are weighted higher.
- **Anti-gaming and wellbeing:** 1 light-day token a week, a nudge after 3 swaps away from the same subject, a PIN-protected parent pause, and an exam-week setting.
- **Report:** "Tell Mum how today went". The child sees the exact text before it's emailed to the parent. Unsent reports make the creature sleepy.
- **Worksheets:** printable practice sheets, 25-mark unit tests and 80-mark papers built from textbook-based question banks with page-referenced answer keys.
- **Accounts and privacy:** parents sign in by email code with no passwords, and children never need an email. Up to 6 children per family, cloud sync (Supabase) with offline support. The admin dashboard shows **usage numbers only**, and database rules block anyone, admins included, from reading families' notes or drawings. Full account deletion. **No ads, no third-party analytics, no web fonts, no AI.**
- **Engineering:** React + TypeScript, Zustand/IndexedDB, Vercel functions, Supabase. A pure, tested rules engine (74 unit tests). Every game number is tunable in one config file, to adjust after the trial week.
- **Phase 2 (teased as locked rooms):** a music corner, chess, and a runner game.

## Draft feature article

**Kicker:** Learning · Habit design
**Headline:** A study app that refuses to teach, and grows a dragon instead
**Standfirst:** Most study apps add more content. Level-Up Lab assumes the textbook is fine, and the hard part is showing up, focusing and remembering. A creature grows only when the work is real.
**Meta:** Personal project · Product, game design and build · 2026 · [Try Level-Up Lab →](https://levelup-lab.vercel.app)

**The problem.** My daughter's textbooks are not the problem. Nor are tutors or a lack of worksheets. The problem is the forty minutes after she says "I studied", which can mean anything from real work to staring at an open book. I wanted something that builds the *habit*: a plan, focused blocks, honest reflection, and spaced recall.

**The bet.** Don't compete with content. Be the coach and the game layer around the child's own books, and make the reward depend on evidence of thinking, not on time spent.

**The decisions.**
- *The gate.* A block only counts once the child writes five takeaways, each with a concrete anchor such as a name, a year, a "because" or a key term. Vague points get gentle coaching from the creature. No pasting.
- *Growth without punishment.* Missed days make the creature sleepy, but progress is never lost. Consistency is measured over a forgiving 5-of-7-day window.
- *Mistakes earn rewards.* Logging a slip earns play time, so kids learn which kind of error costs them most.
- *Kids tell their own story.* The daily report to the parent is shown to the child word for word before it's sent.
- *No AI, no ads, no tracking.* Admins see usage numbers only, and database rules keep families' notes private even from the team.

**What shipped.** An auto-spread study plan built from the school's own portion list, 25-minute focus blocks, the takeaway gate, a mistake log, spaced recall at 1, 3, 7 and 21 days, a creature that grows from egg to mythic across three worlds, an art studio, printable exam-style papers, and multi-child family accounts that sync and work offline. Every game number lives in one config file, ready to tune after the first trial week.

**Pull quote:** "The reward depends on evidence of thinking, not on time spent."

**What's next.** Trial-week tuning, then the locked rooms: music, chess and a runner game.

**[TODO: trial results or quotes? Screenshots: plan builder, the gate with coaching, creature stages.]**
