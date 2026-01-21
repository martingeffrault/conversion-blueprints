# Crypto & Web3 Website Patterns

> **Primary challenge**: Building trust in a low-trust environment
> **Key principle**: "In an industry where scams are everywhere, UX = trust"
> **User focus**: Bridge Web2 familiarity with Web3 complexity
> **Design ethos**: Transparency, clarity, security at every touchpoint
> **Sources**: Coinbound, Digital Silk, Arounda Agency, Web3 Design Studies

---

## The Trust Imperative

### Why Trust Matters More in Crypto

The crypto/Web3 space faces unique challenges:

| Challenge | Implication |
|-----------|-------------|
| High-profile scams/rugs | Default user skepticism |
| Technical complexity | Confusion = abandonment |
| Financial risk | Users need constant reassurance |
| Irreversible transactions | Clear confirmations essential |
| Self-custody | User responsibility requires guidance |

> "In an industry where scams are everywhere, UX = trust. Great interfaces feel secure: clear wallet signings, predictable actions, and warnings before risk."
>
> *Source: Coinbound*

### Trust Building Framework

```
┌─────────────────────────────────────────────────────────────────┐
│                    Web3 Trust Stack                             │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  1. VISUAL TRUST                                                │
│     ├── Professional design (not rushed)                        │
│     ├── Security badges prominent                               │
│     └── Recognizable partner logos                              │
│                                                                 │
│  2. TECHNICAL TRUST                                             │
│     ├── Smart contract audits displayed                         │
│     ├── Code transparency page                                  │
│     └── Bug bounty program                                      │
│                                                                 │
│  3. TEAM TRUST                                                  │
│     ├── Doxxed team members                                     │
│     ├── LinkedIn/Twitter verification                           │
│     └── Advisory board credibility                              │
│                                                                 │
│  4. COMMUNITY TRUST                                             │
│     ├── Active Discord/Telegram                                 │
│     ├── Transparent governance                                  │
│     └── Regular updates/AMAs                                    │
│                                                                 │
│  5. TRANSACTION TRUST                                           │
│     ├── Clear transaction previews                              │
│     ├── Gas fee warnings                                        │
│     └── Confirmation screens                                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Homepage Patterns

### Hero Section

Web3 heroes balance innovation with accessibility:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]              [Products ▼] [Docs] [Governance]  [Launch]│
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │       The Future of Decentralized Finance              │   │
│  │                                                         │   │
│  │   Trade, earn, and own your assets with complete       │   │
│  │   control. No middlemen. No permissions needed.        │   │
│  │                                                         │   │
│  │   [Launch App]  [Read Docs]                            │   │
│  │                                                         │   │
│  │   ✓ Audited by Certik   ✓ $2B+ TVL   ✓ 500K+ Users    │   │
│  │                                                         │   │
│  │   [3D animated visualization / product preview]        │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Essential elements:**
- Clear value proposition (benefits, not tech jargon)
- Primary CTA: Launch App / Connect Wallet
- Secondary CTA: Documentation / Learn More
- Trust signals above fold (audits, TVL, user count)
- Visual that shows product (not abstract art)

### Visual Design Trends

> "Cosmos is a perfect example of Web3 website design trends: colorful gradients, 3D elements, and futuristic space themes."

| Element | Common Treatments |
|---------|-------------------|
| Colors | Aqua, turquoise, navy, orchid, neon accents |
| Backgrounds | Dark mode default, gradient meshes |
| 3D | Floating elements, depth effects |
| Animation | Subtle motion, parallax, particle effects |
| Typography | Clean sans-serif, sometimes monospace |
| Layout | Grid-based, asymmetric sections |

### Trust Signals Section

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                    Security First                               │
│                                                                 │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │
│  │               │ │               │ │               │         │
│  │  [Certik]     │ │  [Hacken]     │ │  [SlowMist]   │         │
│  │   Audited     │ │   Verified    │ │   Reviewed    │         │
│  │               │ │               │ │               │         │
│  │ [View Report] │ │ [View Report] │ │ [View Report] │         │
│  │               │ │               │ │               │         │
│  └───────────────┘ └───────────────┘ └───────────────┘         │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  🔒 All smart contracts are open source and verified    │   │
│  │  🐛 $500K Bug Bounty Program active on Immunefi        │   │
│  │  📊 Real-time protocol statistics on DefiLlama         │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│            [View Code on GitHub]  [Security Docs]              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Stats Dashboard

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                Protocol Statistics                              │
│                                                                 │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │
│  │               │ │               │ │               │         │
│  │   $2.4B       │ │   523,847     │ │   $12.3M      │         │
│  │               │ │               │ │               │         │
│  │ Total Value   │ │    Total      │ │  24h Volume   │         │
│  │   Locked      │ │    Users      │ │               │         │
│  │               │ │               │ │               │         │
│  │  ↑ 12% 24h    │ │  ↑ 2.4% 7d    │ │  ↓ 3% 24h    │         │
│  │               │ │               │ │               │         │
│  └───────────────┘ └───────────────┘ └───────────────┘         │
│                                                                 │
│         [View on DefiLlama]  [Analytics Dashboard]             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Best practices:**
- Link to independent verification (DefiLlama, DappRadar)
- Show real-time or recent data
- Include trends (up/down indicators)
- Don't fake numbers

---

## Wallet Connection UX

### The Gateway to Web3

> "Wallet connection is the gateway to Web3 functionality. The design must make this process clear, secure, and user-friendly."

### Connection Flow

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│               Connect Your Wallet                               │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  ┌─────────────────────────────────────────────┐       │   │
│  │  │ [MetaMask icon]                             │       │   │
│  │  │  MetaMask                                   │       │   │
│  │  │  Connect using browser wallet               │       │   │
│  │  └─────────────────────────────────────────────┘       │   │
│  │                                                         │   │
│  │  ┌─────────────────────────────────────────────┐       │   │
│  │  │ [WalletConnect icon]                        │       │   │
│  │  │  WalletConnect                              │       │   │
│  │  │  Connect using mobile wallet                │       │   │
│  │  └─────────────────────────────────────────────┘       │   │
│  │                                                         │   │
│  │  ┌─────────────────────────────────────────────┐       │   │
│  │  │ [Coinbase icon]                             │       │   │
│  │  │  Coinbase Wallet                            │       │   │
│  │  │  Connect using Coinbase                     │       │   │
│  │  └─────────────────────────────────────────────┘       │   │
│  │                                                         │   │
│  │  ──────────────────────────────────────────────        │   │
│  │                                                         │   │
│  │  New to crypto? [Create a wallet →]                    │   │
│  │                                                         │   │
│  │  🔒 We never ask for your seed phrase                  │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Connection Best Practices

| Element | Implementation |
|---------|----------------|
| Multiple wallets | MetaMask, WalletConnect, Coinbase minimum |
| One-click connect | Single action, no unnecessary steps |
| Mobile support | WalletConnect essential for mobile |
| New user path | "Don't have a wallet?" guide |
| Security warning | "We never ask for seed phrase" |
| Clear prompts | Explain what happens after connection |

### Post-Connection State

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]  [Products ▼]  [Docs]     [0x1234...5678 ▼] [⚙️]       │
│                                    └── Connected wallet         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘

Wallet dropdown:
┌─────────────────────────────┐
│                             │
│  0x1234...5678   [📋]      │
│  Ethereum Mainnet          │
│                             │
│  Balance: 2.45 ETH          │
│  ≈ $6,125.00               │
│                             │
│  ─────────────────────────  │
│                             │
│  [Switch Network]          │
│  [View on Etherscan]       │
│  [Disconnect]              │
│                             │
└─────────────────────────────┘
```

---

## Transaction UX

### Pre-Transaction Preview

> "Before executing a transaction, give users a clear preview: Show token amounts, fees, estimated total, and recipient address."

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│               Confirm Transaction                               │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  Swap                                                   │   │
│  │                                                         │   │
│  │  You pay:          1.0 ETH                              │   │
│  │  You receive:      ~2,450 USDC                          │   │
│  │                                                         │   │
│  │  ─────────────────────────────────────────────────     │   │
│  │                                                         │   │
│  │  Rate:             1 ETH = 2,450 USDC                   │   │
│  │  Price Impact:     < 0.01%                              │   │
│  │  Slippage:         0.5%                                 │   │
│  │                                                         │   │
│  │  ─────────────────────────────────────────────────     │   │
│  │                                                         │   │
│  │  Network Fee:      ~$3.24 (estimated)                   │   │
│  │                    ⚠️ Fees are higher than usual        │   │
│  │                                                         │   │
│  │  ─────────────────────────────────────────────────     │   │
│  │                                                         │   │
│  │  To address:       0xABCD...1234                        │   │
│  │                    ✓ Verified contract                  │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  [Cancel]                     [Confirm in Wallet]              │
│                                                                 │
│  ⚠️ Review transaction carefully before signing                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Transaction States

```
Pending:
┌─────────────────────────────────────────┐
│                                         │
│  ⏳ Transaction Pending                 │
│                                         │
│  Waiting for confirmation...            │
│  This may take 1-5 minutes              │
│                                         │
│  [View on Etherscan]                    │
│                                         │
└─────────────────────────────────────────┘

Success:
┌─────────────────────────────────────────┐
│                                         │
│  ✅ Transaction Successful              │
│                                         │
│  You received 2,450 USDC                │
│                                         │
│  [View on Etherscan]  [Done]           │
│                                         │
└─────────────────────────────────────────┘

Failed:
┌─────────────────────────────────────────┐
│                                         │
│  ❌ Transaction Failed                  │
│                                         │
│  Reason: Insufficient gas               │
│                                         │
│  Your funds are safe. No tokens         │
│  were sent.                             │
│                                         │
│  [Try Again]  [Get Help]               │
│                                         │
└─────────────────────────────────────────┘
```

### Warning Systems

| Warning Type | When to Show |
|--------------|--------------|
| High gas fees | Fees significantly above average |
| High slippage | > 1% slippage risk |
| Unknown contract | First interaction, not verified |
| Large transaction | Above user's usual amount |
| Approval request | Token approval (explain unlimited) |

---

## Progressive Disclosure

### Bridging Web2 to Web3

> "Don't overwhelm users with blockchain jargon up front. Lead them gradually."

### Language Progression

| Beginner-Friendly | Intermediate | Advanced |
|-------------------|--------------|----------|
| Send | Transfer | Execute |
| Receive | Deposit | Mint |
| Balance | Holdings | Portfolio |
| Wallet | Address | EOA |
| Fee | Gas | Gwei |
| Trade | Swap | DEX |
| Earnings | Yield | APY |

### Tooltip/Learn More Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Estimated Gas Fee: $4.25 [ℹ️]                                  │
│                                                                 │
│  ┌──────────────────────────────────────────────────┐          │
│  │                                                  │          │
│  │  💡 What are gas fees?                          │          │
│  │                                                  │          │
│  │  Gas fees are payments made to process your     │          │
│  │  transaction on the blockchain. They go to      │          │
│  │  validators, not to us.                         │          │
│  │                                                  │          │
│  │  Fees change based on network congestion.       │          │
│  │                                                  │          │
│  │  [Learn more about gas →]                       │          │
│  │                                                  │          │
│  └──────────────────────────────────────────────────┘          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Onboarding for New Users

### Guided Experience

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Welcome to [Protocol]! 🎉                                      │
│                                                                 │
│  Let's get you started in 3 simple steps:                      │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  Step 1 of 3                                           │   │
│  │  ●───○───○                                             │   │
│  │                                                         │   │
│  │  Connect Your Wallet                                   │   │
│  │                                                         │   │
│  │  Your wallet is like your bank account for crypto.     │   │
│  │  It stores your assets and lets you interact with      │   │
│  │  decentralized apps.                                   │   │
│  │                                                         │   │
│  │  [I have a wallet]  [Create new wallet]               │   │
│  │                                                         │   │
│  │  ─────────────────────────────────────────────────    │   │
│  │                                                         │   │
│  │  📺 Watch: "What is a crypto wallet?" (2 min)         │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  [Skip tutorial]                                               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Education Resources

- Inline tooltips for all technical terms
- Video tutorials for key actions
- FAQ/Help documentation
- Live chat/Discord support
- Test transactions with small amounts

---

## Team & Transparency

### Team Section

> "Crypto projects live and die by their community. Transparent teams build trust."

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                    Meet the Team                                │
│                                                                 │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │
│  │               │ │               │ │               │         │
│  │   [Photo]     │ │   [Photo]     │ │   [Photo]     │         │
│  │               │ │               │ │               │         │
│  │  Sarah Chen   │ │  Mike Johnson │ │  Dr. Li Wei   │         │
│  │  CEO/Founder  │ │  CTO          │ │  Head of      │         │
│  │               │ │               │ │  Research     │         │
│  │ Ex-Coinbase   │ │ Ex-Google     │ │ Stanford PhD  │         │
│  │               │ │               │ │               │         │
│  │ [X] [in]      │ │ [X] [GH]      │ │ [X] [in]      │         │
│  │               │ │               │ │               │         │
│  └───────────────┘ └───────────────┘ └───────────────┘         │
│                                                                 │
│  ✓ Team is fully doxxed (verified identities)                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Transparency Page

> "Give users permanent access to a Code Transparency page, similar to a Privacy Policy page."

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                    Transparency                                 │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  📝 Smart Contracts                                     │   │
│  │     All contracts verified on Etherscan                 │   │
│  │     [View contracts →]                                  │   │
│  │                                                         │   │
│  │  🔍 Security Audits                                     │   │
│  │     Certik (Mar 2025), Trail of Bits (Jan 2025)        │   │
│  │     [View audit reports →]                              │   │
│  │                                                         │   │
│  │  💻 Open Source                                         │   │
│  │     Full codebase on GitHub                            │   │
│  │     [View repository →]                                 │   │
│  │                                                         │   │
│  │  🐛 Bug Bounty                                          │   │
│  │     Up to $500K on Immunefi                            │   │
│  │     [Report vulnerability →]                            │   │
│  │                                                         │   │
│  │  📊 Treasury                                            │   │
│  │     Multi-sig wallet, viewable on-chain                │   │
│  │     [View treasury →]                                   │   │
│  │                                                         │   │
│  │  🗳️ Governance                                          │   │
│  │     Proposals and voting on Snapshot                   │   │
│  │     [Participate →]                                     │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Community Integration

### Social Links

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                    Join Our Community                           │
│                                                                 │
│  ┌───────────────┐ ┌───────────────┐ ┌───────────────┐         │
│  │               │ │               │ │               │         │
│  │  [Discord]    │ │  [Twitter]    │ │  [Telegram]   │         │
│  │               │ │               │ │               │         │
│  │   Discord     │ │   Twitter     │ │   Telegram    │         │
│  │   50K+        │ │   125K        │ │   30K         │         │
│  │   members     │ │   followers   │ │   members     │         │
│  │               │ │               │ │               │         │
│  │   [Join]      │ │   [Follow]    │ │   [Join]      │         │
│  │               │ │               │ │               │         │
│  └───────────────┘ └───────────────┘ └───────────────┘         │
│                                                                 │
│  📅 Weekly AMAs every Thursday at 4pm UTC                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Mobile Optimization

### Mobile-First Considerations

| Element | Mobile Treatment |
|---------|-----------------|
| Wallet connection | WalletConnect primary, deep links |
| Transaction preview | Full-screen modal, large buttons |
| Address display | Truncated with copy button |
| Network selector | Bottom sheet, not dropdown |
| Charts/data | Simplified, scrollable |

### Mobile Wallet Connection

```
┌─────────────────────────────┐
│                             │
│  Connect Wallet             │
│                             │
│  ┌─────────────────────┐   │
│  │                     │   │
│  │  [MetaMask]         │   │
│  │  Open in app        │   │
│  │                     │   │
│  └─────────────────────┘   │
│                             │
│  ┌─────────────────────┐   │
│  │                     │   │
│  │  [Trust Wallet]     │   │
│  │  Open in app        │   │
│  │                     │   │
│  └─────────────────────┘   │
│                             │
│  ┌─────────────────────┐   │
│  │                     │   │
│  │  [WalletConnect]    │   │
│  │  Scan QR code       │   │
│  │                     │   │
│  └─────────────────────┘   │
│                             │
│  [Cancel]                   │
│                             │
└─────────────────────────────┘
```

---

## Emerging Trends 2025

### AI Integration

> "AI in blockchain UI is becoming a prominent feature. Biometric logins eliminate password needs."

- AI-powered transaction explanations
- Natural language commands
- Predictive gas estimation
- Anomaly detection warnings

### Data Visualization

> "Instead of boring tables or static charts, data will be presented right where you need it in easy-to-understand formats."

- Real-time protocol dashboards
- Interactive portfolio views
- Visual transaction history
- Animated yield displays

---

## Common Mistakes

### ❌ Technical Jargon Overload

Lead with benefits, explain tech later.

### ❌ Missing Audit Information

No audit = no trust for serious users.

### ❌ Complicated Wallet Connection

One-click with multiple options.

### ❌ No Transaction Preview

Users need to see what they're signing.

### ❌ Anonymous Team

Doxxed teams build trust.

### ❌ No Mobile Support

Many users are mobile-first.

### ❌ Fake or Inflated Stats

Independent verification or nothing.

---

## Web3 Website Checklist

### Trust & Security

- [ ] Smart contract audits displayed
- [ ] Links to verified contracts
- [ ] Bug bounty program
- [ ] Team information (doxxed)
- [ ] Open source code
- [ ] Independent stats verification

### User Experience

- [ ] Clear value proposition (not jargon)
- [ ] Multiple wallet options
- [ ] One-click connection
- [ ] Transaction preview screens
- [ ] Clear error messages
- [ ] Education/tooltips

### Community

- [ ] Discord/Telegram links
- [ ] Twitter presence
- [ ] Governance access
- [ ] Regular updates/roadmap

### Technical

- [ ] Mobile responsive
- [ ] Fast load times
- [ ] Real-time data where appropriate
- [ ] Fallback states (wallet disconnected, etc.)

---

## Sources

- [Coinbound - Web3 UX Design Patterns That Build Trust](https://coinbound.io/web3-ux-design-patterns-that-build-trust/)
- [Digital Silk - Crypto Web Design Tips & Best Practices](https://www.digitalsilk.com/digital-trends/crypto-web-design-tips-best-practices/)
- [Arounda Agency - Web3 Design Principles](https://arounda.agency/blog/web3-design-principles-9-main-points)
- [Merge Rocks - Web3 Design Trends 2025](https://merge.rocks/blog/10-web3-design-trends-for-2025)
- [WebStacks - Web 3.0 Website Design Examples](https://www.webstacks.com/blog/web-3-design)
- [Creatif Agency - Crypto Web Design Guide](https://creatif.agency/crypto-web-design-a-beginners-guide-to-designing-for-web3/)
