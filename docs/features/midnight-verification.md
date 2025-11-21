---
title: Midnight Verification
description: Learn how VeriMeZK integrates with the Midnight blockchain to verify zero-knowledge proofs on-chain.
keywords:
  [VeriMeZK, Midnight, blockchain, zk verification, smart contract, privacy]
slug: /features/midnight-verification
---

# Midnight Verification

VeriMeZK integrates with the **Midnight blockchain** to enable on-chain verification of zero-knowledge proofs without compromising user privacy.

## Why Midnight?

Midnight is a privacy-focused blockchain designed for confidential smart contracts. It supports zero-knowledge proofs and prevents sensitive data from appearing on-chain.

## How On-Chain Verification Works

1. The user connects a compatible wallet through the application.
2. The zero-knowledge proof is submitted to a Midnight smart contract.
3. The contract checks the proof against the requested rule.
4. The contract returns a success or failure result to the application.

:::tip
Midnight contracts can verify logic such as "is over 18" or "is a citizen of country X" without storing personal data.
:::

## Requirements

- Wallet connector (for example, a Midnight-compatible Web3 wallet)
- Testnet funds or mainnet tokens to cover gas fees
- A deployed smart contract with the required verification logic

## Example Use Case

A dApp wants to restrict access to users over 21:

- The user generates a proof locally in VeriMeZK.
- The proof is submitted to the Midnight contract.
- If the proof validates, the dApp grants access without learning the user's exact age.

## Privacy

- Document data is never stored on-chain.
- Biometric information is not transmitted.
- Only the proof artifact and the requested rule are present in the transaction payload.

## Next Step

Define bespoke rules with [custom checks](./custom-checks.md) to tailor Midnight verification to your product requirements.
