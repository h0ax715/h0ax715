# Smart Contract Security Researcher

**Solana • EVM • Anchor • Solidity • Foundry**

I find protocol-level vulnerabilities through formal invariant verification — covering lending pools, AMMs, vaults, bridges, and oracle integrations. Active on Cantina, Immunefi, and Sherlock.

Recent: discovered and reported a valid vulnerability on Cantina (paid). Built a custom invariant-based fuzz harness (Python + Foundry) for automated detection of reentrancy, oracle manipulation, access control, and rounding error vulnerabilities.

---

### Selected Work

- **[findings](https://github.com/h0ax715/findings)** — Vulnerability writeups with reproducible Proof of Concept. Covers lending insolvency (Compound-style), oracle manipulation (TWAP), and permanent cache staleness. Each finding includes root cause analysis, attack flow, PoC, and mitigation.

- **[solana-invariants](https://github.com/h0ax715/solana-invariants)** — Formal specification of 50+ DeFi invariants across 9 protocol types (Compound lending, Aave V3 share-value, AMM constant-product, ERC-4626 vaults, liquidations, oracles, staking, StableSwap, precision/rounding). Used as a checklist during manual review and as specifications for automated verification.

---

### Platforms

- **Cantina** — Active researcher, valid finding submitted & paid
- **Immunefi** — Contest participant
- **Sherlock** — Contest participant

---

### Methodology

All findings are discovered through a combination of:

1. **Invariant specification** — formalizing the protocol's expected mathematical properties
2. **Automated fuzzing** — custom harness testing invariants against random state transitions
3. **Manual code review** — verifying invariant-sensitive paths
4. **Edge case testing** — first deposit, full withdrawal, maximum utilization, oracle boundary conditions
