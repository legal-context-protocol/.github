# Legal Context Protocol (LCP)

**The missing legal layer for AI-agent commerce.**

An open standard for publishing and cryptographically proving the **legal terms** behind a transaction — across every major agent-payment protocol (x402, MPP, AP2, ACK) and settlement rail (EVM, Stellar, Hedera, Solana, and more).

🌐 [legalcontextprotocol.org](https://legalcontextprotocol.org) · 📄 [White paper](https://www.legalcontextprotocol.org/white-paper.pdf) · 📐 [Specification](https://github.com/legal-context-protocol/legal-context-protocol)

---

## Why LCP

AI agents can now buy and sell on their own. The **payment** layer is solved — there are billions of dollars of rails. But the **agreement** layer is missing: when an agent transacts and something goes wrong, there's no standard way to know *what the terms were, whether both sides agreed, which law governs, or how to dispute it.*

LCP fills that gap with one idea, layered in increasing strength:

1. **Publish** your terms at one standard URL — `/.well-known/legal-context.json` (no blockchain required).
2. **Prove** they can't be quietly changed — a SHA-256 hash of the terms.
3. **Sign** — the buyer cryptographically signs that hash: non-repudiable proof of *who* agreed to *what*, *when*.
4. **Integrate** — connect to real institutional recourse: dispute resolution, jurisdiction, remedies.

One required field; everything else is opt-in.

---

## Stewardship

The Legal Context Protocol is **co-stewarded by [Integra Ledger](https://integraledger.com) and the [American Arbitration Association (AAA)](https://www.adr.org)** — pairing commerce-infrastructure engineering with the world's leading dispute-resolution institution.

- **David Fisher** — CEO, Integra Ledger — lead author and driving force behind LCP.
- **Bridget McCormack** — CEO, American Arbitration Association — co-led the initiative with David Fisher: co-author of the white paper *"Identity, Trust, and the Legal Foundations of Agentic Commerce"* and a driving force behind the overall plan.

The **LCP technical specification** is co-authored by **David Fisher** and **David Berger** (Chief Science Officer, Integra Ledger).

---

## Projects

- **[legal-context-protocol](https://github.com/legal-context-protocol/legal-context-protocol)** — the specification, JSON Schema, examples, and governance.
- **`@legalcontext/*`** — the open-source (Apache-2.0) reference implementation: 48 packages covering the protocol and rail adapters, the buyer gate, and conformance tooling. *(Publishing to npm.)*

---

## First release — an open invitation

This is the **first public introduction** of the Legal Context Protocol. We are releasing it openly and **actively inviting contributors**.

LCP is built to be **co-stewarded**. We expect — and warmly invite — **companies and foundations to take ownership of specific implementations and adapters.** A protocol steward such as the **x402 Foundation**, for example, is a natural long-term owner of the x402 adapter; rail and protocol partners (payment networks, blockchains, standards bodies) are likewise invited to own and maintain their corresponding packages. Per-package ownership is wired through the implementation repo's `CODEOWNERS`.

**Get involved:**
- Read the [specification](https://github.com/legal-context-protocol/legal-context-protocol) and the [white paper](https://www.legalcontextprotocol.org/white-paper.pdf).
- Propose changes via the SEP process (see the spec repo's `GOVERNANCE.md`).
- Build — or take ownership of — an adapter or implementation.

**Contact:** **David Fisher**, CEO, Integra Ledger — [@dafisher2000](https://github.com/dafisher2000) · via [legalcontextprotocol.org](https://legalcontextprotocol.org).

Licensed under **Apache-2.0**.
