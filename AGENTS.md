I can't attach downloadable files in this chat, so here are both files complete and copy-pasteable. Create them in your **repo root** (the same folder as the `Makefile`), each with the exact filename shown.

---

### 📄 File 1: `AGENTS.md`

```markdown
# AGENTS.md — Operating rules for any AI working in this repo

You assist a solo developer in QDay Aevum Builder Challenge #1 (deadline 11 Dec 2026, 16:00 HKT).
The developer is newer to Web3: explain clearly, never lower the engineering bar.

## Read order (every session)
1. PROJECT_STATE.md — phase, decisions, next steps
2. docs/workflow/*.md — standards in force
3. docs/decisions/ — ADRs for anything you're about to touch

## Hard rules
- Shanghai EVM only. No MCOPY/TSTORE/blob opcodes. evm_version = "shanghai".
  Never suggest OpenZeppelin *Transient contracts.
- Aevum quirks: legacy transactions (--legacy), eth_getLogs ≤1000 blocks, no WebSocket,
  no explorer verification. Details in PROJECT_STATE.md.
- Test-first: no logic or contract code without a failing test first (red → green → commit).
- No secrets in the repo — no keys, no .env, no API keys. Keys live in the Foundry keystore.
- License hygiene: repo is MIT, credit "Based on Aevum Starter Kit (MIT, PQA Labs)".
  Never copy AGPL content (e.g. OpenZeppelin skills) into this repo.
- Conventional commits: feat:/fix:/test:/docs:/chore: — small and atomic.
- Verify before claiming done: show evidence (command output, tx hash). "Seems right" is never sufficient.
- Update PROJECT_STATE.md at the end of every session.

## Optimize for the judging rubric
Innovation · Technical quality · Real-world utility · UX · Demo · Documentation · Safety & controls
```

---
