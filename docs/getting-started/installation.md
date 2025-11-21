---
title: Installation Guide
description: Step-by-step instructions to install and run VeriMeZK locally for development and testing.
keywords:
  [
    VeriMeZK,
    installation,
    setup,
    zero-knowledge,
    zk,
    identity,
    Midnight,
    client-side,
  ]
slug: /getting-started/installation
---

# Installation Guide

Follow these steps to install **VeriMeZK** and prepare your environment for development or integration work.

## Prerequisites

Ensure your system meets the following requirements before proceeding:

- **Node.js** version 18 or later
- **npm** or **yarn**
- A current browser such as Chrome, Firefox, or Brave
- Working knowledge of JavaScript or TypeScript
- Optional familiarity with zero-knowledge proofs or blockchain concepts

:::tip
VeriMeZK runs entirely on the client side. You can experiment without deploying backend services.
:::

## Installation Steps

### 1. Clone the repository

```bash
git clone https://github.com/VeriMeZK/VeriMeZK.git
cd VeriMeZK
```

### 2. Install dependencies

Using npm:

```bash
npm install
```

Or with yarn:

```bash
yarn install
```

### 3. Start the development server

```bash
npm run dev
```

This command starts the local demo interface at `http://localhost:3000`.

## Verify the Setup

Once the app is running:

- You should see the VeriMeZK demo interface.
- Test by scanning a sample document or uploading a passport image.
- The app extracts MRZ data and prompts for face verification.

:::note
All processing stays on the user's device. No data is sent to external services, including during face verification or proof generation.
:::

## Troubleshooting

If you encounter issues:

- Confirm your Node.js version with `node -v`.
- Delete `node_modules` and reinstall dependencies:
  ```bash
  rm -rf node_modules
  npm install
  ```
- Review terminal output for missing dependencies or peer conflicts.
- On Windows, ensure the browser has permission to access the webcam.

:::warning
Privacy-focused browser extensions may interfere with the webcam or document scanning. Temporarily disable them during testing.
:::

## Next Steps

After installation, continue with:

- [Quickstart](./quickstart.md)
- [Core features](../features/document-scanning.md)
- [Architecture overview](../architecture.md)
