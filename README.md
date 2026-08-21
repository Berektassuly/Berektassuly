# Mukhammedali Berektassuly

Software Engineer at [airi.chat](https://airi.chat), building GenAI and backend systems in **Rust**, **TypeScript**, and **Solana**.  
Open-source contributor to **Rust**, **Tokio**, **Foundry**, **Wasmtime / Cranelift**, and **Stockfish**. Member of **Solana Superteam KZ**.

[![Email](https://img.shields.io/badge/Email-mukhammedali%40berektassuly.com-blue?style=flat-square)](mailto:mukhammedali@berektassuly.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-berektassuly-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/mukhammedali-berektassuly)
[![Telegram](https://img.shields.io/badge/Telegram-@Berektassuly-26A5E4?style=flat-square&logo=telegram)](https://t.me/Berektassuly)
[![Blog](https://img.shields.io/badge/Blog-berektassuly.com-FF5722?style=flat-square)](https://berektassuly.com)
[![Habr](https://img.shields.io/badge/Habr-Berektassuly-65A3BE?style=flat-square&logo=habr)](https://habr.com/ru/users/Berektassuly/)

---

## Highlights

- **Merged PRs — [`txodds/tx-on-chain`](https://github.com/txodds/tx-on-chain)**: improved TxLINE developer onboarding, mainnet/devnet activation guardrails, API auth/SSE troubleshooting, and on-chain score-validation guidance ([#2](https://github.com/txodds/tx-on-chain/pull/2), [#4](https://github.com/txodds/tx-on-chain/pull/4))
- **Merged PR — [`foundry-rs/foundry`](https://github.com/foundry-rs/foundry/pull/15236)**: added `require-revert-in-loop`, a Solidity lint for `require` / `revert` inside loops, with matching [Foundry Book docs](https://github.com/foundry-rs/book/pull/1911)
- **Merged PR — [`rust-lang/rust`](https://github.com/rust-lang/rust/pull/157429)**: added a regression test for `unreachable_code` with the try operator
- **Merged PR — [`bytecodealliance/wasmtime`](https://github.com/bytecodealliance/wasmtime/pull/13632)**: fixed a public Cranelift JIT API by re-exporting `JITMemoryKind`
- **Merged PR — [`tokio-rs/tokio`](https://github.com/tokio-rs/tokio/pull/8202)**: documented runtime interaction with `fork()`
- **Merged commit — [`official-stockfish/Stockfish`](https://github.com/official-stockfish/Stockfish/commit/8416ccafff69698e2edd99ec08488147f8f37e34)**: cleaned up ARM universal build selection in Makefile / CI
- **2nd Place — National Solana Hackathon**: built an AI-assisted open-source reward allocation system and a compliance relayer
- **1st Place — iTechpreneur Battle**: awarded a full Rector's Grant for BSc

---

## Key Projects

### [chatpack](https://github.com/berektassuly/chatpack) · Rust, WASM

High-performance library for compressing chat exports (Telegram, WhatsApp, Instagram, Discord) for LLM/RAG pipelines. Published on [crates.io](https://crates.io/crates/chatpack).

| Metric | Value |
|---|---|
| Token reduction | **92% (13×)** — 11M → 850K tokens |
| Full-pipeline throughput | **~1.6M msgs/sec** (Criterion) |
| Parser throughput | **~3.3M msgs/sec** (Criterion) |

Browser version via WASM at **[chatpack.berektassuly.com](https://chatpack.berektassuly.com)** — files never leave your device.

**Ecosystem:** [`chatpack-cli`](https://github.com/berektassuly/chatpack-cli) · [`chatpack-web`](https://github.com/berektassuly/chatpack-web) · [`chatpack-python`](https://github.com/berektassuly/chatpack-python)

---

### [testable-rust-architecture-template](https://github.com/berektassuly/testable-rust-architecture-template) · Rust, PostgreSQL

Backend template demonstrating Clean Architecture with Axum and trait-based Dependency Injection.

- **Transactional Outbox** via `FOR UPDATE SKIP LOCKED` for reliable outbox processing
- Fast test feedback via mock implementations of DB and RPC dependencies
- Demonstrates dependency injection, outbox processing, and testable service boundaries.

---

### [solana-compliance-relayer](https://github.com/berektassuly/solana-compliance-relayer) · Rust, Solana

Compliance layer for Solana payments: integrates Range Protocol API for real-time AML/sanctions screening before on-chain settlement. Fail-closed architecture, configurable risk thresholds, persistent blocklist caching in Postgres.

Reviewed during development by engineers from QuickNode and Range Protocol.

---

## Writing

Technical posts on architecture patterns and real-world Rust engineering at **[berektassuly.com](https://berektassuly.com)** — covering trait-based DI, Solana dual-write safety (Saga/Outbox), and chatpack internals.
