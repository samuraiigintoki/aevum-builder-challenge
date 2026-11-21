
### 📄 File 2: `PROJECT_STATE.md`

```markdown
# PROJECT_STATE — Aevum Builder Challenge #1

> Single source of truth. Any new session: read this first, then docs/workflow/.
> Update at the end of every working session. A session that doesn't update it isn't finished.

## Mission
Build a tUSD8 payment app for QDay Aevum Builder Challenge #1 (DoraHacks).
Solo developer + AI agents. Beginner-friendly pace, senior-quality output.

## Key dates
- **Submission deadline: 11 Dec 2026, 16:00 HKT (08:00 UTC)** — late = rejected
- Judging 12–14 Dec · Winners 15 Dec · Prizes $800/$500/$200 USDT

## Current phase
SETUP COMPLETE → next: PROJECT SELECTION (not yet finalized — do not build until spec is approved)

## Environment facts (verified)
| Item | Value |
|---|---|
| Chain | QDay Aevum Testnet, ID 44005 |
| RPC | https://rpc-test.qday.info (HTTPS only, no WebSocket) |
| Explorer | https://explorer-test.qday.info (verification broken — prove via commit hash + tx evidence) |
| Tokens | tQDAY gas (18 dec) · tUSD8 0x456569838f1d43009A91ebA4263147Afd7233483 (6 dec, EIP-2612 permit + EIP-3009) |
| EVM | **Shanghai only** — no MCOPY/TSTORE; evm_version = "shanghai" mandatory |
| Gotchas | legacy txs (--legacy), eth_getLogs ≤1000 blocks (getLogsChunked), no official ERC-4337, ERC-8004 closed for challenge |
| Local fork | chain 440050, http://127.0.0.1:8555 · Checkout 0x7A4573aC2b17f5F3622ddfabC437c5DE2d3D87Df |
| Dev wallet | 0xFAFef0e2Aa48c5C57161974148c118f414E2973A — 1 tQDAY + 5 tUSD8 (test-only, keystore `aevum-deployer`) |

## Setup status
- [x] Node v24.21.0, Foundry, pnpm · make check green (14 tests, Shanghai-safe, fork tests vs real tUSD8)
- [x] Fork deploy + web payment flow verified · faucet claimed & verified · keystore imported
- [x] Repo: https://github.com/samuraiigintoki/aevum-builder-challenge (based on Aevum Starter Kit, MIT, PQA Labs)

## Adopted standards
- Engineering: addyosmani/agent-skills (MIT) — TDD, review gates, security, ADRs
- Contracts: OpenZeppelin skills (AGPL — guidance only, never copy files into this repo)
- UI: ui-ux-pro-max (MIT) — design system generation when we build the web app
- Borrowed: mattpocock/skills — grilling + handoff patterns

## Decision log
| Date | Decision | Why |
|---|---|---|
| 2026-11-21 | Base repo on Aevum Starter Kit | MIT, official, relayer + fork tooling included |
| 2026-11-21 | addyosmani as engineering standard | Rubric-aligned, security+docs coverage, portable |
| 2026-11-21 | OZ skills = guidance only | AGPL incompatible with vendoring into MIT repo |

## Next steps
1. Finalize project choice (grilling session) → write docs/SPEC.md
2. Scaffold docs/workflow/ from adopted skills
3. Register on DoraHacks once project is named

## Open questions
- Project not finalized (user decision pending)
- Confirm python3 available (needed for ui-ux-pro-max scripts)
```

---
