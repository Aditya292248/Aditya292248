# Aditya Bisht

Student at Northeastern University. I build tools for AI agents: browsers they can drive, recorders that show what they actually changed, and the infrastructure underneath. I also work on applied machine learning and data analysis.

Portfolio: [aditya292248.github.io](https://aditya292248.github.io/)

## What I am working on

**[Stepglass](https://github.com/Aditya292248/stepGlass)** - TypeScript
An open-source, self-hosted tool that records what an AI agent did, verifies what actually changed in the systems it touched, and checks the result against policy. Built in public, one reviewable PR at a time.

**[openBrowser](https://github.com/Aditya292248/openBrowser)** - Rust
A CLI for driving one persistent Chrome tab. Each command is a short-lived process; a local daemon keeps the browser session alive. Structured JSON output for use by agents and scripts.

**[codingAgent](https://github.com/Aditya292248/codingAgent)** - TypeScript
A VS Code coding assistant backed by a local repository graph. Currently at the foundation stage: package boundaries, shared contracts and build tooling.

## Open source contributions

- [open-instinct](https://github.com/mariagorskikh/open-instinct): honor `Retry-After` for webhook forwarding in the gateway; fix cron name validation in the CLI.

## Machine learning and data projects

| Project | Summary |
| --- | --- |
| [ImageDoctor](https://github.com/Aditya292248/imageDoctor) | Full-reference image quality assessment with a fine-tuned ViT-Base on KADID-10k; about 70% lower GPU memory through selective freezing and gradient accumulation. |
| [Loan Default Prediction](https://github.com/Aditya292248/loan-default-prediction) | Default risk on 1.35M Lending Club loans using only application-time features. XGBoost at 0.72 AUC-ROC with SHAP interpretability. |
| [Marketing A/B Test Analysis](https://github.com/Aditya292248/marketing-ab-test-analysis) | 588K-user ad experiment: 43% conversion lift (p < 0.001), dose-response analysis, and a Simpson's paradox check. |
| [Nifty 50 Investment Dashboard](https://github.com/Aditya292248/Nifty-50-Investment-Dashboard) | Streamlit app for analyzing Nifty 50 stocks and building equal-weight portfolios. |
| [Brain Tumor Image Segmentation](https://github.com/Aditya292248/Brain-Tumor-Image-Segmentation) | Medical image segmentation of brain tumors. |

## Other projects

- [Agent Ledger](https://github.com/Aditya292248/agentLedger) - payment engine with approval workflows and n8n integration (TypeScript, PostgreSQL).
- [finreview](https://github.com/Aditya292248/finreview) - financial inclusion platform (React, Express, TypeScript).

## Tools and languages

- **Languages:** Python, TypeScript, Rust, Java, Racket, SQL
- **AI and data:** PyTorch, Vision Transformers, XGBoost, scikit-learn, SHAP, pandas, Streamlit
- **Systems and web:** Chrome DevTools Protocol, Node.js, React, Vite, Express, PostgreSQL, Docker
