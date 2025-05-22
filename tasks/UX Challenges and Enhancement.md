## 🧩 **GiverLiquidity: UX Challenges and Enhancement Proposals**

**Goal:**
To create a UX that is accessible for **Web3 beginners**, while maximizing **social impact through SNS integration**.

---

### 🟥 **\[Challenge] SUI Gas Fees Are Too High a Barrier**

#### ▸ Problems:

- Web3 novices often **don’t own any SUI tokens**
- Obtaining SUI via wallet creation, CEX, or bridges is too complex
- Not suitable for **physical events** or **volunteer-oriented use cases**

---

### ✅ **\[Solution 1] Gasless Architecture via Relayer (Transaction Sponsorship)**

#### ▸ Technical Approach:

- Use **zkLogin** for authentication
- A **relayer** signs and submits the transaction on the user's behalf

#### ▸ Benefits:

- **No SUI or wallet required** for end users
- Accessible for event attendees and the general public
- Web2-like UX: One click to **prove donation**

---

### ✅ **\[Solution 2] zkLogin for SNS Account Authentication**

#### ▸ What is zkLogin?

- A method to convert OAuth logins (Google, Twitter, etc.) into ZK proofs, allowing those identities to **sign transactions on Sui**
- No wallet generation needed — uses OAuth identity for signing authority

#### ▸ Usage Example:

- Log in with **Twitter** → Join GiverLiquidity
- Link **Twitter handle** to donation transaction
- **Relayer covers the gas fees**

---

## 🌐 **Extensions: Visualizing Social Impact**

---

### ✅ **\[Proposal 1] Giver Leaderboard**

| Category | Details                                                               |
| -------- | --------------------------------------------------------------------- |
| Metrics  | Total donations, types of swag donated, event-based rankings          |
| UI       | Display Twitter icon, display name, donation stats in table/card view |
| Purpose  | Showcase “**Visible Altruism**” and introduce gamification            |

---

### ✅ **\[Proposal 2] Real-Time Donation Feed**

| Category | Details                                                         |
| -------- | --------------------------------------------------------------- |
| Content  | Example: “@username donated Devcon swag”                        |
| Tech     | Combine on-chain logs with Walrus/Arweave for off-chain logging |
| Usage    | Display on venue monitors, event websites, social media sharing |

---

### ✅ **\[Proposal 3] SNS-Driven UGC Amplification**

| Category | Details                                                        |
| -------- | -------------------------------------------------------------- |
| UX       | Share button after donation generates a tweet template         |
| Example  | “I donated my Devcon swag. #GiverLiquidity #Web3CSR”           |
| Purpose  | Encourage **organic marketing through user-generated content** |

---

## 🔒 **Security and Ethical Considerations**

- Twitter handles/display names can be **masked or anonymized** (e.g., `@alice****`)
- No use of **GPS/location data** to ensure privacy
- Donation intent/history is stored in **immutable, tamper-proof storage**

---

## 📌 **Recommended Architecture Summary**

| Component      | Recommended Approach                             |
| -------------- | ------------------------------------------------ |
| Authentication | zkLogin (Twitter OAuth)                          |
| Execution      | Gasless via Relayer                              |
| Display        | Leaderboard + Real-Time Feed                     |
| Distribution   | SNS sharing path (Twitter)                       |
| Storage        | On-chain via Sui + Arweave/Walrus for permanence |

---

Through this architecture, GiverLiquidity transforms **“Donation = Goodwill = Pride”** into a **visible and gamified experience**, delivering a **non-custodial, gasless UX** accessible to everyone.
