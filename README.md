# GX Youth 🛡️
### The Ultimate Financial Council for the Next Generation

**GX Youth** is an immersive, multi-agent financial command center designed for the youth of Malaysia. Built on top of the GXBank ecosystem, it transforms the traditional banking experience into a cinematic, AI-driven journey towards financial resilience.

---

## 🌟 Overview

GX Youth isn't just a wallet; it's a **Council of Experts** in your pocket. By combining real-time financial tracking with a collaborative AI council, we help users navigate impulse spending, automate growth, and build a "Debt Shield" that protects their future. 

The app features **Kebo**, a reactive financial mascot that lives on your dashboard, reflecting your financial health through dynamic animations and real-time feedback.

---

## 🚀 Core Features

### 1. The Multi-Agent Council (AI Coach)
A collaborative AI engine where four specialized agents work together to provide coordinated guidance:
- **🛡️ Debt Shield**: Analyzes the impact of purchases before you make them, protecting you from "invisible" debt.
- **🎯 Savings Sentinel**: Dynamically adjusts your saving goals based on cashflow and helps initialize "Growth Pockets."
- **📈 Growth Guru**: Scans the market (ASB, Stocks, Crypto) to suggest the best opportunities for your current resilience level.
- **🧠 Finance Strategist**: The orchestrator that handles budget allocation and finds marketplace alternatives for risky purchases.

### 2. Resilience Score
A holistic, real-time health metric (0-100%) calculated from:
- **Cashflow Safety**: Your ability to stay within daily spending quotas.
- **Savings Progress**: Your trajectory towards long-term and emergency goals.
- **Debt Health**: Your exposure to high-risk commitments.

### 3. Smart Bills & Commitments
- **Auto-Protection**: Automatically "locks" money needed for upcoming bills, ensuring you never overspend your rent or tuition money.
- **Needs-Setup Detection**: Identifies commitments that lack account details and prompts for completion.

### 4. Kebo: Your Reactive Companion
- A custom-built 2D sprite mascot with **10+ dynamic animations** (Idle, Think, Happy, Excited, Sad, Wave, etc.).
- Kebo reacts to your financial actions: celebrate a saving milestone with a dance, or see Kebo "think" while the AI council prepares your budget.

---

## 🏗️ Architecture

### Tech Stack
- **Framework**: [Next.js 16](https://nextjs.org/) (App Router, Turbopack)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) with a Purple Glassmorphic Design System.
- **State Management**: [Zustand](https://zustand-demo.pmnd.rs/) with `persist` middleware for robust, offline-ready local storage.
- **Animations**: [Framer Motion](https://www.framer.com/motion/) for UI transitions and custom Canvas/CSS spritesheet logic for mascot rendering.
- **Data Visualization**: [Recharts](https://recharts.org/) for financial trend analysis.

### System Logic
- **Hydration Wrapper**: A custom hook architecture ensures that the persisted financial state is correctly hydrated before the UI renders, preventing hydration mismatches.
- **Multi-Agent Dispatcher**: A message-based system in the `Coach` component that triggers specialized agent responses based on NLP keywords.

---

## 📱 Use Cases

### Scenario A: The Impulse Buy
**User**: "Should I buy this RM 3,000 iPhone?"
1. **Debt Shield** simulates the impact: "This is 40% of your balance. Not recommended."
2. **Finance Strategist** steps in: "I've found pre-owned alternatives on Shopee and Lazada for RM 899 that fit your budget."

### Scenario B: Automated Growth
1. **Savings Sentinel** notices a balance surplus.
2. **Growth Guru** suggests: "Your Emergency Fund is full. Move RM 200 to your ASB Growth Pocket for 4.2% p.a. returns?"
3. **Kebo** celebrates with an `excited` animation upon confirmation.

---

## 🛠️ Installation & Development

```bash
# Install dependencies
npm install

# Run development server (Port 2222)
npm run dev

# Build for production
npm run build
```

---

## 🏆 Credits
Built by **Team SelaDevs** for the **UTMxHackathon 2026**. 
Powered by **GXBank**, organized by **PERSAKA UTM**, and sponsored by **RunCloud**.
