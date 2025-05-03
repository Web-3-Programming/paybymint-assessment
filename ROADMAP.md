# Project Roadmap: PayByMint

## Phase 0: Dev Environment & Tooling
> Goal: Provide a stable local and cloud-based development environment.

- [x] Hardhat setup with ERC-1155 smart contracts
- [x] Gitpod integration with configured RPC
- [x] MetaMask and testnet support
- [x] Compile + deploy support via `npx hardhat`
- [~] `.env` support for private keys and Infura

## Phase 1: MVP Core Marketplace
> Goal: Build the foundational smart contract and frontend for minting, buying, and listing NFTs.

- [x] Wallet connection (MetaMask, Binance)
- [x] Multi-chain support (Ethereum, Binance Smart Chain)
- [x] ERC-1155 fractional NFT smart contracts
- [x] Mint NFTs with metadata and maxSupply
- [x] Primary sales listing via `createSale`
- [x] Transfer logic for purchase and cancel
- [x] Fetch and display NFTs via `getSales()`
- [~] Auto-approval for marketplace contract
- [ ] Secondary listing flow (resale)
- [ ] Backend indexer for sales tracking

## Phase 2: Creator Tools & Metadata
> Goal: Let creators launch NFTs with IPFS metadata and price configuration.

- [x] Create Item UI with name, desc, price, email
- [x] Upload files and metadata to IPFS via Infura
- [x] Form validation and preview logic
- [x] Mint and auto-store URI on-chain
- [x] Airdrop minting support via `airdropAmount`
- [~] Expose metadata via `tokenURIs` in frontend
- [ ] Email confirmation logic after mint
- [ ] Creator dashboard with live NFT stats

## Phase 3: Listings & Marketplace Engine
> Goal: Enable dynamic listings, secondary sales, and item display.

- [x] Create listings via `createSale()`
- [x] Cancel listing logic via `cancelSale()`
- [x] Purchase logic with transfer and payment
- [x] Get listings by token or user
- [x] Swiper + card UI for homepage display
- [ ] UI for cancelling or editing listings
- [ ] Relist UI for fractional holders
- [ ] Sorting, trait filters, and categories
- [ ] Listing DB to track seller, price, timestamp

## Phase 4: User Profiles & Inventory
> Goal: Enable users to view their owned, created, and listed NFTs.

- [x] `getTokenIdByUser()` fetch by address
- [ ] "My NFTs" dashboard
- [ ] Earnings tracking using backend `Earn` model
- [ ] Receipt and transaction logs per mint
- [ ] Creator badges and verification

## Phase 5: Merchant Tools & Launchpad
> Goal: Create business-facing interfaces for using NFTs as commerce tools.

- [x] Fractionalized supply via `maxSupplys`
- [x] Dynamic pricing over supply thresholds
- [x] Creator-payout logic on mint
- [ ] Set/update `fractionPrice()` through UI
- [ ] Launchpad to mint full collections
- [ ] Wallet-based identity + ENS
- [ ] Sales stats: % sold, price floor, active listings

## Phase 6: Analytics, SEO & Performance
> Goal: Optimize for discovery, searchability, and growth.

- [x] Display trending NFTs (by views, sales)
- [ ] Search engine optimization (OpenGraph, sitemaps)
- [ ] Image CDN, IPFS cache layer
- [ ] Collection pages with filters and stats
- [ ] Shareable links and social previews

## Phase 7: DevOps & Testing
> Goal: Ensure stable testing, secure deployment, and reproducible environments.

- [x] Hardhat compile and deploy
- [x] Gitpod with test RPC for MetaMask
- [~] `.env` for Infura and secrets
- [ ] Add unit tests for minting, listing, airdrops
- [ ] Add UI/integration tests (Cypress or Playwright)
- [ ] Auto-deploy staging via GitHub Actions
- [ ] Version control for smart contracts

---

## Phase 8: Smart Contract Extensions
> Goal: Extend protocol with royalties, auctions, and moderation tools.

- [ ] ERC-2981 royalty support
- [ ] Sale expiration timestamps
- [ ] Pause minting per token
- [ ] Dynamic URI updates (optional)
- [ ] Merkle drops or whitelisting
- [ ] Creator-editable metadata in future versions

## Phase 9: Advanced Features
> Goal: Introduce sophisticated trading tools, expand wallet support, and build out user engagement features to enhance the marketplace ecosystem.

- [ ] Bulk listing and delisting tools
- [ ] Make Offers feature (on listed or unlisted NFTs/collections)
- [ ] Integration of additional wallet providers (e.g., WalletConnect, Coinbase Wallet, Rainbow)
- [ ] User Rewards Program / Loyalty system (e.g., earning points/tokens for activity)
- [ ] Portfolio tracking and historical analytics for users
- [ ] Integration or display of rarity data for collections
- [ ] Floor sweeping functionality
- [ ] Explore integration of non-ERC standards (e.g., Bitcoin Ordinals, if applicable)
- [ ] Design and plan for a potential Native Marketplace Token and Governance Model (DAO)

## Ideas / Backlog
- Mobile PWA support
- Bitcoin Ordinals integration
- Referral and affiliate incentives
- WalletConnect, Coinbase Wallet, Rainbow
- Verified creator badge & ratings
- Social feed of purchases and mints