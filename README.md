# AI App Building Framework

A two-step course for the team. The app built with this framework is how the team learns.

1. **[AI 101](ai-101.html)** — the ideas, before anyone builds.
2. **[The tech stack](stack.html)** — the tools this teaching app is built with.

The course site is published at <https://netjoints.github.io/ai-app-building-framework/>.

## Step 1 · AI 101

The team needs a shared picture of how the field got here:

`rules → neural networks → Transformers → LLMs → GenAI / chat → RAG → agentic AI`

Keep one picture:

```text
LLM   = generates language
RAG   = supplies better context
Agent = uses the model in a tool-using loop
```

The full lesson is [ai-101.html](ai-101.html).

## Step 2 · The tech stack

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

## Selected sources for AI 101

- [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401)
- [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165)
- [Introducing ChatGPT](https://openai.com/index/chatgpt/)
