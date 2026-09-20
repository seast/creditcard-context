# 💳 CreditCard Context (`credit_cards.md` Template)

> AI-Friendly Credit Card & Rewards Optimization Context for LLM Tools (Muse, Cursor, ChatGPT, Claude, etc.)

**CreditCard Context** is a structured Markdown workspace template designed to bring intelligent credit card management and reward optimization to your favorite AI tools. By loading your custom `credit_cards.md` file into tools like **Muse** or **Cursor**, your AI assistant can instantly calculate valuation-adjusted return rates, track quarterly 5% spend caps, warn you about expiring annual credits, and recommend the best card for any purchase.

---

## ✨ Key Features

- **🔒 Privacy First**: Stores card names, tiers, categories, and quarterly spend progress—**never full card numbers, expiration dates, or CVVs**.
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

> **Note**: Be sure to add `credit_cards.md` to your `.gitignore` to prevent committing personal notes or custom progress details to public repositories.

### 2. Customize Your Portfolio
Fill in your credit card portfolio following the template format:
- Group cards by **No Foreign Transaction Fee** vs. **Has Foreign Transaction Fee**.
- Record multipliers, annual fees, statement credit reset dates, and active free trial expirations.
- Perform a quick monthly or quarterly check-in to update 5% rotating category status and spend cap progress.
- You can use common AI tools to fill the contents.

### 3. Load into Your AI Workspace
- **Muse**: Add `credit_cards.md` as a context file in your workspace settings or file tree, add to memory.md
- **Cursor / VS Code**: Reference `@credit_cards.md` directly inside chat prompts.
- **ChatGPT / Claude**: Attach `credit_cards.md` or paste its text into your Project Knowledge / Custom Instructions.

---

## 💡 Example Prompts

Once `credit_cards.md` is loaded into your AI tool, try asking:

- **Purchase Recommendation**:
  > "I am booking an Airbnb for $500 and spending $80 at a restaurant. Which cards should I use for maximum reward value?"
- **Multi-Card Category Strategy**:
  > "What is my optimal dining order for Q4 across all my cards, taking into account quarterly caps and base point valuations?"
- **Perk & Audit Check**:
  > "Review my credit cards for any annual travel credits or subscription trials expiring soon that I need to use or cancel."

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
