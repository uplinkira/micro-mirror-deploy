# Micro Mirror Deploy Mirror

This repository preserves the deployed release snapshot and the original hackathon release context for Micro Mirror.

The long-term product source of truth is:
- `https://github.com/uplinkira/micro-mirror.git`

## Hackathon Record Preserved Here

This deploy mirror intentionally keeps the Shenzhen sprint context attached to the original release.

Public event page:
- `https://luma.com/bwro4uva`

Based on the public event page, the sprint was hosted by `Sophia Li`, `GOAT Network`, and `OpenBuild`, and the onsite build window ran from `14:30` to `17:30` on `March 14, 2026` in Shenzhen around a `GOAT`, `x402`, `ERC-8004`, and `OpenClaw` themed hackathon session.

Micro Mirror was taken from zero to a working MVP during that Shenzhen build window with:
- `uplinkira`
- `2` collaborating bioinformatics graduate researchers from the Chinese Academy of Sciences

Award note:
- according to team records, this project received `General Track First Place`
- at the time of this update, the public event page confirms the sprint context, but no separate public award page was located, so this repository keeps the award wording explicitly as a team record rather than as an externally verified claim

## Product Thesis

Micro Mirror is a preventive wellness prototype that turns a daily face photo into a longitudinal health direction signal, then connects that signal to an upgrade path that includes smart ring data, on-chain agent identity, and GOAT-based checkout.

Most people do not need more one-off health anxiety. They need a lightweight way to notice recovery drift early, compare change over time, and decide what to adjust next.

The core ritual is:
- take one face photo per day
- keep the data on a timeline
- convert that timeline into a preventive health direction
- explain the result using both TCM-style framing and modern medical-style reporting

The upgrade path adds a smart ring so the product can combine visual signals with physiological signals such as:
- HRV
- resting heart rate
- sleep recovery

## What The MVP Includes

- daily camera capture or image upload fallback
- local timeline of daily mirror records
- dual-reference report:
  - TCM-inspired interpretation
  - modern medical-style interpretation
- smart ring preorder flow
- GOAT Testnet3 payment flow with MetaMask
- `AgentKit Workflow Studio`
  - maps local `agentkit/` modules to product workflows
  - highlights `x402`, `x402-merchant`, `ERC-8004`, and `wallet`
- `ERC-8004 Agent Identity Lab`
  - generates sample agent metadata
  - registers an agent from the browser
  - reads linked wallet, reputation summary, and client list
- gamified demo layer:
  - `Season`
  - `Rank`
  - `Quest XP`
  - `Quest Checkout Board`

## Why The Agent Matters

In Micro Mirror, the agent is not just a chatbot wrapper. It has a concrete job across three layers:

1. Observe
- read the image timeline
- combine sleep, stress, hydration, and optional ring signals

2. Decide
- generate an actionable preventive direction
- present the result in dual framing so the user can understand both intuition and structure

3. Act
- move the user into subscription or hardware checkout
- later accumulate trust and identity using `ERC-8004`

## Why GOAT / AgentKit Is Central

This deploy mirror preserves the release story around the infrastructure the MVP was built to showcase:

- `x402`
  - payment intent and settlement framing for the smart ring preorder path
- `x402-merchant`
  - merchant-side order and subscription operations
- `ERC-8004`
  - future-facing on-chain agent identity and trust layer
- `wallet`
  - browser wallet connectivity for the live demo

Generated assets that make the integration visible:
- `generated/agentkit-catalog.json`
- `generated/agentkit-demo.json`

## Repository Role

- Main product repository:
  - `https://github.com/uplinkira/micro-mirror.git`
- This repository:
  - `https://github.com/uplinkira/micro-mirror-deploy.git`

This repository should be read as:
- a deployment mirror
- a hackathon release archive
- a historical snapshot of the Shenzhen demo milestone

Long-term development should continue in:
- `micro-mirror`

The migration and Vercel strategy are documented in:
- `docs/repo_deploy_workflow_2026.md`

## Local Run

```bash
cd D+20260314+goat/micro-mirror-deploy
python3 -m http.server 8000
```

Open:
- `http://127.0.0.1:8000`

## Medical Scope

Micro Mirror is a product prototype and should not be treated as a diagnostic system, a regulated medical device, or a substitute for professional medical advice.

## License

This repository is released under the `Apache-2.0` license.

Important note:
- the `Micro Mirror` product name, branding, pitch framing, and other unlicensed trademarks remain reserved to their respective owners under the terms of `Apache-2.0`
