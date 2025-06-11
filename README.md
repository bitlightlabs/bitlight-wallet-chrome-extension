# Bitlight Wallet Chrome Extension

Bitlight Wallet is a Chrome Extension that provides a secure and user-friendly interface for managing Bitcoin and RGB
assets.

> **Note:** This repository serves as an archive for historical versions of the extension.

---

## Installation

1. Download the desired version from
   the [v0.14.1](https://github.com/bitlightlabs/bitlight-wallet-chrome-extension/tree/main/chrome-extension-0.14.1)
   folder.
2. Open Chrome and navigate to `chrome://extensions/`.
3. Enable **Developer mode** (top right corner).
4. Click **Load unpacked** and select the downloaded extension folder.

---

## Version Information

### Version 0.14.1

- supporting RGB protocol `v0.11.0-beta.9`.
- Derivation paths:
    - **BTC Mainnet:** `m/86h/0h/0h/0`
    - **RGB Mainnet:** `m/86h/0h/0h/9`

---

## Differences Between Chrome Extension v0.14.1 and v0.15.1+

- **v0.14.1** uses the following derivation path for RGB mainnet with UTXO binding:
    - `m/86h/0h/0h/9/*`
- UTXOs in v0.14.1 can be found at the above path:

  ![v0141-rgb-utxos.png](/images/v0141-rgb-utxos.png)

- **v0.15.1 and later** create RGB-related UTXOs at:
    - `m/86h/827166h/0h`  
      (where `coin_type` is a decimal encoding of the RGB string)

- If you cannot find RGB mainnet UTXOs in v0.15.1 or later, please use v0.14.1 to check:
    - [Installation instructions](#installation)

- **UTXO migration functionality** is available in v0.15.1 and later.

---