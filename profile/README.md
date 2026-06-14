<div align="center">

# Qietr

### Private payments for the agentic web.

Pay for APIs, content, and metered services in USDC &mdash;<br />
without revealing your identity, history, or balance.

[![Website](https://img.shields.io/badge/Website-qietr.com-111111?style=for-the-badge&labelColor=111111)](https://qietr.com)
[![X](https://img.shields.io/badge/Follow-%40QietrCom-111111?style=for-the-badge&logo=x&logoColor=white&labelColor=111111)](https://x.com/QietrCom)
[![Docs](https://img.shields.io/badge/Read_the-Docs-111111?style=for-the-badge&labelColor=111111)](https://github.com/QietrProtocol/qietr/tree/main/docs)
[![License](https://img.shields.io/badge/License-MIT-111111?style=for-the-badge&labelColor=111111)](https://github.com/QietrProtocol/qietr/blob/main/LICENSE)

</div>

```
You should be able to pay without being watched.
```

---

## About Us

Our mission is simple: **make payments private by default.**

The web is gaining a native payment rail &mdash; **HTTP 402 (x402)** &mdash; that lets a
server demand a stablecoin payment before it responds. It is ideal for AI agents
paying for APIs, tools, and data on the fly. But a plain x402 payment is fully
public: anyone watching the chain sees exactly who paid whom, when, and how much.

Qietr fixes that. We wrap x402 micropayments in a **zero-knowledge shielded pool**,
so a merchant gets paid and can verify the payment while learning *nothing* about
the payer. Privacy, self-custody, and honest disclosure are baked into the core.
We're building the quiet layer the payment web forgot &mdash; and we're building it
in the open.

## Flagship

<div align="center">

### Qietr Protocol

**A zero-knowledge privacy layer for x402 stablecoin micropayments on Solana.**

![Solana Devnet](https://img.shields.io/badge/Solana-Devnet_Live-111111?style=for-the-badge&logo=solana&logoColor=white&labelColor=111111)
![Groth16](https://img.shields.io/badge/ZK-Groth16_/_BN254-111111?style=for-the-badge&labelColor=111111)
![USDC](https://img.shields.io/badge/Settles_in-USDC-111111?style=for-the-badge&labelColor=111111)

&mdash; BUILT ON &mdash;

<table>
<tr>
<td align="center" width="200">
<strong>Circom</strong><br /><br />
ZK circuits &mdash; Poseidon<br />hashing + Groth16
<br /><br />
<img src="https://img.shields.io/badge/Circom-2B2B2B?style=flat-square" alt="Circom" />
</td>
<td align="center" width="200">
<strong>Anchor</strong><br /><br />
On-chain programs &mdash;<br />Merkle tree + verifier
<br /><br />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</td>
<td align="center" width="200">
<strong>Groth16</strong><br /><br />
zk-SNARK proofs<br />over BN254
<br /><br />
<img src="https://img.shields.io/badge/BN254-2B2B2B?style=flat-square" alt="BN254" />
</td>
</tr>
</table>

</div>

## Ecosystem

<table>
<tr>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-circuits">qietr-circuits</a></h3>
ZK circuits &mdash; Poseidon hashing and Groth16 proofs over BN254.
<br /><br />
<img src="https://img.shields.io/badge/Circom-2B2B2B?style=flat-square" alt="Circom" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-pool">qietr-pool</a></h3>
Anchor program &mdash; Merkle tree, deposit, withdraw, Groth16 verifier.
<br /><br />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-sdk">qietr-sdk</a></h3>
TypeScript SDK &mdash; notes, proofs, relayer client, x402 helper.
<br /><br />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
</td>
</tr>
<tr>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-relayer">qietr-relayer</a></h3>
Fastify service &mdash; gasless deposits, fee logic, rate-limit, sanctions.
<br /><br />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-indexer">qietr-indexer</a></h3>
Geyser plugin + API &mdash; indexes pool state into Postgres.
<br /><br />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-web">qietr-web</a></h3>
Next.js app &mdash; wallet adapter, deposit/pay UI, note manager.
<br /><br />
<img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js" />
</td>
</tr>
<tr>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-msg">qietr-msg</a></h3>
Anchor program &mdash; encrypted off-chain messaging for agents.
<br /><br />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/qietr-escrow">qietr-escrow</a></h3>
Anchor program &mdash; agent job escrow with CPI token transfers.
<br /><br />
<img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
</td>
<td valign="top" width="333">
<h3><a href="https://github.com/QietrProtocol/qietr/tree/main/docs/dev/06-tokenomics.md">$QIET</a></h3>
Protocol token &mdash; revenue share, governance, fee discounts. <em>Not minted yet.</em>
<br /><br />
<img src="https://img.shields.io/badge/Design-2B2B2B?style=flat-square" alt="Design" />
</td>
</tr>
</table>

---

<div align="center">

<sub>Live on Solana devnet &middot; not yet audited &middot; not on mainnet &mdash; <a href="https://github.com/QietrProtocol/qietr#deployment-status">honest status</a></sub>

<br /><br />

**Built quiet. Built in the open.**

<sub>&copy; 2026 Qietr Protocol &middot; MIT licensed</sub>

</div>
