# ⚡️ Cha-Ching Monorepo 🚀

Welcome to **Cha-Ching**, the ultimate hackathon project for onchain bounty payments, automated GitHub workflows, and next-gen web experiences – all deployed at **[cha-ching.it](https://cha-ching.it)**!

---

## 🗂️ Monorepo Structure

```bash
/cha-ching
  /app           # Next.js 15 app (NextAuth.js)
  /backend       # Node.js API server (Nest.js)
  /bot           # GitHub bot (Custom workflow engine)
  /contracts     # Solidity smart contracts (Hardhat3)
```

---

## 💡 Tech Stack

✅ **Next.js 14** – Frontend framework <br>
✅ **NextAuth.js** – GitHub OAuth authentication <br>
✅ **shadcn-ui** – Beautiful components (dark mode by default!) <br>
✅ **Hardhat/Foundry** – Ethereum smart contract toolkit <br>
✅ **Node.js** – Backend API server <br>
✅ **Probot** – GitHub bot for automations <br>
✅ **pnpm workspaces** – Monorepo dependency management <br>

---

## 🚀 Quick Start

### 1️⃣ Install dependencies

```bash
pnpm install
```

### 2️⃣ Environment Variables

Each package has its own `.env`:

```bash
/app/.env.local
/backend/.env
/bot/.env
```

Example for the frontend (`.env.local`):

```env
NEXTAUTH_SECRET=your_random_secret
NEXTAUTH_URL=https://cha-ching.it
GITHUB_ID=your_github_client_id
GITHUB_SECRET=your_github_client_secret
```

### 3️⃣ Local Development

Spin up the entire monorepo stack:

```bash
pnpm dev
```

This will:
✅ Start the Next.js frontend
✅ Run the backend API server
✅ Deploy contracts to local blockchain (Hardhat node)
✅ Start the GitHub bot

### 4️⃣ Smart Contracts

```bash
cd apps/contracts
pnpm build     # Compile contracts
pnpm test      # Run tests
```

### 5️⃣ GitHub Bot

The bot runs with **Probot**. To start it locally:

```bash
cd apps/bot
pnpm dev
```

---

## 🌍 Live Demo

👉 Visit: **[https://cha-ching.it](https://cha-ching.it)**
👉 Sign in with GitHub (NextAuth.js)
👉 Experience the hacker-ready dark mode!

---

## 🌟 Features

✅ **GitHub OAuth** – Sign in with your GitHub account <br>
✅ **Dark Mode Default** – Smooth hacker aesthetic 🌒 <br>
✅ **Onchain Smart Contracts** – Deploy and manage bounties <br>
✅ **GitHub Bot** – Automate bounty payouts and workflows <br>
✅ **Shared Monorepo** – Everything in one place, ready to hack! <br>

---

## 🛠️ Extending It

- Deploy to Vercel for production
- Add Prisma or other DB to persist data
- Integrate custom GitHub webhooks
- Expand bot to handle issue labeling, bounty verification, and more!

---

## 🪙 License

MIT – do what you want, just give credit!

---

### 💬 Questions or Ideas?

Open an issue or PR – let’s build together!

---

> Let’s make onchain bounties effortless, automated, and beautiful with **Cha-Ching**! 💸✨
