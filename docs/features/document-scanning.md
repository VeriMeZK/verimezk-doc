---
title: Document Scanning
description: Learn how VeriMeZK extracts identity data from passports and ID cards using MRZ recognition.
keywords:
  [VeriMeZK, document scanning, MRZ, identity document, OCR, zero-knowledge]
slug: /features/document-scanning
---

# Document Scanning

VeriMeZK supports scanning identity documents, such as passports and ID cards, using **MRZ (Machine Readable Zone)** recognition. Document scanning is the first step in the verification flow.

## How It Works

- The user scans or uploads a document (for example, a passport).
- The system extracts the MRZ using optical character recognition (OCR).
- Extracted data is parsed into structured fields such as full name, birthdate, nationality, document number, and expiration date.

:::tip
VeriMeZK uses a lightweight OCR engine optimized for browser environments. No document data is sent to external servers.
:::

## Supported Input Methods

- **Webcam capture** for live scans
- **Image upload** supporting JPG, PNG, or PDF

:::warning
Ensure the MRZ zone is legible and well lit. Blurry or cropped images are likely to fail during parsing.
:::

## Sample MRZ

Example of a valid MRZ (from a passport):

```
P<UTOERIKSSON<<ANNA<MARIA<<<<<<<<<<<<<<<<<<<
L898902C36UTO7408122F1204159ZE184226B<<<<<10
```

## Privacy

- Scanning and parsing occur locally in the browser.
- Document data is neither stored nor transmitted.
- Only structured fields feed into subsequent proof generation.

## Next Step

After document scanning, proceed to [Face Verification](./face-verification.md) to confirm liveness and identity matching.
