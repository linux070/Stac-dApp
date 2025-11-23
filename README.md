# Stac - Home of DeFi on Arc

An AI-powered decentralized finance (DeFi) platform built on Arc Network, combining token swapping, cross-chain bridging, and liquidity provision capabilities.

## Features

### 🏠 Homepage
- Live statistics dashboard with real-time platform metrics
- 24h trading volume, Total Value Locked (TVL), active users, and transaction count
- Quick action cards for easy access to Swap, Bridge, and Liquidity features
- Beautiful gradient hero section with Arc Network branding

### 💱 Swap
- Token-to-token exchanges with optimal routing
- Comprehensive swap quote simulation showing:
  - Expected output and minimum received
  - Price impact and exchange rate
  - Trading fees and gas estimates
  - Route visualization
- Adjustable slippage tolerance (0.1% - 50%)
- "Switch tokens" button for quick reversal
- Balance display and "MAX" button when wallet connected
- Supports ETH, USDC, USDT, DAI, WBTC

### 🌉 Bridge
- Secure cross-chain asset transfers between Ethereum Sepolia and Arc Testnet
- Chain swap button to reverse source/destination
- Estimated arrival time (2-5 minutes)
- Bridge fee display and breakdown
- Security warnings and best practices
- Supports ETH, USDC, USDT, DAI

### 💧 Liquidity
- **My Positions Tab:**
  - View all active liquidity positions
  - Track fees earned and pool share
  - APR display for each position
  - Add more or remove liquidity
- **Portfolio Tab:**
  - Complete wallet asset overview
  - Real-time USD values and 24h changes
  - Total portfolio value tracking
  - Quick actions for each asset

### 📊 Transactions
- **My Transactions:** Personal transaction history
- **All Transactions:** Platform-wide live feed
- Transaction persistence across page refreshes
- Real-time updates from Arc Testnet and Ethereum Sepolia
- Transaction filtering by type (Swap, Bridge, Add/Remove LP)
- Copy transaction hash and view on explorer
- Status indicators (Success, Pending, Failed)

### 🔐 Wallet Support
- MetaMask
- WalletConnect
- Coinbase Wallet
- Rabby Wallet
- Automatic network detection
- Balance display and refresh
- Network switching prompts

### 🎨 Design & UX
- **Theme:** Blue and white color blend with dark mode support
- **Responsive:** Fully responsive across mobile, tablet, and desktop
- **Animations:** Smooth transitions using Framer Motion
- **i18n:** Multi-language support (English, Spanish, Chinese, French)
- **Accessibility:** WCAG AA compliant contrast ratios

## Tech Stack

- **Frontend:** React 18 with Vite
- **Styling:** Tailwind CSS
- **Blockchain:** ethers.js v6
- **Animations:** Framer Motion
- **Internationalization:** react-i18next
- **Icons:** Lucide React
- **Charts:** Recharts

## Getting Started

### Prerequisites
- Node.js 18+ and npm
- MetaMask or another Web3 wallet

### Installation

1. Clone the repository:
\`\`\`bash
git clone https://github.com/yourusername/stac.git
cd stac
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
\`\`\`

3. Start the development server:
\`\`\`bash
npm run dev
\`\`\`

4. Open your browser and navigate to `http://localhost:3000`

### Building for Production

\`\`\`bash
npm run build
\`\`\`

The built files will be in the `dist` directory.

## Configuration

### Network Settings

Update the network configurations in `src/config/networks.js`:

- **Arc Testnet Chain ID:** Currently placeholder - update with actual Arc Testnet chain ID
- **RPC URLs:** Update with official Arc Testnet RPC endpoints
- **Contract Addresses:** Deploy smart contracts and update addresses

### Token Contracts

Update token addresses in `src/config/networks.js` for:
- USDC
- USDT
- DAI
- WBTC

## Smart Contracts

The platform requires the following smart contracts to be deployed:

1. **Swap Router:** Handles token swapping with optimal routing
2. **Swap Factory:** Creates and manages liquidity pools
3. **Bridge Contracts:** Lock-and-mint mechanism for cross-chain transfers
4. **LP Manager:** Manages liquidity positions

Contract interfaces and ABIs should be added to `src/contracts/` directory.

## Security

- Input sanitization for all user inputs
- Address validation with checksum verification
- Slippage protection
- Reentrancy guards in smart contracts
- No private key storage or handling
- Secure session management

## Roadmap

- [ ] Deploy smart contracts to Arc Testnet
- [ ] Integrate real blockchain data
- [ ] Add limit orders
- [ ] Implement real-time price feeds
- [ ] Add portfolio analytics dashboard
- [ ] Mobile app (React Native)
- [ ] Governance token and DAO

## Contributing

Contributions are welcome! Please read our contributing guidelines before submitting PRs.

## License

MIT License - see LICENSE file for details

## Support

For support, email support@stac.finance or join our Discord community.

## Acknowledgments

- Built on [Arc Network](https://docs.arc.network)
- Inspired by Uniswap and Relay.link
- OpenZeppelin for smart contract libraries

---

**Disclaimer:** This is testnet software for demonstration purposes. Never use real funds on testnets.
