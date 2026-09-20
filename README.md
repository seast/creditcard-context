# 💳 CreditCard Context (`credit_cards.md` Template)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-blue.svg)](https://daringfireball.net/projects/markdown/)

> AI-Friendly Credit Card & Rewards Optimization Context for LLM Tools (Muse, Cursor, ChatGPT, Claude, etc.)

**CreditCard Context** is a structured Markdown workspace template designed to bring intelligent credit card management and reward optimization to your favorite AI tools. 

By loading your custom `credit_cards.md` file into tools like **Muse**—which natively supports custom `.md` context files—or **Cursor**, your AI workspace assistant can instantly calculate valuation-adjusted return rates, track quarterly 5% spend caps, warn you about expiring annual credits, and recommend the best card for any purchase.

---

## ✨ Key Features

- **🔒 Privacy First**: Stores card names, tiers, categories, and quarterly spend progress—**never full card numbers, expiration dates, or CVVs**.
- **🧠 Native Muse Workspace Support**: Works out of the box with Muse's custom Markdown context feature, allowing seamless background context integration without pasting text repeatedly.
- **🌐 Foreign Transaction Fee (FTF) Awareness**: Explicitly separates cards into **No FTF** (for international travel) and **Domestic Only** categories to prevent unexpected conversion fees abroad.
- **📈 Spend Cap & Perk Tracking**: Log quarter-to-date spending progress (e.g., Chase Freedom / Discover $1,500 quarterly limits, BOA $2,500 caps) and statement credit resets.
- **🤖 Context-Aware AI Recommendations**: Query your AI assistant directly to evaluate complex multi-tier strategies (e.g., *"What is my Q4 dining strategy once I hit my BOA spend limit?"*).

---

## 🚀 Quick Start

### 1. Clone or Copy Template
Copy `credit_cards.sample.md` into your local workspace or project directory as `credit_cards.md`:

```bash
cp credit_cards.sample.md credit_cards.md
```

> **Important**: Add `credit_cards.md` to your `.gitignore` to prevent committing personal notes or custom progress details to public repositories.

### 2. Customize Your Portfolio
Fill in your credit card portfolio following the template format:
- Group cards by **No Foreign Transaction Fee** vs. **Has Foreign Transaction Fee**.
- Record multipliers, annual fees, statement credit reset dates, and active free trial expirations.
- Perform a quick monthly or quarterly check-in to update 5% rotating category status and spend cap progress.

### 3. Load into Your AI Workspace
- **Muse**: Place `credit_cards.md` in your workspace or specify it as a custom context Markdown file in your Muse settings.
- **Cursor / VS Code**: Reference `@credit_cards.md` directly inside chat prompts.
- **ChatGPT / Claude**: Attach `credit_cards.md` or paste its text into your Project Knowledge / Custom Instructions.

---

## 💬 Example Context Dialog

Here is an example of how an AI workspace assistant (e.g., Muse, Cursor, ChatGPT) uses `credit_cards.md` context to guide spending decisions during international travel:

**User:**
> "I am currently in Paris. I need to rent a car, pay for a $150 bistro dinner, and book a flight back. Among my cards—**Chase Sapphire Reserve (CSR)**, **Chase Sapphire Preferred (CSP)**, **Amex Gold**, and **BOA Customized Cash (123)**—which card should I use for each?"

**AI Assistant:**

Based on your loaded `credit_cards.md` profile and location context (Paris, France):

### 1. 🚗 Renting a Car
* **Recommended Card:** **Chase Sapphire Reserve (CSR)**
* **Effective Return:** **3x UR Points** (~4.5% value) + Primary CDW
* **Key Reason:** CSR provides **Primary Auto Rental Collision Damage Waiver (CDW)** coverage globally. You can safely decline the rental company's expensive CDW coverage. 
* *Avoid:* **BOA 123** due to a **3% Foreign Transaction Fee (FTF)**, and **Amex Gold** because its rental coverage is secondary only.

### 2. 🍽️ Paying for Bistro Dinner
* **Recommended Card:** **Chase Sapphire Reserve (CSR)** (or **CSP**)
* **Effective Return:** **3x UR Points** (~4.5% value)
* **Key Reason:** CSR earns 3x points on worldwide dining with **$0 Foreign Transaction Fees**. 
* *Note on Amex Gold:* While Amex Gold earns 4x on worldwide dining, Visa/Mastercard acceptance in European bistros is significantly higher than Amex, making CSR the most reliable primary card.

### 3. ✈️ Booking an Airline Ticket: Amex Gold vs. CSR / CSP Insurance Comparison
* **Primary Recommendation (Max Value):** **Amex Gold**
  * **Earning Rate:** **5x MR Points** (~7.5% return value) on flights booked directly or via Amex Travel.
  * **Insurance:** Includes **12-Hour Trip Delay Reimbursement** (up to $500 per trip) and Trip Cancellation/Interruption protection.
* **Alternative Option (Max Insurance Protection):** **Chase Sapphire Reserve (CSR)**
  * **Earning Rate:** **3x UR Points** (~4.5% return value).
  * **Insurance Advantage:** Superior **6-Hour Trip Delay Coverage** (kicks in twice as fast as Amex or CSP, up to $500 per ticket for meals/lodging) plus primary baggage delay reimbursement ($100/day after 6 hours).
* **Backup Option:** **Chase Sapphire Preferred (CSP)**
  * **Earning Rate:** **2x UR Points** (~3.0% return value).
  * **Insurance:** Shares standard **12-Hour Trip Delay Coverage** ($500 limit) and $10,000 Trip Cancellation protection with Amex Gold.

* **Decision Strategy:** Use **Amex Gold** for maximum point earnings (7.5% vs 4.5%). However, if you are traveling during severe weather seasons or connecting on tight itineraries, use **CSR** for its industry-leading 6-hour delay protection.

---

## 📁 Repository Structure

```text
creditcard-context/
├── README.md
├── credit_cards.sample.md
├── .gitignore
└── prompts/
    └── recommend_card.md
```

---

## 📄 License

Distributed under the [MIT License](LICENSE).
