### Rahshaun Chambers · QuantumFlex

**Independent smart contract invariant verification. Don't take my word for it: rerun the evidence yourself.**

I check whether Solidity contracts keep their critical properties (balances that always add up, funds that
can always leave, roles that can't be bypassed) under adversarial and unexpected inputs, using Foundry
fuzzing against the real contracts and Halmos symbolic checks. Every result ships with the tests that
produced it.

**Start here:** [contract-invariant-samples](https://github.com/rahshaun44-byte/contract-invariant-samples).
Checks on EigenLayer, Uniswap v4, Sky (MakerDAO), Morpho Blue and Base's Nitro validator at pinned commits,
all rerunnable with one command. Three reports carry their own corrections, where my review found a check
that didn't reach the contract.

| Package | Scope | Price |
|---|---|---|
| Starter | One small contract or hook | $250 |
| Standard | 1–3 contracts (~800 lines) or one upgrade diff | $500 |
| Extended | Larger multi-contract systems | from $1,500 |

Each includes an agreed invariant list, 10,000 fuzz runs per invariant, Halmos where it fits (bounds
stated), a report with remediation advice, one retest, and the tests to keep in CI. 5–7 days, all local,
nothing touches a live network. Details and limits: [OFFER.md](https://github.com/rahshaun44-byte/contract-invariant-samples/blob/main/OFFER.md).

Not a full audit. A clean result tells you exactly which properties held under which checks, and no more.

**Contact:** quantumhat232@gmail.com
