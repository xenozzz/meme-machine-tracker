# 🧠 Meme Machine V5.0+ | Public Tracker

> **"The only economy where losing money is a feature."**

Welcome to the official public repository for **Meme Machine**. Since the game code is private (to prevent insider trading and source code theft), this repository serves as our **Issue Tracker**, **Suggestion Box**, and **Game Manual**.

### 🔗 https://slots.xenoz.online

---

## 🚨 PATCH NOTES V5.0: THE BRAINROT UPDATE

# Changelog - Meme Machine

## [Latest Session - December 19, 2025]

### 🎰 Gambling Mechanics Enhancements
*   **Social Credit Penalties:** Implemented a -5 social credit deduction for every gambling action across Roulette, Coinflip, and Plinko to encourage active work participation.
*   **Stats Tracking:** Ensured all gambling API routes (`/api/roulette`, `/api/coinflip`, `/api/coinflip-pvp`, `/api/plinko`) correctly update `total_wagered` and `total_won_gambling` statistics for accurate leaderboard and profile displays.

### 🛡️ Item & Security Refinements
*   **Cyber Firewall & Espionage:** Reviewed and validated the full logic for "Cybersecurity" (firewall) and "Espionage" (hacker) items. 
    *   Firewall now correctly blocks hacks and expires after 12 hours.
    *   Espionage allows hacking random rich players with a 4-hour cooldown.
    *   Integrated both features seamlessly into the `WallStreetModal` and `StoreModal`.

### 🎨 Visual & UI Corrections
*   **Emoji Fixes:** Corrected broken/corrupted emojis for the "Delivery Knight" animation and lootbox rewards in chat and profile views.
*   **Brainrot Player 2.0:** Verified that the YouTube embed (Brainrot Player) displays correctly across all game tabs (Slots, Roulette, Coin, Plinko), ensuring maximum engagement during the grind.

### ⚙️ Admin & Reset Features
*   **Plinko Reset System:** 
    *   Updated database schema with `is_plinko_reset_pending`.
    *   Created `/api/admin/trigger-plinko-reset` for administrative control.
    *   Implemented a narrative-driven reset in `/api/plinko/route.ts` that resets player scores/stats when triggered by an admin.

### 🛠️ TypeScript & Build Stability
*   **Bug Squashing:** Addressed numerous TypeScript errors in `app/page.tsx` and related components (`CoinGame.tsx`, `RouletteGame.tsx`, etc.).
*   **Export/Import Fixes:** Standardized type exports (`UserProfile`, `CoinResult`, `RouletteResult`) and corrected relative import paths.
*   **Backend Stability:** Resolved critical backend errors, including duplicate variable declarations in `/api/plinko` and incorrect `Promise.all` destructuring in `/api/coinflip-pvp`.

### ⚔️ PvP & Gambling
* **PvP Deathrolls:** Challenge players to 1v1 coin-flip duels. Includes invite system (accept/decline), expiration timers, and history logs.
    * *Note: Losing a massive wager triggers a "Humiliation" message in the global feed.*
* **Roulette:** New 8-bit table.
    * **Red/Black:** 2x Payout.
    * **Green:** 10x Payout (The Rug Pull).
    * **The Glitch:** 1% chance a win flips to a loss due to "Server Error."
* **Slots:** $10 spin ($15 if low credit). Jackpots up to **$25,000**.

### 📉 Economy & QoL
* **Bank Rework:** Cap set to **$85,000**. Interest is now **2% Hourly** (paid to wallet). Withdrawal fee: 2%.
* **Market QoL:** Added `Buy 1`, `10`, `MAX` and `Sell 1`, `10`, `ALL` buttons for Fish/Stocks.
* **Espionage:** Raid other players ($1,000 cost) to steal 5-10% of their wallet.
* **Lootbox 2.0:** 5m Cooldown. Drops: Cash, Wage Multipliers, Rare PFPs, Emotes, Junk, and the **Mythic Printer**.

### 📺 Media & Social
* **Brainrot Player:** Added **UNMUTE** button, Split View (Subway Surfers + Content), and **Custom YouTube URL** support.
* **Social:** Global Chat with auto-censor (don't get banned). Toast alerts for big plays. Leaderboard tracks Net Worth.

---

## 📖 GAME MANUAL (The Rules)

### 1. Work & Career
Click to earn. Risks scale with reward.
* **Intern:** Earns $1 + Coffee. (Risk: 0%).
* **Manager:** Earns $5 + Coffee. (Risk: **1%** chance of getting fired / -$100). *Req: 500 Credit.*
* **CEO:** Earns $50 + 2xCoffee. (Risk: **5%** chance of SEC Raid / -20% Wallet). *Req: 1500 Credit.*
* *Coffee:* Each level adds +$1 to base wage (Uncapped).

### 2. Taxes & Social Credit
The government takes its cut. Taxes apply to **Wallet Only**.
* **<$1k:** 0% Tax
* **$1k - $5k:** 20% Tax
* **>$5k:** 50% Tax

**Social Credit System:**
* **Gain:** Working (+5), Snitching.
* **Lose:** Gambling (-5), Chat Violations.
* **Penalty:** If Credit < 500, you pay **+10% Tax** and Slots cost **$15**.

### 3. Banking & Assets
* **The Bank:** Safe from Hackers. Tax-Free.
    * **Cap:** $85,000.
    * **Interest:** 2% per hour (must hold funds to earn).
    * **Fee:** 2% on withdrawals.
* **Stock Market:** Rare Fish prices change every minute. High volatility.

### 4. Winning Numbers (Slots)
* `067` - **JACKPOT** ($25,000)
* `777` - **LUCKY** ($7,777)
* `666` - **DEVIL** ($6,666)
* `420` - **BLAZE** ($4,200)
* `123` - **STRAIGHT** ($1,230)
* `007` - **BOND** ($700)
* `069` - **NICE** ($690)
* `XXX` - **TRIPLES** ($500)

---

## 🛠️ How to Contribute

### 🐛 Found a Bug?
Did the Market crash? Did the Roulette wheel spin forever?
* Check the [Issues Tab](https://github.com/YOUR_USERNAME/REPO_NAME/issues) first.
* **[Open a Bug Report](https://github.com/YOUR_USERNAME/REPO_NAME/issues/new)**.
* *Please include screenshots and your device (Mobile vs Desktop).*

### 💡 Feature Requests
We are looking for toxic mechanics and fun gambling concepts.
* **[Submit a Feature Request](https://github.com/YOUR_USERNAME/REPO_NAME/issues/new)**.

---

## ⚠️ Disclaimer
**Do not post sensitive information.**
When uploading screenshots of bugs, please ensure you are not sharing personal passwords or sensitive data. This is a public repository.

*Managed by the Meme Machine Dev Team. Social Credit +10 for starring this repo.*
