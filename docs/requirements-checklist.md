# EVMS Requirements Checklist

A starting checklist for an **electronic voucher management system RFP**. Mark each item as Mandatory, Desirable, or Not needed for your programme, and ask vendors to answer each one in their own words rather than with a simple "yes".

## Voucher lifecycle

- [ ] Batch generation with configurable PIN length and format  
- [ ] Import of externally generated batches  
- [ ] Defined voucher states with role-based state changes  
- [ ] Activation, blocking, unblocking, and expiry by batch, range, or serial  
- [ ] Reversal and re-issue rules with audit trail  

## Security

- [ ] PIN encryption at rest and in transit  
- [ ] PIN masking in all user interfaces and reports  
- [ ] Strong authentication for back-office, dealers, and APIs  
- [ ] Complete audit log of sensitive actions  
- [ ] Segregation of duties for generation, activation, and release  

## Distribution

- [ ] Multi-level reseller hierarchy  
- [ ] Dealer wallets, credit limits, and top-up  
- [ ] Price lists, discounts, and commissions per level  
- [ ] POS terminal support (Android / Linux) with offline handling  
- [ ] USSD, SMS, app, web portal, and partner API channels  

## Integration

- [ ] Redemption via the operator's charging or IN platform  
- [ ] Idempotent APIs with clear timeout and retry behaviour  
- [ ] Wallet, billing, and ERP integration as required  

## Reporting and reconciliation

- [ ] Daily reconciliation of inventory, sales, redemptions, and balances  
- [ ] Dealer statements and channel performance reports  
- [ ] Export formats for finance and regulators  

## Non-functional

- [ ] High-availability deployment with documented failover  
- [ ] Capacity for stated peak volumes, with load-test evidence  
- [ ] Monitoring, alerting, and support model with escalation  

## Migration

- [ ] Plan for live vouchers, dealer balances, and history  
- [ ] Parallel run and reconciliation checkpoints  
- [ ] Rollback plan  

## Related

See the main [README](../README.md). Product context: [electronic voucher management system](https://evdsystem.com/electronic-voucher-management-system-evd-telecom/).
