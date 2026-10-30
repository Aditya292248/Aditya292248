# Aditya Bisht

Software engineer and student at Northeastern University. I build infrastructure for AI agents: how they pay for things, how they are authorized, how they drive a browser, how they understand code, and how a human can verify what they actually did.

Portfolio: [aditya292248.github.io](https://aditya292248.github.io/)

## Allowance

**[Allowance](https://useallowance.com)** - spending wallets for AI agents. Kotlin, TypeScript

I work across the Allowance product, with most of my work on the Android app, the agent wallet, and the MCP server agents use to make purchases.

- **Android app:** built the native Kotlin / Jetpack Compose client to parity with iOS. That covered allowances, approval flows that require device authentication, connected-agent onboarding, deep links, push notifications through Firebase Cloud Messaging, and chat with the conversation engine.
- **Agent Wallet:** one-time and scoped virtual cards for agent purchases, with readiness gates, a fail-closed Stripe Issuing webhook, and secure reveal links so card details never pass through the agent.
- **MCP and evals:** tools on the Allowance MCP server, an eval runner built on the Codex SDK, and an admin control page for running MCP evals.
- **Browser agents:** checkout workers built on Browser Use that complete shopping tasks while the user reviews and approves them.

## Projects

### [Stepglass](https://github.com/Aditya292248/stepGlass)
TypeScript, open source, Apache-2.0

A self-hosted tool that records what an AI agent did, verifies what actually changed in the systems it touched, and checks the result against policy. Most agent traces show what the agent said or what a tool returned. Stepglass records before-and-after evidence for each change, so a reviewer who doesn't read code can see what the agent tried to do, what changed, what went wrong, and which recorded step proves it. It is built in public, one reviewable PR at a time.

### [openBrowser](https://github.com/Aditya292248/openBrowser)
Rust

A CLI that drives a single persistent Chrome tab. Each command runs as a short-lived process. A local daemon keeps the browser session alive between commands until `close`, so agents and shell scripts can work with one real tab step by step. It gives structured JSON output, reports oversized snapshot responses clearly, and is tested end to end against a real Chrome session.

### Gatepoint
TypeScript, private

A trust gateway that sits between AI agents and the tools they call. Each agent gets an Ed25519 identity and a gateway-issued certificate and signs every request. The gateway checks each call against tenant policy before letting it through. With Ahaan Kallat, I built:

- tenant API key authentication, input validation, key revocation for compromised keys, and audit logging
- the policy engine, including a system policy layer for internal routes
- an LLM-powered policy generator, and a guardrail evaluation system with AI-generated test scenarios
- the web dashboard for agent management and intent history, and reference ecommerce and IT agents that run through the gateway

### [Neocortex](https://github.com/rusheelsharma/neocortex)
TypeScript

Turns a GitHub repository into a knowledge base you can query in natural language. It uses AST parsing, vector embeddings, and dependency-graph expansion to return only the code context an LLM needs. My contributions:

- vector embeddings and semantic search
- semantic compression through program slicing, to fit token budgets
- line, variable, and file extraction commands, with query-classifier support
- the presentation UI

## Open source contributions

- [open-instinct](https://github.com/mariagorskikh/open-instinct)

## Machine learning

- [ImageDoctor](https://github.com/Aditya292248/imageDoctor): full-reference image quality assessment with a fine-tuned ViT-Base on KADID-10k, using about 70% less GPU memory through selective freezing and gradient accumulation.
- [Loan Default Prediction](https://github.com/Aditya292248/loan-default-prediction): XGBoost at 0.72 AUC-ROC on 1.35M Lending Club loans, using only application-time features, with SHAP interpretability.
- [Marketing A/B Test Analysis](https://github.com/Aditya292248/marketing-ab-test-analysis): a 588K-user ad experiment showing a 43% conversion lift (p < 0.001), with dose-response analysis.

## Tools and languages

- **Languages:** TypeScript, Python, Kotlin, Rust, Java, SQL
- **Agents and AI:** MCP, Browser Use, Chrome DevTools Protocol, OpenAI and Codex SDKs, embeddings, PyTorch, XGBoost
- **Mobile and web:** Jetpack Compose, React, Node.js, Express
- **Infrastructure:** PostgreSQL, Prisma, Stripe Issuing, Firebase, Docker
