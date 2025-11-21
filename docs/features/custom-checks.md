---
title: Custom Checks
description: Define your own identity verification rules using VeriMeZK's flexible proof engine.
keywords: [VeriMeZK, custom checks, identity logic, zk rules, verification]
slug: /features/custom-checks
---

# Custom Checks

VeriMeZK lets teams define **custom identity verification rules**, enabling flexible, privacy-preserving logic tailored to each product.

## What Is a Custom Check?

A custom check is a logical rule that can be verified using zero-knowledge proofs. Examples include:

- "Is over 21"
- "Is from France"
- "Document is not expired"
- "Face matches the document photo"

## How to Define a Rule

Each rule typically includes:

- A **name** (for example, `isAdult`)
- A **condition** (for example, `birthdate <= today - 18 years`)
- A **data source** (for example, an MRZ field or biometric match)
- A **proof template** used to generate the ZKP

:::tip
Combine multiple conditions to create compound rules such as "is adult AND is an EU citizen."
:::

## Example

```json
{
  "rule": "isAdult",
  "condition": "birthdate <= today - 18y",
  "source": "document.MRZ.birthdate",
  "proof": "zkAgeProof"
}
```

## Reusable Logic

Custom checks can be reused across:

- Multiple applications
- Different user flows
- On-chain and off-chain verification

## Privacy

- Checks are evaluated locally.
- Only the result and proof are shared.
- Raw identity data stays on the device.

## Next Step

To integrate these checks into your application, review the [SDK methods](../api/methods.md) and the [architecture overview](../architecture.md).
