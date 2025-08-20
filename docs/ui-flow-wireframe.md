# DIN (Dinyk) UI Flow Wireframe
## Decentralized Insurance Platform on Kaia Blockchain

This document outlines the UI flow and wireframe structure for the DIN (Decentralized Insurance) platform based on the whitepaper specifications.

---

## 🎯 Overview

DIN is a decentralized insurance platform on Kaia blockchain that provides parametric insurance products. Users can either purchase insurance for risk hedging or provide liquidity to earn premiums and staking rewards.

### User Types
1. **Insurance Buyers** - Purchase insurance to hedge against risks
2. **Insurance Providers (LP)** - Deposit USDT to underwrite insurance and earn premiums + staking rewards

---

## 📱 Main Navigation Structure

```
┌─────────────────────────────────────────────────┐
│                   Header                         │
│  [DIN Logo]  Insurance  Liquidity  Portfolio     │
│                              [Connect Wallet]     │
└─────────────────────────────────────────────────┘
```

### Navigation Items
- **Insurance** → Insurance catalog and purchase flow
- **Liquidity** → Liquidity provision dashboard
- **Portfolio** → User's positions and claims
- **Wallet** → Connection status and balance

---

## 🏠 Landing Page

### Hero Section
```
┌─────────────────────────────────────────────────┐
│                                                   │
│         Decentralized Insurance on Kaia          │
│                                                   │
│    Protect your crypto assets with on-chain      │
│         parametric insurance products             │
│                                                   │
│     [Buy Insurance]    [Provide Liquidity]       │
│                                                   │
└─────────────────────────────────────────────────┘
```

### Key Metrics Dashboard
```
┌──────────────┬──────────────┬──────────────────┐
│  Total TVL   │ Active Pools │ Total Premiums   │
│  $2.5M USDT  │     12       │   $125K USDT     │
└──────────────┴──────────────┴──────────────────┘
```

### Featured Insurance Products
```
┌─────────────────────────────────────────────────┐
│            Active Insurance Products             │
├─────────────────────────────────────────────────┤
│ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐│
│ │  BTC -10%   │ │  ETH -15%   │ │  KLAY -20%  ││
│ │  7 Days     │ │  14 Days    │ │  30 Days    ││
│ │  Premium: 5%│ │  Premium: 8%│ │  Premium:12%││
│ │  [Details]  │ │  [Details]  │ │  [Details]  ││
│ └─────────────┘ └─────────────┘ └─────────────┘│
└─────────────────────────────────────────────────┘
```

---

## 💼 Insurance Catalog Page

### Filter & Search Bar
```
┌─────────────────────────────────────────────────┐
│ Asset: [All ▼]  Trigger: [All ▼]  Duration: [▼] │
│                                    [Search 🔍]   │
└─────────────────────────────────────────────────┘
```

### Insurance Products Grid
```
┌─────────────────────────────────────────────────┐
│                Insurance Products                │
├─────────────────────────────────────────────────┤
│ ┌───────────────────────────────────────────┐   │
│ │ BTC Price Protection                       │   │
│ │ ┌─────────────────────────────────────┐   │   │
│ │ │ Tranche A: -5%  | Premium: 2%       │   │   │
│ │ │ Capacity: 100K USDT | Filled: 60%   │   │   │
│ │ │ Expiry: 7 Days  | [Buy Insurance]   │   │   │
│ │ └─────────────────────────────────────┘   │   │
│ │ ┌─────────────────────────────────────┐   │   │
│ │ │ Tranche B: -10% | Premium: 5%       │   │   │
│ │ │ Capacity: 50K USDT | Filled: 80%    │   │   │
│ │ │ Expiry: 7 Days  | [Buy Insurance]   │   │   │
│ │ └─────────────────────────────────────┘   │   │
│ │ ┌─────────────────────────────────────┐   │   │
│ │ │ Tranche C: -15% | Premium: 10%      │   │   │
│ │ │ Capacity: 25K USDT | Filled: 30%    │   │   │
│ │ │ Expiry: 7 Days  | [Buy Insurance]   │   │   │
│ │ └─────────────────────────────────────┘   │   │
│ └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

---

## 🛒 Insurance Purchase Flow

### Step 1: Product Selection
```
┌─────────────────────────────────────────────────┐
│           BTC -10% Price Protection              │
├─────────────────────────────────────────────────┤
│ Coverage Details:                                │
│ • Trigger: BTC price drops 10% from baseline     │
│ • Baseline: $45,000 (Round start price)          │
│ • Expiry: March 10, 2025 00:00 UTC              │
│ • Oracle: Kaia Price Feed + OO-lite             │
│                                                   │
│ Coverage Amount:                                 │
│ ┌─────────────────────────────────────────┐     │
│ │ Enter amount: [1000] USDT               │     │
│ │ Premium (5%): 50 USDT                   │     │
│ │ Total Payment: 50 USDT                  │     │
│ └─────────────────────────────────────────┘     │
│                                                   │
│ [← Back]              [Continue to Review →]     │
└─────────────────────────────────────────────────┘
```

### Step 2: Review & Confirm
```
┌─────────────────────────────────────────────────┐
│              Review Your Insurance               │
├─────────────────────────────────────────────────┤
│ Product: BTC -10% Protection                     │
│ Coverage: 1000 USDT                             │
│ Premium: 50 USDT                                │
│ Expiry: March 10, 2025                          │
│                                                   │
│ Payment Breakdown:                               │
│ • Insurance Premium: 47.5 USDT                  │
│ • Protocol Fee (5%): 2.5 USDT                   │
│ • Total: 50 USDT                                │
│                                                   │
│ ⚠️ Important:                                    │
│ • Payout is automatic upon trigger              │
│ • No manual claims needed                       │
│ • Non-refundable after purchase                 │
│                                                   │
│ □ I understand the terms and conditions         │
│                                                   │
│ [← Back]                    [Confirm Purchase]   │
└─────────────────────────────────────────────────┘
```

### Step 3: Transaction Status
```
┌─────────────────────────────────────────────────┐
│           Transaction in Progress                │
├─────────────────────────────────────────────────┤
│                                                   │
│              [Loading Animation]                 │
│                                                   │
│   Waiting for wallet confirmation...             │
│                                                   │
│   Transaction Hash:                              │
│   0x1234...5678                                 │
│                                                   │
│   [View on Kaiascope]                           │
└─────────────────────────────────────────────────┘
```

---

## 💰 Liquidity Provision Dashboard

### Liquidity Overview
```
┌─────────────────────────────────────────────────┐
│            Liquidity Provider Dashboard          │
├─────────────────────────────────────────────────┤
│ Your Statistics:                                 │
│ ┌──────────────┬──────────────┬───────────────┐ │
│ │ Total Deposit│ Active Pools │ Total Earnings │ │
│ │ 10,000 USDT  │      3       │   450 USDT    │ │
│ └──────────────┴──────────────┴───────────────┘ │
└─────────────────────────────────────────────────┘
```

### Available Pools
```
┌─────────────────────────────────────────────────┐
│              Available Tranche Pools             │
├─────────────────────────────────────────────────┤
│ ┌───────────────────────────────────────────┐   │
│ │ BTC -5% Tranche                           │   │
│ │ Expected Premium: 2% (200 USDT/10K)       │   │
│ │ Staking APY: 3.5%                         │   │
│ │ Risk Level: LOW                           │   │
│ │ Pool Size: 100,000 USDT                   │   │
│ │ Your Share: 0 USDT                        │   │
│ │ [Deposit USDT]                            │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ BTC -10% Tranche                          │   │
│ │ Expected Premium: 5% (500 USDT/10K)       │   │
│ │ Staking APY: 3.5%                         │   │
│ │ Risk Level: MEDIUM                        │   │
│ │ Pool Size: 50,000 USDT                    │   │
│ │ Your Share: 5,000 USDT                    │   │
│ │ [Add More] [Withdraw]                     │   │
│ └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

### Deposit Modal
```
┌─────────────────────────────────────────────────┐
│           Provide Liquidity to Pool              │
├─────────────────────────────────────────────────┤
│ Pool: BTC -10% Tranche                          │
│ Current Round: #12 (Ends in 2 days)             │
│                                                   │
│ Deposit Amount:                                  │
│ ┌─────────────────────────────────────────┐     │
│ │ [5000] USDT                             │     │
│ │ Balance: 15,000 USDT                    │     │
│ │ [25%] [50%] [75%] [MAX]                │     │
│ └─────────────────────────────────────────┘     │
│                                                   │
│ Expected Returns:                                │
│ • Premium Income: ~250 USDT (5%)                │
│ • Staking Rewards: ~175 USDT (3.5% APY)        │
│ • Total Expected: ~425 USDT                     │
│                                                   │
│ Risks:                                          │
│ • 10% chance of payout trigger                  │
│ • Funds locked until round end                  │
│                                                   │
│ [Cancel]                         [Confirm Deposit]│
└─────────────────────────────────────────────────┘
```

---

## 📊 Portfolio Management

### Portfolio Overview
```
┌─────────────────────────────────────────────────┐
│                 My Portfolio                     │
├─────────────────────────────────────────────────┤
│ Tabs: [Active Insurance] [LP Positions] [History]│
├─────────────────────────────────────────────────┤
│              Active Insurance Policies           │
│ ┌───────────────────────────────────────────┐   │
│ │ Policy #1234                              │   │
│ │ BTC -10% Protection                       │   │
│ │ Coverage: 1000 USDT                       │   │
│ │ Premium Paid: 50 USDT                     │   │
│ │ Status: ● Active                          │   │
│ │ Expires: 5 days                           │   │
│ │ Current BTC: $44,500 (-1.1%)              │   │
│ │ [View Details]                            │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ Policy #1235                              │   │
│ │ ETH -15% Protection                       │   │
│ │ Coverage: 500 USDT                        │   │
│ │ Premium Paid: 40 USDT                     │   │
│ │ Status: ✓ Claimable                      │   │
│ │ Payout: 500 USDT                          │   │
│ │ [Claim Now]                               │   │
│ └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

### LP Positions Tab
```
┌─────────────────────────────────────────────────┐
│              Liquidity Positions                 │
├─────────────────────────────────────────────────┤
│ ┌───────────────────────────────────────────┐   │
│ │ BTC -10% Tranche Pool                     │   │
│ │ Deposited: 5,000 USDT                     │   │
│ │ Current Value: 5,087 USDT                 │   │
│ │ Earned Premium: 250 USDT                  │   │
│ │ Staking Rewards: 87 USDT                  │   │
│ │ Round Status: Active (2 days left)        │   │
│ │ [Withdraw After Round]                    │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ ETH -5% Tranche Pool                      │   │
│ │ Deposited: 3,000 USDT                     │   │
│ │ Current Value: 3,045 USDT                 │   │
│ │ Earned Premium: 60 USDT                   │   │
│ │ Staking Rewards: 45 USDT                  │   │
│ │ Round Status: Settlement                  │   │
│ │ [Withdraw Available]                      │   │
│ └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

---

## 🔄 Insurance Lifecycle States

### Round Phases Display
```
┌─────────────────────────────────────────────────┐
│           Insurance Round Timeline               │
├─────────────────────────────────────────────────┤
│                                                   │
│  Phase 1      Phase 2     Phase 3     Phase 4   │
│  Funding   →  Matching  →  Active  →  Settlement │
│  (3 days)     (1 hour)     (7 days)   (1 day)   │
│                                                   │
│  [===●===========================================]│
│      ↑ Current Phase                             │
│                                                   │
│  Next Phase: Matching in 12 hours                │
└─────────────────────────────────────────────────┘
```

---

## 📱 Mobile Responsive Design

### Mobile Navigation
```
┌─────────────────┐
│ ☰  DIN   [Wallet]│
├─────────────────┤
│                 │
│  Total Portfolio│
│  12,450 USDT    │
│                 │
│ ┌─────────────┐ │
│ │ Quick Actions│ │
│ │ ┌─────────┐ │ │
│ │ │   Buy   │ │ │
│ │ │Insurance│ │ │
│ │ └─────────┘ │ │
│ │ ┌─────────┐ │ │
│ │ │ Provide │ │ │
│ │ │Liquidity│ │ │
│ │ └─────────┘ │ │
│ └─────────────┘ │
│                 │
│  Active Policies│
│  ┌────────────┐ │
│  │ BTC -10%   │ │
│  │ Active     │ │
│  └────────────┘ │
└─────────────────┘
```

---

## 🎨 Design System

### Color Palette
- **Primary**: #0EA5E9 (Kaia Blue)
- **Success**: #10B981 (Green)
- **Warning**: #F59E0B (Amber)
- **Danger**: #EF4444 (Red)
- **Background**: #0F172A (Dark)
- **Surface**: #1E293B (Card Background)
- **Text**: #F1F5F9 (Light)

### Typography
- **Headings**: Inter Bold
- **Body**: Inter Regular
- **Numbers**: Space Mono (Monospace)

### Components
- **Cards**: Rounded corners, subtle shadow
- **Buttons**: Primary (filled), Secondary (outlined)
- **Inputs**: Dark theme with border focus states
- **Modals**: Overlay with centered content
- **Toast**: Top-right notifications

---

## 🔔 Notification System

### Transaction Notifications
```
┌──────────────────────────┐
│ ✓ Success               │
│ Insurance purchased!     │
│ Policy #1236            │
│ [View Details]          │
└──────────────────────────┘
```

### Alert Notifications
```
┌──────────────────────────┐
│ ⚠️ Alert                │
│ Your policy expires     │
│ in 24 hours            │
│ [View Policy]           │
└──────────────────────────┘
```

---

## 🔐 Wallet Connection Flow

### Connect Wallet Modal
```
┌─────────────────────────────────────────────────┐
│            Connect Your Wallet                   │
├─────────────────────────────────────────────────┤
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ 🦊 MetaMask                               │   │
│ │     Recommended                           │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ 🔷 Kaikas                                 │   │
│ │     Kaia Native Wallet                    │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ ┌───────────────────────────────────────────┐   │
│ │ 🔗 WalletConnect                          │   │
│ │     Connect Mobile Wallet                 │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ By connecting, you agree to our Terms           │
└─────────────────────────────────────────────────┘
```

### Network Switch Prompt
```
┌─────────────────────────────────────────────────┐
│          Wrong Network Detected                  │
├─────────────────────────────────────────────────┤
│                                                   │
│   Please switch to Kaia Mainnet                  │
│   to use DIN Insurance                          │
│                                                   │
│   Current: Ethereum Mainnet                      │
│   Required: Kaia Mainnet (Chain ID: 8217)       │
│                                                   │
│          [Switch to Kaia Network]                │
│                                                   │
└─────────────────────────────────────────────────┘
```

---

## 📈 Analytics Dashboard (Admin View)

### Protocol Metrics
```
┌─────────────────────────────────────────────────┐
│              Protocol Analytics                  │
├─────────────────────────────────────────────────┤
│ ┌──────────────┬──────────────┬───────────────┐ │
│ │ Total TVL    │ Active Users │ Total Volume  │ │
│ │ $2.5M        │ 1,234        │ $125K/day     │ │
│ └──────────────┴──────────────┴───────────────┘ │
│                                                   │
│ Loss Ratio Chart:                                │
│ ┌───────────────────────────────────────────┐   │
│ │     📊 [Chart showing loss ratios]        │   │
│ └───────────────────────────────────────────┘   │
│                                                   │
│ Pool Performance:                                │
│ ┌───────────────────────────────────────────┐   │
│ │ Pool         | Premium | Payouts | Profit │   │
│ │ BTC -5%      | $50K    | $10K    | $40K   │   │
│ │ BTC -10%     | $25K    | $15K    | $10K   │   │
│ │ ETH -15%     | $15K    | $0      | $15K   │   │
│ └───────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

---

## 🔍 Oracle Status Display

### Oracle Information Panel
```
┌─────────────────────────────────────────────────┐
│              Oracle Information                  │
├─────────────────────────────────────────────────┤
│ Primary Oracle: Kaia Price Feed                  │
│ Status: ● Active                                 │
│ Last Update: 2 minutes ago                       │
│                                                   │
│ Fallback Oracle: OO-lite                        │
│ Status: ● Standby                                │
│                                                   │
│ Current Prices:                                  │
│ • BTC/USD: $45,234.56                           │
│ • ETH/USD: $2,456.78                            │
│ • KLAY/USD: $1.23                               │
│                                                   │
│ [View Oracle Documentation]                      │
└─────────────────────────────────────────────────┘
```

---

## 🚨 Error States

### Error Display
```
┌─────────────────────────────────────────────────┐
│              ⚠️ Error Occurred                   │
├─────────────────────────────────────────────────┤
│                                                   │
│   Transaction failed due to insufficient         │
│   USDT balance.                                 │
│                                                   │
│   Required: 1,000 USDT                          │
│   Available: 500 USDT                           │
│                                                   │
│   [Go to Swap]          [Cancel]                │
└─────────────────────────────────────────────────┘
```

---

## 📋 Implementation Notes

### Technical Requirements
1. **Web3 Integration**: @kaiachain/ethers-ext for Kaia blockchain
2. **Smart Contracts**: Insurance, Treasury, TranchePool contracts
3. **State Management**: React Context for Web3 connection
4. **UI Framework**: Next.js 15 with Tailwind CSS
5. **Wallet Support**: MetaMask, Kaikas, WalletConnect

### Key User Flows
1. **Insurance Purchase**: Browse → Select → Review → Confirm → Receipt
2. **Liquidity Provision**: Select Pool → Deposit → Monitor → Withdraw
3. **Claim Process**: Automatic trigger → Oracle verification → Auto-payout
4. **Portfolio Management**: View positions → Track performance → Withdraw

### Responsive Breakpoints
- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

### Accessibility
- WCAG 2.1 AA compliance
- Keyboard navigation support
- Screen reader compatibility
- High contrast mode support

---

*This wireframe document serves as the foundation for implementing the DIN insurance platform UI. All flows are designed to prioritize user experience, transparency, and trust in the decentralized insurance ecosystem.*