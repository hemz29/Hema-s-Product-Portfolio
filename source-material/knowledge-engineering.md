# Knowledge Engineering — source notes and draft article

Source: an internal slide Hema shared on 13 Nov 2026 ("Knowledge Platform capability flow", marked current focus). The slide itself is **not** stored in this repo.
**Disclosure rule:** generic names only. Say "a large UK telco", never the company. Call the context layer "a shared context broker" and the design capability "a design assistant". No pilot team names.

## Key facts to use
- **Hema's role:** product lead, started in Nov 2026.
- **Thesis:** scattered engineering knowledge is progressively distilled into reusable context, then into applied capabilities, then into measurable outcomes.
- **Layer 1, knowledge sources.** Context stays in the systems where teams already work: wiki pages (architecture, product, process), the work tracker (epics, features, stories, acceptance criteria), document libraries (policies, standards), email (decisions, approvals), meeting transcripts and recordings, workshop boards (discovery thinking), published engineering docs, and people's tacit knowledge. More sources are added over time. **Two are connected today: the wiki and the work tracker.**
- **Layer 2, shared context.** A knowledge broker retrieves the most relevant engineering context for a question and makes it reusable downstream. It is context-agnostic, reusable and shared.
- **Layer 3, SDLC capabilities.** In scope now are **Plan** (requirements discovery) and **Design** (a design assistant). Build, Test, Deploy and Operate are intended future extensions, not yet applied.
- **Layer 4, outcome.** Faster, more consistent feature delivery across the product lifecycle, so customers get new capabilities sooner.
  - Leading indicators:
    - **Faster:** requirements gathered, defined and validated sooner, with fewer discovery hand-offs.
    - **Better:** higher-quality, traceable inputs, fewer clarification loops and less rework.
    - **Reusable:** each feature builds on shared product context, so future delivery is aware of what came before.
- **Route to scale:** (1) prove value with pilot teams, (2) productise by moving from sandbox to production, (3) scale with more sources, use cases and integrations.

## Draft feature article

**Kicker:** AI · Enterprise knowledge · Now
**Headline:** An engineering organisation's memory is everywhere except where you need it
**Standfirst:** I've just taken product lead on a knowledge platform at a large UK telco. It turns scattered engineering context (wiki pages, work-tracker stories, meeting transcripts, the things people only say out loud) into one reusable layer that AI capabilities can build on.
**Meta:** Work · Product lead · Started Nov 2026 · Developing story

**The problem.** Ask why a feature was built a certain way and the answer is in six places: a wiki page, a Jira-style epic, an email approval, a recorded call, a workshop board, and someone's head. Every new piece of work starts with a hunt through all of them. That hunt is where discovery hand-offs multiply and rework begins.

**The architecture.** Four layers, each narrower and more useful than the last:
1. **Sources:** leave knowledge where teams already work, and don't ask anyone to migrate.
2. **A shared context broker:** retrieves the most relevant context for a question and makes it reusable by any downstream tool.
3. **Capabilities across the lifecycle:** starting with requirements discovery and design assistance.
4. **Outcomes:** faster, more consistent delivery.

**The deliberate scope.** Two sources connected and two lifecycle stages live. Everything else on the roadmap is greyed out on purpose. Breadth is earned after the first pilots prove value.

**How we'll know it's working.** Faster: requirements validated sooner, with fewer hand-offs. Better: traceable inputs and fewer clarification loops. Reusable: every feature leaves context behind for the next one.

**The route to scale.** Prove value with pilot teams, move from sandbox to production, then add sources, use cases and integrations.

**Pull quote:** "The grey boxes are a promise, not a claim."

**Key priorities.**
- **Prove value in the pilot.** Get the shared context broker to return trusted, cited context from the first two sources into requirements discovery and design, and show a measurable drop in discovery hand-offs and clarification loops.
- **Build for scale from day one.** Retrieval-quality evals, permission-aware access and a repeatable pattern for onboarding new sources. That way the move from sandbox to production, and from two lifecycle stages to six, adds use cases without rework.

**My role as product lead.**
- **Own the vision, roadmap and sequencing.** Decide which sources and lifecycle stages come next based on pilot evidence, and keep the roadmap honest about what is live and what is still intended.
- **Define what "working" means.** Turn the faster/better/reusable indicators into concrete metrics and retrieval-quality evals, and set the pilot success criteria that gate productisation.
- **Connect the people around it.** Run discovery with pilot engineering teams, align architects and stakeholders on the platform model, and turn feedback into a prioritised backlog that drives adoption.

[Drafted by Claude from the slide. Hema to edit.]

**Visual:** redraw the four layers as a simple editorial diagram in the site's own style. Never reuse the internal slide.
