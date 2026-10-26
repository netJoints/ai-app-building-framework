# AI App Building Framework

A course for the team, including product managers. The app built with this framework is how the team learns.

1. **[AI 101](ai-101.html)** — the ideas, before anyone builds.
2. **[The tech stack](stack.html)** — the tools this teaching app is built with.
3. **[Research before you build](research.html)** — research before building the app for users. Pricing and viability are written. Steps 1, 2, and 3 of that chapter are next.

The course site is published at <https://netjoints.github.io/ai-app-building-framework/>.

## Chapter 1 · AI 101

The team needs a shared picture of how the field got here:

`rules → neural networks → Transformers → LLMs → GenAI / chat → RAG → agentic AI`

Keep one picture:

```text
LLM   = generates language
RAG   = supplies better context
Agent = uses the model in a tool-using loop
```

The full lesson is [ai-101.html](ai-101.html).

## Chapter 2 · The tech stack

One web app. Firebase Hosting serves it. Capacitor packages that same app for Android and iOS. Firebase Functions runs the backend, including model calls.

| Tool | Need | Role |
| --- | --- | --- |
| GitHub Actions and secrets | Code and automation | Build, test, and deploy. Credentials stay in GitHub Actions secrets, outside source code. |
| Firebase Hosting | Hosting | Serve the web app. |
| Firestore | Document data | Document database for document-shaped records. |
| Neon | Relational data | Postgres for structured, relational records. |
| Firebase Functions | Backend logic | Server-side logic. Model calls, Neon, and Stripe are reached from here. |
| Firebase Auth | Users | Sign-in, identity, and who may call the backend. |
| Stripe | Payments | Charges, subscriptions, and payment state. |
| Capacitor | Mobile | Package the same web app for Android and iOS. |

The full lesson is [stack.html](stack.html).

## Chapter 3 · Research before you build

Research before starting to build the app for users. Product managers and the rest of the team share this chapter.

1. Step 1 — next
2. Step 2 — next
3. Step 3 — next
4. **Pricing** — who pays, what they pay for, and what to learn before a price is chosen.
5. **Viability** — TAM, SAM, and SOM, then the break-even cost calculation.

| Term | Name | What it counts |
| --- | --- | --- |
| TAM | Total Addressable Market | Everyone who could buy this kind of product. |
| SAM | Serviceable Addressable Market | The part of the TAM that matches this product’s specific niche. |
| SOM | Serviceable Obtainable Market | The part of the SAM the team can realistically reach and win. |

Break-even uses one period, such as a month or the first year. Add the costs you pay anyway: hosting and related services, Claude Code, the domain and SMS verification, and marketing. Divide that total by the money kept from one paying customer, after costs that grow with that customer. Compare the result with the SOM for the same period.

The full lesson is [research.html](research.html).

## Selected sources for AI 101

- [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)
- [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)
- [Introducing ChatGPT](https://openai.com/index/chatgpt/)
