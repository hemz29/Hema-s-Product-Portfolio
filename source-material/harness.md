# Harness — source notes and draft article

Source: repo https://github.com/hemz29/Harness-chatbot (code only, no README; read 13 Nov 2026).
Live link: **[TODO: is it deployed anywhere? Built in Google AI Studio.]**

## What the code shows
- **"Harness: grounded multi-model intelligence workspace with Claude and Gemini."** A React 19 + Vite + Tailwind app, scaffolded in Google AI Studio.
- **Multiple models in one thread:** adapters for Claude (Anthropic API) and Gemini, with model names configurable per provider. API key slots also exist for OpenAI and Grok (not yet wired). The prompt box placeholder reads: "Ask anything, run a multi-model comparative query…"
- **Grounding sources:** (1) attached documents injected as delimited context, (2) Tavily web search snippets, (3) a pasted email thread for drafting replies (`draftEmailWithModel`).
- **Context Inspector:** shows what's attached (document name, character count, estimated tokens, truncation), so the user can see exactly what the model sees.
- **Per-message telemetry:** model used, latency, estimated tokens, and grounding metadata (document, search count, email).
- **Conversation trimming:** keeps the most recent 20 messages and tells the user when trimming happens.
- **Bring your own keys,** stored only in the browser's local storage. Sessions are saved locally too.
- **Roadmap hints in the UI:** voice input ("coming soon").

**Gap vs Hema's description** ("linked to all of my apps and web search"): today it covers documents, email (by paste) and web search. Connecting live to her apps is the vision, not yet built. The article should say that honestly.

## Draft feature article (short format)

**Kicker:** AI · Personal tooling
**Headline:** I built my own AI workbench to see what the models see
**Standfirst:** Harness puts Claude and Gemini side by side, grounds them in my documents, emails and live web search, and shows exactly what context each answer was built from.
**Meta:** Personal build · 2026 · [View the code →](https://github.com/hemz29/Harness-chatbot)

**Why build one.** As a product person working on RAG systems, I wanted to *feel* the trade-offs, not just read about them. What happens to an answer when a document gets truncated? When search is on or off? When the same question goes to two different models?

**What it does.**
- *Two models, one thread.* Ask Claude or Gemini, or compare their answers to the same prompt.
- *Grounded on demand.* Attach a document, paste an email thread to draft a reply, or switch on live web search (Tavily).
- *Nothing hidden.* A context inspector shows every piece of attached context, its size in tokens and whether it was truncated. Each reply shows the model, latency and estimated tokens.
- *My keys, my machine.* API keys and chat history stay in the browser.

**What I learned.** [TODO: Hema, one or two real observations, e.g. where the models differed, or how much truncation changed answers.]

**What's next.** Connecting it to the apps I use every day (calendar, mail, notes) so it becomes a true personal assistant, plus OpenAI/Grok adapters and voice input.
