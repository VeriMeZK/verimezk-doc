---
title: Security & Privacy
description: Learn how VeriMeZK ensures user privacy and protects against spoofing or data leaks.
keywords: [VeriMeZK, security, privacy, spoofing, data protection, ZK]
slug: /security
---

# Security and Privacy

VeriMeZK is designed with privacy and security safeguards for every stage of the verification flow.

## Core Principles

- **Client-side execution:** No backend services or persistent storage are required.
- **Zero-knowledge by default:** Proofs disclose only the verification result.
- **No tracking:** Analytics, cookies, and fingerprinting are intentionally excluded.

## Spoofing Protection

- Liveness detection guards against presentation attacks.
- Biometric matching validates that the live user matches the document image.
- Document authenticity checks flag cloned or tampered passports and IDs.

## Data Handling

- All processing remains in the browser.
- No uploads, logs, or cloud storage are involved.
- Only proof artifacts, never raw identity data, leave the user's device.

## Audits and Transparency

- The codebase is open-source for community review.
- Smart contracts support independent auditing before deployment.
