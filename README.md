# Electronic Voucher Management System RFP Guide

An educational guide to writing a request for proposal (RFP) for an **electronic voucher management system (EVMS)**: what to ask vendors, which requirements matter most for telecom airtime, eTopup, and gift card programmes, and how to score the answers. Written for telecom operators, VAS partners, and payment platforms evaluating vendors, including the [EVD System](https://evdsystem.com/) platform from [MoboGage](https://evdsystem.com/about-mobogage/).

---

## What Is an EVMS RFP?

An **electronic voucher management system** generates, stores, distributes, activates, and redeems digital vouchers such as airtime PINs, data bundles, and gift cards, and tracks every voucher through its lifecycle. An **RFP** is the structured document an operator sends to vendors so their proposals can be compared on the same terms.

A good EVMS RFP does two things. It describes the operator's real situation (volumes, channels, integrations, markets) clearly enough that vendors can answer honestly. And it asks questions that separate a platform that has run in production from one that only looks good in a demo.

---

## RFP Structure

```
1. Background and objectives
2. Current state (existing system, volumes, channels, pain points)
3. Scope (in scope / out of scope)
4. Functional requirements
5. Integration requirements (IN/charging, billing, wallet, POS, APIs)
6. Non-functional requirements (availability, security, performance)
7. Migration and cutover
8. Commercial model and support
9. Evaluation criteria and timeline
10. Response format
```

A ready-to-adapt requirements checklist is in [docs/requirements-checklist.md](./docs/requirements-checklist.md).

---

## Key Requirement Areas

### 1. Voucher lifecycle

Ask how the system handles generation, batch import, storage, allocation, activation, sale, redemption, expiry, blocking, and reversal. Ask vendors to describe each state and who can move a voucher between states.

### 2. PIN security

Ask how PINs are generated, encrypted at rest, masked in user interfaces, and exposed only at the moment of sale. Ask who, if anyone, can view a PIN in clear text, and how that access is logged.

### 3. Distribution channels

List the channels you need: reseller POS terminals (Android or Linux), mobile app, USSD, SMS, web portal, and partner APIs. Ask how each one authenticates and what happens when a terminal is offline.

### 4. Reseller hierarchy and finance

Ask how many hierarchy levels are supported, how dealer wallets and credit work, how pricing and commissions are configured, and how statements are produced.

### 5. Integration with charging

For airtime, redemption has to reach the operator's intelligent network or online charging system. Ask which interfaces the vendor has integrated before and how they handle timeouts and duplicate requests.

### 6. Reconciliation and reporting

Ask for examples of daily reconciliation reports between sales, redemptions, inventory, and dealer balances. Reconciliation is where weak platforms show their gaps.

### 7. Availability and scale

Describe your peak periods and ask how the platform is deployed for failover, how it scales, and what the support model is during an incident.

### 8. Migration

If you are replacing an existing system, ask how live vouchers, dealer balances, and history will move, and what the cutover and rollback plan looks like.

---

## How to Score Responses

| Criterion | What good looks like |
|-----------|----------------------|
| **Functional fit** | Clear, specific answers mapped to each requirement, with gaps stated honestly |
| **Production evidence** | Reference deployments you can actually speak to |
| **Security** | Documented PIN handling, access control, and audit logging |
| **Integration experience** | Named interfaces already integrated, with a test plan |
| **Operations** | Monitoring, support hours, escalation, and incident process |
| **Migration plan** | Phased plan with reconciliation checkpoints and rollback |
| **Commercials** | Transparent licence or revenue-share model, with no hidden per-feature fees |

Weight the criteria before responses arrive, so scoring is not shaped by whichever demo was most polished.

---

## Common RFP Mistakes

- Copying a generic payments RFP that ignores voucher lifecycle and PIN security  
- Not sharing realistic volumes, so vendors either overprice or undersize  
- Asking yes/no questions that every vendor answers "yes"  
- Leaving migration out of scope, then discovering it is the hardest part  
- Skipping a proof of concept on the one integration that matters most  

---

## FAQ

**What is an electronic voucher management system?**  
A platform that manages digital vouchers such as airtime PINs and gift cards from generation through distribution, sale, and redemption, with security and reconciliation built in.

**What should an EVMS RFP include?**  
Background, current state, scope, functional and integration requirements, non-functional requirements, migration, commercial model, and clear evaluation criteria.

**How long does an EVMS selection usually take?**  
It varies widely with scope and procurement rules. Plan time for clarification questions, demos, a proof of concept, and contract negotiation.

**Should we run a proof of concept?**  
Usually yes, focused on the riskiest integration, often redemption against the charging system or the POS channel.

**How does this relate to MoboGage / EVD System?**  
EVD System is MoboGage's electronic voucher management and distribution platform. See the [electronic voucher management system](https://evdsystem.com/electronic-voucher-management-system-evd-telecom/) page and the guide on [how to choose an EVMS](https://evdsystem.com/evd-software/how-to-choose-electronic-voucher-management-system/).

---

## Further Reading / Related Industry Resources

- [Electronic voucher management system for telecom](https://evdsystem.com/electronic-voucher-management-system-evd-telecom/) — EVD System product overview  
- [How to choose an electronic voucher management system](https://evdsystem.com/evd-software/how-to-choose-electronic-voucher-management-system/) — buyer's guide  
- Related repo: [electronic-voucher-management-system-guide](https://github.com/iwtglobal/electronic-voucher-management-system-guide) — EVMS concepts and architecture  

---

## License

Documentation in this repository is provided under the MIT License. See [LICENSE](./LICENSE).

*Educational material only. Not legal or procurement advice. MoboGage and EVD System refer to offerings on evdsystem.com.*
