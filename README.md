Nietzsche’s Mustache — NET

Nietzsche’s Mustache (NET) is a community-driven meme token on Solana.

It is not a bank.
It is not a protocol.
It is not a yield promise.
It is a transparent, philosophical, and ironic experiment in crypto culture.

Token Information

* Name: Nietzsche’s Mustache
* Ticker: NET
* Chain: Solana
* Token Address: 5pZDTusrC2s16i9Zw8SHFnL4ew4R9C6G5kwmD6vWpump
* Origin: Pump.fun
* Website: https://netmustache.xyz

Purpose

NET was created as a response to the absurdity of crypto markets.

Markets move.
Narratives rise and collapse.
Liquidity appears and disappears.
Most tokens disappear quickly.

NET is being built slowly, transparently, and on-chain.

Transparency

This repository will be used to document:

* Token information
* Burn records
* Liquidity actions
* Public wallet information
* Project updates
* Community-facing roadmap

Core Principle

No false promises.
No guaranteed returns.
No artificial hype.

Only slow building, public records, and long-term discipline.

God is dead. Liquidity is alive.

Disclaimer

NET is a meme token and a high-risk crypto asset.

Nothing in this repository is financial advice.
Nothing here should be understood as a promise of profit, price performance, listing, or future value.

Every participant is responsible for their own decisions.
## Public Records

The main public records for NET are documented here:

- [Transparency Log](./TRANSPARENCY.md)
- [Tokenomics](./TOKENOMICS.md)
- [Burn Records](./BURNS.md)
- [Liquidity Records](./LIQUIDITY.md)
- [Staking Records](./STAKING.md)
- [Public Wallets](./WALLETS.md)
- [Roadmap](./ROADMAP.md)
- [Disclaimer](./DISCLAIMER.md)

## Current development snapshot — 17 October 2026

- [Complete NET website source and evidence package](./net-site-preview-2026-10-17.zip) — HTML, existing project artwork, finalized RPC responses and a Python evidence-replay script.
- [Verified listed-burn summary](./net-burn-summary-2026-10-17.json) — 71,000,002.366453 NET across seven listed transactions.
- [Finalized mint snapshot](./net-mint-snapshot-2026-10-17.json) — dated total-supply and authority observations.

**The website redesign is a local preview. It has not been published to netmustache.xyz.** No wallet transaction, trading bot or new paid infrastructure was activated in this work.

After downloading the source package, run:

```sh
unzip net-site-preview-2026-10-17.zip -d net-preview
cd net-preview
python3 tools/verify_burns.py evidence/2026-10-17
python3 -m http.server 8767 --bind 127.0.0.1 --directory site
```

Open http://127.0.0.1:8767/ in your browser. The replay script reads recorded RPC responses; it cannot sign or send transactions.
