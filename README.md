# The Stellar Token Builder's Masterclass
Documenting the journey of building 60+ tokens on Stellar.
Follow my journey: https://medium.com/@mintonft
## 📖 Getting Started Guide

New to Stellar? Start with the step-by-step tutorial:

👉 [GETTING_STARTED.md](./GETTING_STARTED.md)

This guide covers everything from creating your first token to adding liquidity on Day 1.
## 🔒 Security Best Practices

Security is the foundation of every Stellar token. Here are the critical steps every builder must take:

### 1. Set Master Weight to Zero
After creating your issuing account, immediately set the master weight to 0. This prevents anyone with the original secret key from taking control.

### 2. Use Multiple Signers
Never rely on a single secret key. Use at least 2-3 signers:
- Hardware wallet (Ledger/Trezor) in a safe
- Mobile wallet for routine operations
- Backup in a separate location

### 3. Set Proper Thresholds
- **Low threshold:** 1 signature (allow trust, bump sequence)
- **Medium threshold:** 2 signatures (payments, offers)
- **High threshold:** 3 signatures (set options, account merge)

### 4. Use Authorization Required Flag
For regulated tokens or projects requiring KYC, set the "Authorization Required" flag to control who can hold your token.

### 5. Store Keys Securely
- Never store secret keys in plain text
- Never email or screenshot secret keys
- Use hardware wallets for high-value accounts
- Store recovery phrases offline

**Read more:** [Stellar Security: How to Protect Your Issuing Account](https://medium.com/@mintonft)
