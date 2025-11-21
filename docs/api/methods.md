---
title: SDK Methods
description: Detailed reference of all SDK methods and their parameters.
keywords: [VeriMeZK, SDK, API, methods, reference]
slug: /api/methods
---

# SDK Methods

## `scanDocument()`

Scans and parses MRZ from a document.

```ts
const result = await scanDocument();
```

Returns:

```ts
{
  name: string;
  birthdate: string;
  nationality: string;
  documentNumber: string;
}
```

---

## `verifyFace()`

Performs liveness detection and biometric match.

```ts
const match = await verifyFace();
```

Returns: `true | false`

---

## `generateProof(rule: string)`

Generates a ZK proof for a given rule.

```ts
const proof = await generateProof("isAdult");
```

Returns: `ZkProofObject`

---

## `verifyProof(proof: ZkProofObject)`

Verifies a proof on-chain or off-chain.

```ts
const result = await verifyProof(proof);
```

Returns: `true | false`
