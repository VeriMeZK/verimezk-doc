---
title: Face Verification
description: Perform liveness detection and biometric matching to verify the user's identity against the scanned document.
keywords:
  [
    VeriMeZK,
    face verification,
    liveness detection,
    biometric match,
    identity check,
  ]
slug: /features/face-verification
---

# Face Verification

After scanning an identity document, VeriMeZK performs **face verification** to ensure the user is present and matches the document photo.

## Goals

- Confirm the user is physically present through liveness checks.
- Match the live face with the document image.
- Prevent spoofing attempts such as printed photos or deepfakes.

## How It Works

1. The user grants camera access.
2. The system captures a live video stream.
3. Liveness detection prompts the user (for example, blink or turn).
4. Biometric matching compares:
   - The live capture
   - The document image (from the MRZ or embedded chip)

:::tip
The face verification module is optimised for speed and privacy, with all processing completed locally.
:::

## Privacy and Security

- No face data is uploaded or persisted.
- External API calls are not required.
- Only a yes/no match result is used for subsequent proof generation.

## Troubleshooting

- Provide even lighting and a neutral background.
- Remove sunglasses, masks, or hats when possible.
- Use a high-resolution webcam for best results.

:::warning
If liveness detection fails, the user is prompted to retry. This prevents spoofing and maintains verification integrity.
:::

## Next Step

Once face verification succeeds, proceed to [generate a ZK proof](./proof-generation.md) for the selected identity attribute.
