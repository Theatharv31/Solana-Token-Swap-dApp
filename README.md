# Solana Token Swap dApp

## Block Diagram 

![SwapFunctionalityDiagram](https://github.com/user-attachments/assets/492e8250-fc43-4a19-8709-737d40f07bb6)


## Overview
The Solana Token Swap dApp is a decentralized platform enabling secure token exchanges between two parties without the need for intermediaries. The platform leverages Solana's high throughput, low fees, and the Anchor framework to deliver a seamless token swap experience.

## Technical Details

### Structure
- **Offer Account:** Stores the details of a swap offer, including maker, token mints, and token amounts.
- **Vault Account:** Temporarily holds the maker's tokens during the swap process.
- **Anchor Framework:** Provides easy-to-use abstractions for creating and managing Solana programs.

### Key Functions
1. **Make Offer**
   - Creates an offer account linked to the maker's wallet.
   - Sets up a vault account to hold the maker's tokens.
   - Saves the offer details (token mints, amounts, etc.).
   
2. **Take Offer**
   - Validates and processes the taker's acceptance of the offer.
   - Transfers tokens from the taker to the maker.
   - Releases tokens from the vault to the taker.
   - Closes the offer and vault accounts.

---
