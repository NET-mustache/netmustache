# EXIT Protocol
## The Public Memory Layer for Autonomous Finance

> **Remember the agent. Verify the record. Inform the boundary.**

**Status:** Open Research Proposal  
**Version:** 0.4.1  
**Origin:** Nietzsche’s Mustache (NET) Research & Transparency Initiative  
**Document type:** Public architecture proposal  
**Token status:** No EXIT token exists  
**Repository status:** Research-stage publication

---

## Disclaimer

This document is a technical and strategic research proposal.

It is not:

- an investment offer;
- a token launch announcement;
- a promise of financial return;
- a guarantee of an airdrop;
- a commitment to create an EXIT token;
- legal, financial, or insurance advice;
- or a claim that the proposed architecture is complete.

No EXIT token, snapshot, allocation formula, valuation, launch date, or distribution commitment currently exists.

If a native token later becomes technically necessary for permissionless operator staking, decentralized attestation, or objective slashing, any token design would require a separate technical proposal, legal review, security review, and public governance process.

Any future recognition question is addressed exclusively in Section 35. Holding NET does not guarantee any EXIT allocation or financial benefit.

---

# 1. Executive Summary

The autonomous economy currently lacks a public memory.

Agent-wallet infrastructure can enforce private limits. Payment protocols can move value. Identity standards can establish who an agent claims to be. None of these systems, by themselves, answer:

- Who or what caused the transaction?
- Which human, organization, or principal ultimately controlled the agent?
- Which wallets, deployments, platforms, and related agents belong to the same history?
- Has the agent previously violated policies, been manipulated, or participated in harmful activity?
- What evidence supports those conclusions?
- Should a policy engine, merchant, exchange, wallet, or another agent trust this counterparty now?

EXIT Protocol is proposed as the public, evidence-based accountability layer for autonomous finance.

Its first product is the **Agent Accountability Layer**:

1. Agent Registry
2. Principal and wallet relationships
3. Agent Genealogy
4. Incident Ledger
5. Evidence standards
6. Dispute and correction process
7. Multi-dimensional Risk Profiles
8. Counterparty-risk Query API

EXIT does not attempt to replace the policy-enforcement infrastructure already being built by wallet and custody providers. Instead, it supplies the historical, cross-platform risk information those private policy engines cannot see.

EXIT also publishes an open Agent Guard specification covering instruction provenance, authority rules, execution policies, human approval, and transaction certificates. Enforcement may be performed by an EXIT reference implementation or by existing policy-engine partners consuming EXIT data.

Later, EXIT may expand into Market Integrity through realizable-value analysis, liquidity durability, related-wallet conditions, behavioral covenants, and risk-adjusted routing.

EXIT does not attempt to read an AI system’s mind. It gives the agent economy something it currently lacks:

# Memory.

The long-term question is:

> **Who is this agent, who stands behind it, what has it done before, what evidence supports the record, and how should that record affect what it is allowed to do next?**

---

# 2. The Problem

Crypto infrastructure has advanced rapidly.

The industry already has:

- high-performance L1 and L2 networks;
- smart contracts;
- decentralized exchanges;
- liquidity aggregators;
- MEV protection;
- price oracles;
- token-risk scanners;
- transaction simulation;
- wallet warnings;
- identity and wallet graphs;
- multisig systems;
- smart accounts;
- protocol insurance;
- on-chain monitoring;
- agent-wallet policy engines;
- agent-payment protocols;
- and agent identity and credential standards.

These systems solve important parts of the security problem.

But the decision chain remains fragmented.

A typical autonomous action may look like this:

```text
Public information
        ↓
Agent interpretation
        ↓
Tool call
        ↓
Transaction construction
        ↓
Wallet signature
        ↓
Blockchain execution
```

The blockchain confirms the final step.

It does not necessarily verify:

- whether the public information contained a hidden instruction;
- whether the agent was allowed to treat that source as authority;
- whether the action exceeded the owner’s budget;
- whether a new recipient required confirmation;
- whether the agent used an unapproved protocol;
- whether market conditions changed beyond the permitted limit;
- or whether the agent bypassed its own declared rules.

This creates a new class of financial risk:

# Valid but unauthorized execution.

There is also a second class of risk:

# Authorized but uninformed execution.

An agent may operate fully inside its private spending and protocol rules while interacting with a counterparty that has a documented history of compromises, policy violations, harmful deployments, or related high-risk principals. Existing policy engines can enforce the rules they know. They cannot act on public history that has not been organized into a portable, evidence-based record.

A technically valid transaction can still represent:

- prompt injection;
- social engineering;
- compromised API instructions;
- manipulated external content;
- excessive treasury exposure;
- policy bypass;
- unsafe routing;
- or an action the owner never intended to authorize.

The missing primitive is therefore not another generic risk score.

It is:

# A public memory between identity and enforcement — plus a verifiable boundary between information, instruction, authority, policy, and execution.

---

# 3. Enforcement Landscape 2026

By mid-2026, agent-wallet policy enforcement is no longer an empty category.

Production systems already provide combinations of:

- enclave or trusted-execution policy evaluation;
- spending limits;
- approved recipients and protocols;
- co-approval;
- kill switches;
- delegated keys;
- wallet-level allowlists;
- transaction simulation;
- and guarded execution.

Relevant infrastructure includes Turnkey, Privy/Stripe, Coinbase Agentic Wallets, Crossmint, MetaMask Guard Mode, AWS AgentCore payment integrations, smart-account frameworks, and institutional custody providers.

Agent-payment infrastructure is also advancing through systems such as x402, AP2, Skyfire, and other machine-payment rails. Agent identity is beginning to form through KYA-style credentials and registries such as ERC-8004.

These systems are important integration targets, not the first battlefield for EXIT.

Their policies are generally private and platform-specific. They can answer:

> “Does this proposed transaction satisfy the rules configured inside this wallet or platform?”

They generally cannot answer:

> “What has this counterparty agent and its principal done across platforms, wallets, deployments, and prior incidents?”

That is EXIT’s position.

> **The enforcement layer is being built. EXIT builds the public memory that enforcement remains blind to.**

---

# 4. Core Design Principle

EXIT is built around one principle:

> **Do not attempt to prove subjective intent when objective authority and policy compliance can be enforced.**

An AI system’s internal “intent” is difficult to measure.

The following questions are measurable:

- Was the command source authorized?
- Was the instruction signed?
- Was the proposed action permitted?
- Was the recipient approved?
- Was the spending limit respected?
- Was the protocol allowlisted?
- Was human approval required?
- Was the risk certificate current?
- Was the policy version valid?
- Did the final transaction match the approved transaction?

EXIT therefore uses:

# Policy-Constrained Execution

The system does not ask:

> “Did the agent mean well?”

It asks:

> “Was the agent permitted to do this?”

---

# 5. EXIT’s Three-Layer Architecture

EXIT combines three complementary layers.

## Layer One — Agent Memory

Agent Memory creates the first public, cross-platform record of autonomous financial actors through:

- Agent Registry;
- Principal and wallet relationships;
- Agent Genealogy;
- Incident Ledger;
- evidence standards;
- dispute and correction;
- Risk Profiles;
- and a counterparty-risk Query API.

This is EXIT’s first product and first implementation target.

## Layer Two — Agent Integrity

Agent Integrity defines open policy and provenance specifications for protecting autonomous financial actors from:

- unauthorized instructions;
- prompt injection;
- untrusted command sources;
- excessive spending;
- unsafe protocol calls;
- hidden or obfuscated commands;
- unauthorized recipients;
- policy bypass;
- and missing human approval.

EXIT publishes this layer as open schemas and a reference implementation. Existing policy engines may consume EXIT data and enforce the resulting limits. EXIT does not need to replace them.

## Layer Three — Market Integrity

Market Integrity adds execution-time economic constraints:

- realizable exit value;
- liquidity durability;
- concentration risk;
- creator and related-wallet activity;
- authority changes;
- covenant status;
- route quality;
- and market-stress conditions.

Agent Memory answers:

> **Who is this agent, who stands behind it, and what has it done before?**

Agent Integrity answers:

> **Is the actor authorized to perform the action?**

Market Integrity answers:

> **Is the action still inside the declared economic boundaries?**

Together they create:

# Verifiable Agent Accountability and Execution Integrity

---

# 6. Agent Memory: Registry, Genealogy, Incidents, and Risk

EXIT’s original Agent Guard thesis is strengthened by adding a public accountability layer before execution. Identity alone is not enough. A credential can establish who an agent is, but it cannot establish whether the agent has previously been compromised, violated policy, participated in harmful activity, or belongs to a principal with a recurring pattern of risky behavior.

EXIT therefore adds four connected components.

## Agent Registry

A machine-readable registry of autonomous agents, including:

- agent identity;
- principal or owner;
- deployer;
- controlled wallets;
- platform and framework;
- related agents;
- token deployments;
- fee destinations;
- first and last observed activity;
- and incident summary.

Every relationship must expose its evidence type and confidence level. Confirmed facts, strong inferences, probabilistic links, and unverified reports must never be presented as the same thing.

## Agent Genealogy

Wallet graphs place addresses at the center. EXIT places the agent at the center and maps:

```text
Agent
↔ Principal
↔ Deployer
↔ Wallets
↔ Platform
↔ Related agents
↔ Token deployments
↔ Fee destinations
↔ Incidents
```

The objective is to show not only where funds moved, but which autonomous actor, principal, infrastructure, and historical pattern the movement belongs to.

## Incident Ledger

EXIT should maintain standardized, evidence-based incident records containing:

- incident type and severity;
- affected agent and principal;
- trigger and instruction source;
- transaction evidence;
- economic impact;
- confidence level;
- dispute status;
- principal response;
- remediation;
- and final resolution.

The ledger records facts and clearly labels inference, allegation, dispute, correction, and resolution. It must include a visible correction and appeal process.

## Evidence-Based Risk Profile

EXIT should not begin with a single opaque score. The first profile should be multi-dimensional:

```text
Identity confidence
Principal transparency
Wallet transparency
Execution transparency
Policy-compliance history
Confirmed incidents
Unresolved incidents
Compromise history
Related high-risk entities
Remediation quality
Evidence freshness
Overall classification
```

Evidence comes before scoring. A numerical score may be introduced later only if the methodology is transparent, contestable, and supported by sufficient historical data.

## Closed Accountability Loop

The combined architecture creates a feedback loop:

```text
Agent behavior
→ Evidence
→ Incident Ledger
→ Risk Profile
→ Execution Policy
→ Limits and approvals
→ New behavior
→ Updated record
```

Past behavior can therefore affect future authority. A recently compromised agent may receive lower transfer limits. Repeated policy violations may require human approval. Strong remediation may improve the profile over time.

This is the central upgrade to EXIT: the protocol does not only block unsafe actions; it creates the memory of the autonomous economy and uses that memory to shape future execution.

---

# 7. First Product: Agent Accountability Layer

EXIT’s first product is a public, machine-readable accountability layer for autonomous agents.

It records:

- the agent;
- its principal or controlling organization;
- deployer and platform relationships;
- controlled and related wallets;
- related agents;
- token and contract deployments;
- fee destinations;
- evidence-based incidents;
- disputes and corrections;
- and multi-dimensional risk profiles.

EXIT Agent Guard is published alongside this product as an open policy and provenance specification. It is designed to integrate with — not compete against — existing policy-enforcement infrastructure such as Turnkey, Privy, Coinbase Agentic Wallets, Crossmint, smart-account frameworks, and institutional custody systems.

EXIT’s Query API can supply those systems with information they do not independently maintain:

```text
Is the counterparty a registered agent?
Who is its principal?
Has it been compromised?
Does it have unresolved incidents?
Is it linked to high-risk wallets or deployments?
What evidence supports the classification?
How fresh is the record?
```

## Who Is Recorded

The data subjects are:

- autonomous agents;
- their principals;
- controlled wallets;
- related agents;
- deployments;
- and publicly evidenced incidents.

Initial records do not require voluntary enrollment. Public on-chain evidence can be indexed and attributed under explicit evidence and confidence standards. Verified self-registration and platform cooperation may improve records later.

## Who Pays

Potential customers are:

- agent-wallet policy engines;
- agent platforms;
- exchanges;
- wallets and custodians;
- merchants and payment processors;
- counterparties interacting with agents;
- insurers and risk providers;
- researchers;
- and institutional treasury operators.

The product is therefore a two-sided information market: agents and principals are recorded; infrastructure providers and counterparties pay to query, integrate, monitor, or verify the record.

## Agent Guard’s New Role

Agent Guard has two roles:

1. **Open specification and reference implementation** — Execution Constitution, provenance schema, policy rules, approval requirements, and transaction certificates.
2. **Integration surface** — a standard by which existing enforcement systems consume EXIT’s registry, incident, and risk data at signing time.

EXIT may build its own firewall only as a reference implementation or fallback. The primary objective is to make public agent history portable across enforcement systems.

---

# 8. Policy and Provenance Specification

The following sections define EXIT’s open policy and provenance specification. Enforcement may be performed by an EXIT reference firewall or by existing policy-engine partners consuming EXIT data.

# 9. Execution Constitution

Every protected agent should have a machine-readable **Execution Constitution**.

This constitution defines the limits of the agent’s authority.

Example:

```yaml
agent_policy:
  version: 1

  identity:
    agent_id: "agent_042"
    owner: "owner_multisig"
    policy_controller: "governance_multisig"

  permitted_command_sources:
    - owner_multisig
    - approved_api
    - signed_scheduler

  untrusted_sources:
    - public_social_media
    - public_web_pages
    - unsigned_messages
    - decoded_external_payloads

  spending_limits:
    maximum_per_transaction_usd: 5000
    maximum_per_hour_usd: 10000
    maximum_per_day_usd: 20000
    maximum_treasury_exposure_percent: 5

  human_approval_required:
    - new_token_deployment
    - contract_upgrade
    - transfer_above_10000_usd
    - first_transfer_to_new_recipient
    - treasury_withdrawal_above_2_percent
    - new_command_source
    - new_protocol_integration

  allowed_chains:
    - solana
    - base

  allowed_protocols:
    - jupiter
    - cow_protocol
    - aave

  forbidden_actions:
    - transfer_to_unverified_address
    - reveal_private_credentials
    - execute_instruction_embedded_in_public_content
    - execute_decoded_or_obfuscated_command
    - bypass_policy_engine
    - use_unapproved_bridge
    - change_policy_without_delay

  emergency_conditions:
    - pause_after_abnormal_treasury_outflow
    - pause_after_governance_key_change
    - pause_after_provenance_violation
    - pause_after_conflicting_attestation
```

This constitution is not a marketing statement.

It is an enforceable execution boundary.

---

# 10. Instruction Provenance

Autonomous agents consume information from many sources:

- owners;
- multisigs;
- APIs;
- schedulers;
- social posts;
- websites;
- direct messages;
- other agents;
- market-data feeds;
- governance proposals;
- encoded or transformed content.

EXIT records how a proposed action was formed.

Example:

```text
Owner policy
      ↓
Approved scheduler
      ↓
Market-data request
      ↓
External website
      ↓
Agent interpretation
      ↓
Tool call
      ↓
Proposed transaction
```

The provenance system should record:

- authorized principal;
- command source;
- source classification;
- timestamps;
- content hashes;
- transformation steps;
- tools called;
- model or agent version;
- policy version;
- approval events;
- risk checks;
- proposed transaction hash;
- and final transaction hash.

Private prompts, credentials, or business logic do not need to be publicly exposed.

A hybrid model can use:

- encrypted off-chain storage for sensitive content;
- public hashes for integrity;
- signatures for source authentication;
- and on-chain anchors for timestamping and dispute evidence.

The system should be able to answer:

> **Which instruction caused this action, and was that instruction authorized to cause it?**

---

# 11. Command-Source Classification

Not all information should be allowed to become a command.

EXIT should distinguish between:

## Authorized instruction sources

Examples:

- owner multisig;
- signed operator API;
- approved scheduler;
- governance execution module;
- verified automation service.

## Data-only sources

Examples:

- public websites;
- X posts;
- Discord messages;
- Telegram messages;
- market news;
- analyst reports;
- external agent responses.

A data-only source may influence analysis.

It must not automatically acquire execution authority.

This distinction is central.

A public post can be valid market data.

It should not become a treasury command.

---

# 12. Policy Engine

The Policy Engine evaluates objective conditions.

## 12.1 Authority rules

- Only the owner multisig may authorize policy changes.
- Public content cannot authorize transfers.
- New command sources require approval.
- Unsigned instructions cannot trigger high-value actions.
- Decoded or obfuscated content cannot become an executable command.
- Governance actions require the designated governance authority.

## 12.2 Spending rules

- Maximum value per transaction.
- Maximum value per hour.
- Maximum value per day.
- Maximum percentage of treasury at risk.
- Maximum first-time transfer.
- Maximum exposure to a single asset.
- Maximum loss threshold.

## 12.3 Protocol rules

- Only approved protocols may be used.
- Only approved contract versions may be called.
- Contract upgrades invalidate prior approval.
- Unapproved bridges are blocked.
- Wrapped assets may be restricted.
- New program addresses require review.

## 12.4 Recipient rules

- First transfer to a new address requires confirmation.
- High-risk addresses are blocked.
- Sanctioned or compromised addresses are rejected.
- Recipient changes invalidate previous approval.
- Address substitution after approval is forbidden.

## 12.5 Trading rules

- Maximum slippage.
- Maximum price impact.
- Minimum expected output.
- Minimum remaining liquidity.
- Maximum leverage.
- Maximum position concentration.
- Maximum daily loss.
- Maximum exposure to unverified assets.

## 12.6 Human approval rules

- Token deployment.
- Treasury migration.
- Contract upgrade.
- Authority transfer.
- New recipient.
- Large transfer.
- Governance-key change.
- Emergency withdrawal.
- Policy change.
- First interaction with a new protocol.

---

# 13. Execution Firewall

The Execution Firewall sits between the agent’s decision system and the wallet or account capable of moving assets.

```text
Information and instructions
            ↓
Agent reasoning
            ↓
Proposed action
            ↓
EXIT Provenance Layer
            ↓
EXIT Policy Engine
            ↓
EXIT Risk Checks
            ↓
Pass / Reject / Pause / Human Approval
            ↓
Wallet or smart account
            ↓
Blockchain
```

A policy failure should be fail-closed.

The agent should not possess unrestricted unilateral authority.

Possible enforcement models include:

- smart-account modules;
- multisig policy modules;
- delegated session keys;
- limited execution keys;
- router programs;
- escrow programs;
- transaction co-signing;
- allowlisted program calls;
- hardware-wallet approval;
- institutional custody integration;
- Turnkey policy engines;
- Privy wallet policies;
- Coinbase Agentic Wallets;
- Crossmint on-chain limits;
- MetaMask Guard Mode;
- and compatible smart-account or custody systems.

The strongest architecture limits the authority of the agent’s key itself.

Even if the reasoning system is compromised, the execution boundary remains active.

---

# 14. Human Approval Layer

Human approval should not be required for every transaction.

That would destroy automation.

Instead, approval should be triggered by policy.

Examples:

```text
Normal trade below $2,000
→ automatic execution

First interaction with a new protocol
→ human approval

Transfer above $10,000
→ multisig approval

Contract upgrade
→ delayed multisig approval

Emergency treasury migration
→ emergency governance procedure
```

This creates controlled autonomy.

The agent remains useful without becoming unrestricted.

---

# 15. Execution Certificate

For an approved action, EXIT can produce a signed execution certificate.

Example:

```json
{
  "agent_id": "agent_042",
  "policy_version": "1.4",
  "command_source": "signed_scheduler",
  "source_authorized": true,
  "spending_check": "pass",
  "recipient_check": "pass",
  "protocol_check": "pass",
  "market_risk_check": "pass",
  "human_approval": "not_required",
  "certificate_timestamp": 1783682400,
  "expires_in_seconds": 10,
  "proposed_transaction_hash": "0x...",
  "certificate_signature": "0x..."
}
```

The certificate may be issued by EXIT’s reference implementation, by an enforcement partner consuming EXIT data, or through a co-signed model combining a policy engine with an EXIT risk attestation.

The certificate does not claim that the transaction will be profitable.

It proves that the transaction satisfied the declared policy at a specific time.

---

# 16. Transaction Integrity

A valid certificate must be bound to the exact transaction.

The system should prevent:

- recipient substitution;
- amount substitution;
- protocol substitution;
- route substitution;
- token substitution;
- delayed reuse;
- replay on another chain;
- and post-approval modification.

The approved transaction hash and the executed transaction must match.

If the transaction changes, the policy evaluation must run again.

---

# 17. Emergency Circuit Breaker

EXIT should support automatic pausing when predefined conditions occur.

Examples:

- abnormal treasury outflow;
- repeated policy violations;
- compromised command source;
- governance-key change;
- newly detected malicious contract;
- rapid token-authority change;
- stale or conflicting risk data;
- unexplained recipient change;
- unexplained policy update;
- suspicious provenance;
- execution outside the declared operating profile.

The circuit breaker’s first purpose is not punishment.

Its first purpose is containment.

The system should stop additional autonomous execution and require authorized review.

---

# 18. Layer Three — Market Integrity

Once the Agent Accountability Layer and its first enforcement integrations are functional, EXIT can expand into Market Integrity.

The goal is not to rebuild every mature data platform.

EXIT should integrate external intelligence and convert it into enforceable execution conditions.

Possible inputs:

- wallet and entity intelligence;
- token-risk APIs;
- holder concentration;
- mint and freeze authority;
- liquidity and routing data;
- price and volatility feeds;
- exploit databases;
- protocol allowlists;
- contract-risk data;
- creator and deployer history;
- related-wallet activity.

EXIT’s value is not another isolated dashboard.

Its value is:

# Turning information into consequences that partner enforcement systems can act on.

---

# 19. Realizable Value Module

Displayed portfolio value and realizable value are not always equal.

A position may appear valuable while having limited exit capacity.

The Realizable Value module may estimate:

- expected output for a defined position size;
- slippage across available routes;
- transaction fees;
- price impact;
- pool depth;
- liquidity durability;
- concentration risk;
- stress scenarios;
- and post-trade treasury exposure.

Example:

```yaml
market_integrity_policy:
  minimum_exit_ratio: 0.82
  maximum_price_impact_percent: 3.5
  minimum_post_trade_liquidity_usd: 300000
  maximum_single_asset_treasury_exposure_percent: 15
```

This is not a future-price prediction.

It is an execution-time risk boundary.

---

# 20. Economic Relationship Intelligence

Creator, deployer, market-maker, influencer, and related-wallet activity can matter.

EXIT should not attempt to rebuild every wallet graph from zero.

It can integrate external intelligence while applying transparent confidence levels.

Possible signals:

- common funding source;
- recurring transfer patterns;
- coordinated timing;
- launch-time allocations;
- related liquidity actions;
- repeated project history;
- shared infrastructure;
- bundle relationships;
- indirect creator funding.

The system should distinguish:

```text
Confirmed relationship
High-confidence relationship
Possible relationship
Unverified signal
```

Uncertain clustering must not be presented as certainty.

---

# 21. Behavioral Covenants

Future versions may support machine-readable behavioral commitments.

Examples:

- creator-related wallets may sell no more than a defined percentage;
- treasury spending may not exceed a weekly limit;
- minimum liquidity must remain above a threshold;
- token authorities must remain revoked;
- token unlock schedules must not change without notice;
- agent-controlled treasury exposure must remain inside policy.

A covenant should only contain measurable conditions.

Bad covenant:

> “The team will always support the community.”

Good covenant:

> “Declared creator-related wallets may not sell more than 0.5% of circulating supply during any rolling 30-day period.”

The purpose is to convert vague promises into measurable rules.

---

# 22. Risk-Adjusted Routing

A route with the highest output is not always the safest route.

Future EXIT routing may evaluate:

- expected output;
- slippage;
- MEV exposure;
- pool depth;
- liquidity durability;
- bridge risk;
- wrapped-asset risk;
- oracle freshness;
- protocol risk;
- covenant status;
- recipient risk;
- and execution-certificate availability.

Possible modes:

```text
Maximum Output
Balanced
Maximum Integrity
Policy-Protected Execution
```

---

# 23. What EXIT Will Not Rebuild

EXIT should not begin by recreating:

- agent-wallet infrastructure and policy engines such as Turnkey, Privy, Coinbase Agentic Wallets, Crossmint, thirdweb, Alchemy, Fireblocks, or smart-account frameworks;
- agent-payment protocols such as x402, AP2, Mastercard Agent Pay, or Skyfire;
- agent identity standards and KYA credential systems such as ERC-8004-style registries;
- wallet-intelligence platforms such as Arkham or Bubblemaps;
- token-risk products such as RugCheck or GoPlus;
- execution venues and aggregators such as Jupiter or CoW Protocol;
- oracles such as Chainlink or Pyth;
- or every security database.

These systems may become:

- customers;
- data providers;
- identity inputs;
- integration partners;
- enforcement partners;
- execution venues;
- or independent verification sources.

Their private policy engines enforce the rules they know.

EXIT supplies the public memory those rules cannot see.

The strategic principle is:

> **Do not rebuild enforcement. Build the evidence-based memory that makes enforcement informed.**

---

# 24. Tokenless MVP

EXIT should begin without a native token.

The first MVP consists of five modules.

## Agent Registry and Schemas

Publish machine-readable schemas for:

- agent records;
- principal relationships;
- wallet relationships;
- incident records;
- evidence classes;
- dispute status;
- and risk profiles.

## Incident Report #001

Publish one complete, evidence-standard incident report based on a documented autonomous-agent event.

The report should demonstrate:

- timeline reconstruction;
- agent and principal attribution;
- wallet flows;
- command or trigger source;
- economic impact;
- confidence levels;
- unresolved questions;
- dispute handling;
- and remediation.

## Genealogy Graph and Public Dashboard

Build a public interface connecting:

```text
Agent
↔ Principal
↔ Wallets
↔ Platform
↔ Deployments
↔ Fee destinations
↔ Related agents
↔ Incidents
```

## Counterparty-Risk Query API

The API should be designed first for signing-time consumption by policy engines and counterparties.

Example response fields:

- registration status;
- identity confidence;
- principal confidence;
- unresolved incident count;
- compromise history;
- related high-risk entities;
- evidence freshness;
- dispute status;
- and recommended policy flags.

## Agent Policy Specification

Publish the Execution Constitution, provenance, risk-input, and execution-certificate schemas as an open specification.

The first phase does not require a production firewall. Provenance logging and a reference firewall move to the pilot-integration phase.

## MVP Success Definition

The first phase succeeds through measurable adoption and evidence quality:

- agents and principals registered with evidence;
- incidents documented to the published standard;
- relationships corrected through the dispute process;
- API queries served;
- and at least one external policy engine, platform, wallet, or counterparty evaluating the API for integration.

It does not succeed merely because it has a token or community attention.

---

# 25. First 90 Days

## Days 1–30

- Publish EXIT Protocol v0.4.
- Define Agent Registry and Incident Ledger schemas.
- Define evidence classes and dispute procedures.
- Select the first documented agent incident.
- Map public agent platforms on Solana and Base.

## Days 31–60

- Publish EXIT Incident Report #001.
- Build the initial agent and principal registry.
- Create a basic genealogy graph.
- Publish a public dashboard prototype.
- Open structured evidence and dispute submissions.

## Days 61–90

- Release a basic query API.
- Publish the first multi-dimensional risk-profile methodology.
- Add correction and appeal workflows.
- Publish the Agent Guard policy specification.
- Approach one agent platform for a pilot integration.
- Begin at least one data-integration discussion with a policy-engine or wallet-infrastructure provider.
- Replay historical incidents against the proposed controls.

---

# 26. Development Roadmap

## Phase 0 — Research and Specification

- Define the threat model.
- Define objective versus subjective checks.
- Publish the policy schema.
- Publish the provenance schema.
- Identify historical incidents.
- Interview agent developers.
- Interview DAO and treasury operators.
- Map existing wallet and smart-account integrations.
- Publish a public request for criticism.

## Phase 1 — Tokenless Registry and Ledger

- Agent Registry.
- Principal and wallet attribution.
- Genealogy graph.
- Incident Ledger.
- Evidence and dispute standards.
- Risk-profile methodology.
- Public dashboard.
- Counterparty-risk Query API.

## Phase 2 — Pilot Integrations

Two parallel pilots should be pursued:

**Agent-platform pilot**

- integrate one voluntary agent or platform;
- add provenance logging;
- test the open policy specification;
- publish transparent pilot reports.

**Policy-engine data-customer pilot**

- provide signing-time counterparty-risk queries;
- map EXIT flags to an existing policy engine;
- measure query latency, false positives, false negatives, and record freshness;
- define production thresholds with the pilot partner.

A reference firewall, emergency pause, and transaction-bound certificates may be implemented where required for testing.

## Phase 3 — Market Integrity Modules

- Realizable Value module.
- Liquidity durability checks.
- Protocol-risk integration.
- Recipient and wallet intelligence.
- Risk-adjusted routing.
- Creator and related-wallet conditions.
- Behavioral covenant prototype.

## Phase 4 — Multi-Agent and Multi-Chain

- Base and EVM support.
- Smart-account integrations.
- Multisig integrations.
- Institutional policy controls.
- Cross-chain policy consistency.
- Multi-agent delegation controls.

## Phase 5 — Independent Attestation

- Multiple independent operators.
- Operator reputation.
- Conflicting-attestation handling.
- Objective fault rules.
- Attestation availability guarantees.
- Economic security research.

## Phase 6 — Token Decision

A native token is considered only if the protocol proves a real requirement for:

- permissionless operators;
- independent attestation;
- economically punishable false reporting;
- decentralized security capacity;
- or protocol-level collateral.

---

# 27. When a Native Token Could Be Justified

A token should not exist merely to:

- finance development;
- attract attention;
- manufacture governance;
- reward social activity;
- create speculative demand;
- or imitate other infrastructure projects.

A token may become technically justified when independent operators must stake collateral before issuing attestations.

Possible future functions:

- operator stake;
- objective slashing;
- attestation capacity;
- delegated security;
- incident bounties;
- operator reputation;
- protocol parameter governance.

A conceptual stake model:

```text
Required Operator Stake
=
Value at Risk
× Policy Complexity
× Agent Risk Coefficient
× Operator Error Coefficient
```

Users should still be able to pay product fees in assets such as SOL, ETH, or stablecoins.

Native-token demand should come from security capacity, not forced friction.

---

# 28. Objective Slashing Only

AI may assist with:

- anomaly detection;
- provenance analysis;
- threat classification;
- and incident investigation.

AI should not independently impose financial punishment based on subjective interpretation.

Possible objectively slashable events:

- signing conflicting certificates;
- issuing an attestation without required checks;
- reporting an incorrect on-chain fact;
- using an expired policy;
- bypassing mandatory approval;
- falsifying provenance;
- certifying a transaction different from the executed transaction;
- or failing a clearly defined service obligation.

Prediction errors and subjective judgments require separate treatment.

---

# 29. Slashing, Warranty, and Insurance Must Be Separate

EXIT’s first version should not promise automatic financial compensation for losses.

The architecture should separate:

1. policy enforcement;
2. operator fault;
3. protocol slashing;
4. user compensation;
5. licensed insurance or coverage.

Direct compensation may create legal and regulatory obligations.

Any future warranty or insurance product should require:

- specialized legal advice;
- jurisdictional analysis;
- capital-model review;
- risk-pricing expertise;
- and potentially a licensed external partner.

Calling a mechanism “slashing” does not automatically prevent it from being treated as insurance or another regulated financial product.

Publishing evidence-based incident records about identifiable principals creates a separate publisher-liability and defamation risk. Before public launch, the project requires jurisdiction-specific analysis covering publication venue, the evidence threshold required for each claim severity, correction and safe-harbor mechanisms, and the legal weight of the dispute and appeal process.

---

# 30. Security Threat Model

EXIT must assume that attackers may target:

- the agent model;
- command sources;
- APIs;
- policy controllers;
- data providers;
- operator nodes;
- wallets;
- signing devices;
- smart contracts;
- human approvers;
- and the registry and incident ledger themselves.

Important threat classes include:

## 30.1 Prompt injection

Untrusted content attempts to become an instruction.

## 30.2 Source impersonation

An attacker pretends to be an authorized source.

## 30.3 Policy bypass

The agent attempts to call the wallet without policy evaluation.

## 30.4 Transaction substitution

The approved transaction is replaced before execution.

## 30.5 Stale approval

An old certificate is reused after conditions change.

## 30.6 Malicious policy update

An attacker weakens the policy before executing an action.

## 30.7 Data-provider compromise

External risk data becomes false or unavailable.

## 30.8 Operator collusion

Independent attestation operators coordinate dishonestly.

## 30.9 Human-approval compromise

The approving device or multisig participant is compromised.

## 30.10 Denial of service

Attackers attempt to freeze legitimate autonomous operations.

## 30.11 Reputation poisoning

An attacker submits fabricated or misleading incident evidence to damage a competing agent or principal. The evidence standard, confidence labeling, and dispute process are the primary defenses; submissions that cannot meet the published evidence threshold must not enter the public record as confirmed claims.

## 30.12 Sybil agent identities

A principal redeploys an agent under a new identity to reset its history. Genealogy must therefore be derived from wallet, funding, deployer, and principal relationships — not from self-declared agent identity — so that a reputation reset requires abandoning the underlying economic infrastructure, not just the name.

---

# 31. Privacy Architecture

Provenance must not require public disclosure of:

- private prompts;
- API secrets;
- trading strategies;
- internal reasoning;
- customer information;
- or institutional policy details.

Possible privacy design:

- private encrypted event logs;
- public event hashes;
- selective disclosure;
- zero-knowledge policy proofs;
- signed policy results;
- and time-stamped on-chain anchors.

The protocol should prove compliance without forcing unnecessary disclosure.

---

# 32. Governance

EXIT can begin with open technical governance before token governance.

Initial governance tools:

- GitHub issues;
- request-for-comment documents;
- public design discussions;
- security reviews;
- transparent milestones;
- contributor acknowledgements;
- and versioned specifications.

Governance does not require a token on day one.

Technical legitimacy should come before token voting.

---

# 33. NET’s Role

NET began as a memecoin.

It later became:

- a public experiment in transparency;
- a study of liquidity behavior;
- a market-observation project;
- a bounty environment;
- a token-incentive laboratory;
- and a cultural critique of crypto market structure.

EXIT can emerge from this research without rewriting NET’s history.

The honest relationship is:

> **NET observed the market, documented its absurdities, and created the research environment from which EXIT emerged.**

The projects remain distinct.

## NET

- culture;
- research;
- transparency;
- community;
- experimentation;
- public market observation.

## EXIT

- public agent memory and accountability product;
- evidence and policy standards;
- integration surface for enforcement infrastructure;
- autonomous-finance protection;
- market-integrity expansion.

NET is not automatically converted into EXIT.

EXIT is not presented as a guaranteed financial benefit for NET holders.

---

# 34. NET Recognition Policy

Any future recognition question is governed exclusively by the public statement in Section 35. No separate allocation category, snapshot, percentage, or eligibility rule is promised in this document.

---

# 35. Recommended Public Statement on NET and EXIT

> EXIT currently has no token, no snapshot, and no promised distribution. If a native token later becomes technically necessary for permissionless operator staking, independent attestation, or objective slashing, the project may present a separate community proposal exploring possible recognition of historical NET participants, verified contributors, researchers, bounty participants, security reporters, developers, documentation contributors, translators, and testnet users. Any future decision would depend on technical necessity, legal review, security design, anti-Sybil protections, and public governance. Holding NET does not guarantee an EXIT allocation or financial benefit.

---

# 36. Why No Immediate Airdrop Promise Exists

An immediate promise could:

- turn EXIT into a speculative extension of NET;
- create buying based on future-distribution expectations;
- attract Sybil wallets instead of builders;
- create snapshot manipulation;
- complicate legal analysis;
- force token design before product-market fit;
- and weaken EXIT’s credibility as infrastructure.

The community should be rewarded for helping build a real security standard.

It should not be encouraged to buy one token solely because another token may someday exist.

---

# 37. Revenue Model

EXIT should generate external revenue.

The priority order should follow the first product:

1. **Counterparty-risk Query API** — subscription or usage-based access for policy engines, wallets, platforms, exchanges, merchants, and institutional counterparties.
2. **Platform integration licenses** — verified and evidence-linked agent profiles, genealogy, monitoring, and incident feeds.
3. **Incident-analysis and forensic services** — structured investigations and evidence reports.
4. **Enterprise monitoring and policy-data subscriptions** — alerts, record changes, remediation tracking, and principal exposure.
5. **Agent Guard and policy-specification integrations** — implementation, support, and certificate services.
6. **Future independent attestation fees** — only after an operator network exists.

Revenue should not depend on token emissions.

---

# 38. Defensibility

EXIT’s core moat is the accumulated, evidence-labeled behavioral dataset of autonomous agents — the same category of moat that made credit bureaus durable: not merely technology, but accumulated record plus institutional trust.

Code can be copied.

A dashboard can be copied.

A risk score can be copied.

EXIT’s long-term defensibility may come from:

- standardized policy schemas;
- agent and wallet integrations;
- provenance history;
- historical incident datasets;
- execution-certificate adoption;
- external data-provider integrations;
- independent operator reputation;
- and security capacity backed by accountable capital.

The strongest network effect is not speculation.

It is becoming the independent public record that policy and counterparties consult before autonomous money is allowed to move.

---

# 39. Success Metrics

Registry and evidence metrics come first:

- registered agents;
- attributed principals;
- evidence-backed wallet and platform relationships;
- incidents documented to the published standard;
- percentage of claims by evidence class;
- dispute-resolution time;
- correction rate;
- record freshness;
- Query API volume;
- external data customers;
- policy-engine integrations;
- agent-platform integrations;
- and recurring revenue from non-token products.

Pilot enforcement metrics include:

- signing-time query latency;
- false-positive rate;
- false-negative rate;
- stale-record rate;
- policy-decision latency;
- risky actions escalated;
- and transaction certificates issued.

Production thresholds should be agreed with pilot partners before launch. Low-latency trading use cases may require materially stricter limits than treasury or merchant workflows.

Token price is not a protocol-security metric.

---

# 40. Open Research Questions

1. What is the minimum policy schema that works across different agent frameworks?
2. How should private provenance be proven without revealing sensitive content?
3. Which checks belong off-chain?
4. Which checks must execute on-chain?
5. How can an agent be prevented from bypassing the firewall?
6. How should delegated execution keys be limited?
7. How should policy changes be approved and delayed?
8. How should conflicting attestations be resolved?
9. Which failures are objectively slashable?
10. How can false positives avoid freezing legitimate operations?
11. How should emergency recovery work?
12. Which wallet and smart-account systems should be integrated first?
13. Which risk providers should be treated as inputs?
14. How should data-provider conflicts be handled?
15. How should execution certificates expire?
16. How should multi-agent delegation work?
17. How should cross-chain policy consistency be maintained?
18. What legal structure is required before economic guarantees are offered?
19. When does a native token become technically necessary?
20. How should early NET participation be recognized without creating a premature promise?
21. Which evidence standard is sufficient to publish an incident about an identifiable principal in each relevant jurisdiction?
22. How should agent identity continuity be established across redeployments to prevent reputation resets?
23. What data format do existing policy engines need to consume counterparty-agent risk at signing time?

---

# 41. Proposed Repository Structure

```text
exit-protocol/
├── README.md
├── DISCLAIMER.md
├── CONTRIBUTING.md
├── LICENSE
├── docs/
│   ├── architecture.md
│   ├── agent-registry.md
│   ├── agent-genealogy.md
│   ├── incident-ledger.md
│   ├── evidence-standard.md
│   ├── dispute-process.md
│   ├── risk-profile.md
│   ├── policy-schema.md
│   ├── provenance-standard.md
│   ├── execution-firewall.md
│   ├── execution-certificate.md
│   ├── market-integrity.md
│   ├── objective-slashing.md
│   ├── net-community-policy.md
│   └── roadmap.md
├── incidents/
│   └── EXIT-INC-0001.md
├── research/
│   ├── agent-platform-map.md
│   ├── historical-incidents.md
│   ├── market-data-landscape.md
│   ├── agent-infrastructure-landscape.md
│   ├── privacy-model.md
│   ├── legal-questions.md
│   └── open-questions.md
├── schemas/
│   ├── agent-record.schema.json
│   ├── incident-record.schema.json
│   ├── risk-profile.schema.json
│   ├── agent-policy.schema.json
│   ├── execution-certificate.schema.json
│   └── provenance-record.schema.json
├── examples/
│   ├── example-agent-record.yaml
│   ├── example-incident.yaml
│   ├── example-risk-profile.yaml
│   ├── example-agent-policy.yaml
│   └── example-certificate.json
├── api/
│   ├── openapi.yaml
│   └── counterparty-risk.md
└── sdk/
    └── README.md
```

For the first public release inside the NET repository:

```text
research/exit-protocol-open-research-proposal-v0.4.md
```

A separate EXIT repository should be created when implementation begins.

---

# 42. Contribution Areas

Contributors may help with:

- AI-agent security;
- prompt-injection threat models;
- Solana program design;
- EVM smart accounts;
- multisig integration;
- delegated session keys;
- policy-language design;
- provenance architecture;
- privacy and cryptography;
- risk-provider integration;
- historical incident research;
- legal and regulatory analysis;
- SDK development;
- testing;
- documentation;
- translation;
- and bounty design.

---

# 43. Final Position

EXIT should not begin by trying to replace production wallet-policy and execution infrastructure.

It should begin with one measurable mission:

> **Give the autonomous economy a memory it cannot fake — and make that memory shape what agents are allowed to do next.**

EXIT’s first product is the Agent Accountability Layer:

```text
Agent Registry
      +
Principal and Wallet Genealogy
      +
Incident Ledger
      +
Evidence and Dispute Standards
      +
Multi-Dimensional Risk Profiles
      +
Counterparty-Risk Query API
```

Existing policy engines can consume that memory when evaluating:

- recipients;
- counterparties;
- transaction limits;
- human approval;
- collateral requirements;
- and protocol access.

EXIT Agent Guard remains an open policy and provenance specification, a reference implementation, and an integration surface — not the first product category in which EXIT attempts to outbuild established infrastructure providers.

Market Integrity remains the later expansion layer through realizable value, liquidity durability, behavioral covenants, related-wallet conditions, and risk-adjusted routing.

The strategic principle is:

> **The execution layer is being built. EXIT builds the public memory that execution remains blind to.**

NET watched the market.

EXIT creates the memory and boundaries of autonomous money.

---

# 44. Closing Statement

> **Remember the agent.**  
> **Verify the record.**  
> **Inform the boundary.**

---

# Version Note

**v0.4 — Repositioned after enforcement-layer market analysis (July 2026): the Agent Accountability Layer is promoted to the first product; Agent Guard is reframed as an open specification, reference implementation, and data feed for existing policy-enforcement infrastructure.**

**v0.4.1 — Consistency revision (July 2026): three-layer architecture wording unified; stale v0.3 section numbering corrected (12.x policy rules, 30.x threat classes); duplicate list items removed; Market Integrity heading and prerequisites updated to the new first product; threat model extended with reputation poisoning (30.11) and Sybil agent identities (30.12); registry and incident ledger added as protected assets; NET-recognition cross-references corrected to Section 35; formatting normalized.**

---

# 45. Discussion Status

This proposal is open for criticism.

The project is specifically seeking:

- technical objections;
- competing architectures;
- security concerns;
- privacy concerns;
- legal questions;
- integration suggestions;
- evidence that proposed components already exist;
- and proposals that simplify the architecture.

A protocol that may one day influence financial trust should first survive public criticism.
