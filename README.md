# Micro Mirror Hackathon Snapshot

This repository preserves the released snapshot of `Micro Mirror` from the Shenzhen hackathon build on `March 14, 2026`.

## Snapshot Identity

- Snapshot date:
  - `March 14, 2026`
- Snapshot city:
  - `Shenzhen, China`
- Snapshot role:
  - hackathon release archive
  - deployed demo mirror
  - historical record of the original project version

## Team At The Time Of The Snapshot

The use case framing and the solution flow preserved in this snapshot were distilled collaboratively from the team's shared daily observations and discussion.
本快照中保留的使用场景定义与解决方案流程，是团队基于日常观察与讨论共同提炼出来的。

- [`Xena016`](https://github.com/Xena016) and [`Sheryl0907`](https://github.com/Sheryl0907) both came from bioinformatics backgrounds and contributed grounded architecture thinking about the practical feasibility of the medical testing approaches discussed in the concept.

- [`uplinkira`](https://github.com/uplinkira) contributed from an applied interaction design perspective, effectively acting as the user in the loop to test accessibility and commercial potential across the flow.

- For prototype implementation, `uplinkira` analyzed and applied the organizer-provided [`GOAT Network AgentKit`](https://github.com/GOATNetwork/agentkit) to produce the website landing page and payment interface prototype.

- `Xena016` and `Sheryl0907` produced the mobile-side prototype for the personal information input flow and the report output flow.

## Event Context

Public event page:
- `https://luma.com/bwro4uva`

Based on the public event page, the sprint was hosted by `Sophia Li`, `GOAT Network`, and `OpenBuild`, and the onsite build window ran from `14:30` to `17:30` on `March 14, 2026` in Shenzhen around a `GOAT`, `x402`, `ERC-8004`, and `OpenClaw` themed hackathon session.

## Competition Result

- `Micro Mirror Demo` received `General Track First Place`!

## What This Snapshot Preserves

- the original `Micro Mirror` product framing
- the hackathon-stage payment and agent demo
- the Shenzhen onsite build context
- the team composition and result record attached to that date

## Product Thesis At Snapshot Time

Micro Mirror was conceived as a preventive wellness prototype that turns a daily face photo into a longitudinal health direction signal, then connects that signal to an upgrade path that includes smart ring data, on-chain agent identity, and GOAT-based checkout.

The core ritual was:
- take one face photo per day
- keep the data on a timeline
- convert that timeline into a preventive health direction
- explain the result using both TCM-style framing and modern medical-style reporting

The upgrade path added smart ring signals such as:
- HRV
- resting heart rate
- sleep recovery

## What The Snapshot MVP Includes

- daily camera capture or image upload fallback
- local timeline of daily mirror records
- dual-reference report:
  - TCM-inspired interpretation
  - modern medical-style interpretation
- smart ring preorder flow
- GOAT Testnet3 payment flow with MetaMask
- `AgentKit Workflow Studio`
- `ERC-8004 Agent Identity Lab`
- gamified demo layer:
  - `Season`
  - `Rank`
  - `Quest XP`
  - `Quest Checkout Board`

## Repository Role

This repository should be read as:
- a deployed snapshot
- a hackathon archive
- a March 14, 2026 Shenzhen milestone record

## Local Run

```bash
cd micro-mirror-deploy
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
