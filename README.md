### Rahshaun Chambers

I check Solidity contracts for the rules they must never break, using Foundry fuzzing run against the
real contracts and Halmos symbolic checks, and I show my work so you can rerun it.

**Start here:** [contract-invariant-samples](https://github.com/rahshaun44-byte/contract-invariant-samples).
Checks on EigenLayer, Uniswap v4, Sky (MakerDAO), Morpho Blue and Base's Nitro validator at pinned
commits, all rerunnable with one command. Three reports carry their own corrections, where my review
found a check that didn't reach the contract.

**Fixed-scope invariant verification:**

| | Scope | Price |
|---|---|---|
| Starter | one small contract or hook | $250 |
| Standard | 1–3 contracts, up to ~800 lines, or one upgrade diff | $500 |
| Larger | multi-contract systems | quoted, from $1,500 |

Every engagement:

- we agree the list of invariants before I start
- Foundry suite against your real contracts, 10,000 runs per invariant
- Halmos checks where they fit, with their bounds stated
- a short report, with a runnable test for anything that breaks, and remediation advice
- one retest of your fixes
- the tests are yours to keep in CI
- 5–7 days; everything runs locally, nothing touches a live network

Not a full audit, and a clean result is not a promise of no bugs. It tells you exactly which rules held,
under which checks.

**Also building:** [untether](https://github.com/rahshaun44-byte/untether), which runs coding agents from
Telegram.

**Contact:** quantumhat232@gmail.com
