# Kali Kannada — source notes and draft article

Sources: `kali-kannada-deck.pdf` / `.pptx` (HelloPM Buildathon deck, 10 slides; same content in both).
Live: https://kali-kannada.vercel.app (live beta, no sign-up)
Code: https://github.com/hemz29/StudyBuddy

## Key facts to use
- **What it is:** an exam-preparation companion for Grade 6 students taking Kannada as a third language. Students read school chapters, practise in the exam format, and get handwritten work checked. Tagline: "Kannada, with confidence".
- **Role:** product leader, parent, and sole founder-builder. Built for the HelloPM Buildathon.
- **Stack:** Claude Code, ChatGPT, Supabase, Vercel, GitHub, Microsoft Copilot (imagery).
- **Research:** 17 parents surveyed (13 Grade 6, 11 ICSE, all third-language). All had prepared for a test in the past month, 6 in the past week.
  - 14/17 can't reliably explain or check their child's work. 9/17 are unable to check answers or often unsure. 8/17 struggle to get their child studying independently (the top difficulty). 6/17 have trouble understanding lessons.
  - Current tools: 9 use tutors, 8 textbooks or notes, 6 already use ChatGPT or Gemini, 5 a translator. These tools are fragmented across explanation, practice and checking.
  - 6/17 spend ₹1,500–₹3,000+ on extra Kannada help.
  - What parents want: independent practice (12), explanations in a language they understand (9), a syllabus match (7), written-answer support (5), checks against school expectations (5).
- **Core insight:** "The strongest pain is confidence, not content discovery." The problem isn't access to content. It's understanding, matching the school syllabus, written practice, and knowing whether answers are right.
- **Journey:** choose a lesson → read the chapter (word-level sound and meaning) → practise grammar → download a school-format worksheet → write by hand and upload a phone photo (via QR) → confirm the recognised text → see marks and progress.
- **Signature decision:** the student confirms the OCR reading of their handwriting *before* marking. No competitor does this.
- **Feedback that changed the product:**
  - "I don't want to give my Google login" → built guest access with no sign-up.
  - "The page should have something to help me trust this" → added a founder story and trust signals.
  - "Show what else the product will give" → added a Future Plans page.
  - "Can I upload my own content?" → added to the roadmap as a repeat-use need.
- **Available now:** 3 chapters, grammar cards, worksheets and 1-hour timed tests, print or answer online, handwriting OCR with confirmation, automated marking and feedback, hints with controlled marks treatment, a parent view showing progress by skill, child nicknames, a pilot analytics dashboard, and content reviewed by a practising Kannada educator.
- **Next:** speaking practice, uploads of parent-provided content, more chapters, grades, boards and languages, personalised recommendations, and a teacher view. Licensing is required before wider launch.
- **Competitors:** DoerDo, Veda AI, PadhoAI, tutors, ChatGPT. "Narrower than generic AI, more complete for this job." Why not just ChatGPT? Kali packages prompting, syllabus context, exam format, handwriting confirmation, marking and parent progress into one repeatable workflow.
- **Pilot (invite-only, one Bengaluru ICSE school, no partnership claimed):** 6 parent accounts, 7 children, 24 visits, 12-minute average visit, 11 worksheets printed, 8 started, 3 completed, 2 parents returned on another day. Feedback: 2 of 3 would use it for the next test, 1 probably would. Recommendation scores of 10, 8 and 5 (average 7.7/10).
- **Honest limits:** not yet proven are weekly retention, better exam outcomes, and willingness to pay.
- **GTM:** acquisition through invite-only parent WhatsApp groups. Activation means completing one full marked test. Retention comes from upcoming unit tests. Referral from parent to parent. Revenue starts with a school partnership, then subscriptions. Pricing hypothesis: under ₹500/month, against the ₹1,500–₹3,000+ some parents already spend.

## Draft feature article

**Kicker:** Learning · EdTech
**Headline:** When the homework is in a language the parents can't read
**Standfirst:** Thousands of Bengaluru children study Kannada as a third language, and most of their parents can't check a single answer. Kali Kannada takes a child from the school chapter to a marked, handwritten exam paper, with no tutor and no sign-up.
**Meta:** Personal project · Sole founder-builder: research, product, design and build · HelloPM Buildathon 2026 · [Try Kali Kannada →](https://kali-kannada.vercel.app)

**The problem.** I'm one of these parents myself. When my child sits down to revise for a Kannada test, I can't tell whether an answer is right. I surveyed 17 parents in the same position, and 14 said the same thing. They didn't lack content. They had textbooks, tutors, translators and ChatGPT. What they lacked was *confidence*: help understanding the chapter, practice in the format the school actually tests, and an honest check of their child's written answers.

**The insight.** Generic AI can explain a word. It can't tell you whether your child's handwritten answer would score marks on a school paper. So I built around that workflow instead of around chat.

**The decisions.**
- *Built for paper, not screens.* School exams are handwritten, so Kali produces printable school-format worksheets with a 1-hour timer, and students upload a phone photo of their answers.
- *The child confirms what the machine read.* Before anything is marked, the student checks the OCR reading of their handwriting. If the system misreads an answer, the child doesn't lose marks for it. None of the competitors I looked at do this.
- *Let parents' doubts shape the product.* "I don't want to give my Google login" led to guest access. "Something to help me trust this" led to a founder story and an educator content review.
- *Say what isn't proven.* The roadmap is kept separate from what's live, and licensing comes before any wider launch.

**What shipped.** Three full chapters with word-level audio and meanings, grammar drills, timed worksheets, handwriting recognition with confirmation, automated marks and feedback, and a parent view of progress by skill. It's all live and free to try without an account.

**Early signals.** In an invite-only pilot with families from one school, 7 children made 24 visits averaging 12 minutes, and parents printed 11 worksheets. Two of the three parents who left feedback said they'd use it for the next test, and the average recommendation score was 7.7/10. What it doesn't prove yet: retention, better results, and willingness to pay. That's the next milestone.

**Pull quote:** "The strongest pain was confidence, not content."

**What's next.** Speaking practice, parent-uploaded content, more chapters and grades, then a school partnership before any subscription.

**Built with:** Claude Code · Supabase · Vercel · ChatGPT

**[TODO: confirm "Thousands of Bengaluru children" or soften. Screenshots needed: chapter reader, worksheet, OCR confirmation screen.]**
