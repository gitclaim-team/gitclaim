<div align="center">
  <img src="./assets/gitclaim-logo.png" alt="GitClaim Logo" width="300"/>
  <h1>⚡️ GitClaim Monorepo 🚀</h1>
</div>

Welcome to **GitClaim**, your all-in-one solution for on-chain bounty payouts, AI-powered GitHub workflow automation, and futuristic web coordination - live at **[https://gitclaim.axlabs.com](https://gitclaim.axlabs.com)**!

Here’s how GitClaim **supercharges open-source collaboration:**
1. 🪙 Create & fund a bounty tied to a GitHub issue.
2. 🤖 GitClaim AI Agent recommends bounties to developers based on their skills.
3. 🔧 Developers submit PRs to fix issues and claim bounties.
4. ✅ Once merged, the GitClaim GitHub App releases funds onchain using a [vlayer WebProof](https://book.vlayer.xyz/features/web.html) with the support of [Filecoin](https://filecoin.io/).

<em>No middlemen. No spreadsheets. Just seamless, verifiable rewards for real contributions.</em>

## 🧠 How does it work

1. **Fund the bounty.**  
   - A project maintainer opens a GitHub issue and deposits the reward into GitClaim’s on-chain escrow smart contract.  
   - The funds now wait safely until the work is finished.

2. **Match builders to bounties.**  
   - Developers go to the [GitClaim app](https://gitclaim.axlabs.com) and click on "Claim a bounty".
   - Developers have the opportunity to tell our AI Agent what they are good at, or what are they keen to solve. For example, "I'm good at Golang, but would like to develop my Solidity skills as well".
   - GitClaim AI Agent recommends the most relevant open bounties.

3. **Submit the fix.**  
   - A developer forks the repo, creates a branch, and opens a pull request (PR).  
   - In the PR description they add a [closing keyword](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword) like `Fixes #123` to link it to the issue.  
   - The GitClaim AI Agent immediately asks, "What wallet address should we pay if this PR is merged?"

4. **Provide a payout address.**  
   - The developer replies with their wallet (e.g., `0xA0A1…`).  
   - The GitClaim AI Agent validates the address and logs it for the payout.

5. **Review & choose the best PR.**  
   - Multiple developers can compete on the same issue.  
   - Project maintainers review the submissions and merge the PR that solves the problem.

6. **Generate an auditable proof.**  
   - When the PR is merged, GitClaim collects key metadata (commit hash, issue ID, PR link, etc).  
   - That metadata is pinned to [Filecoin](https://filecoin.io/) as a public, tamper-proof record.  
   - A [VLayer WebProof](https://book.vlayer.xyz/features/web.html) is created from the Filecoin link.

7. **Release the funds automatically.**  
   - The GitClaim AI Agent submits the WebProof to the escrow smart contract. 
   - The contract verifies the proof and instantly releases the bounty to the developer's wallet.

👉 **Result:** no middlemen, no spreadsheets—just a transparent, end-to-end flow from "bug found" to "payment sent", all backed by on-chain guarantees and public proofs.

## 🗂️ Monorepo Structure

```bash
/gitclaim
  /app           # Next.js 15 app (NextAuth.js)
  /backend       # Node.js API server (Nest.js)
  /contracts     # Solidity smart contracts (Foundry)
  /envio-indexer # Blockchain indexer (Envio HyperIndexer)
```

## 💡 Tech Stack

✅ **Next.js 14** – Frontend framework <br>
✅ **NextAuth.js** – GitHub OAuth authentication <br>
✅ **shadcn-ui** – Beautiful components (dark mode by default!) <br>
✅ **Hardhat/Foundry** – Ethereum smart contract toolkit <br>
✅ **Node.js** – Backend API server (NestJS) <br>
✅ **Probot** – GitHub bot for automations <br>
✅ **pnpm workspaces** – Monorepo dependency management <br>

---

## 🌍 Live Demo

👉 Visit: **[https://gitclaim.axlabs.com](https://gitclaim.axlabs.com)**

---

## 🪙 License

MIT – do what you want, just give credit!

---

### 💬 Questions or Ideas?

Open an issue or PR – let’s build together!

---

> Let’s make onchain bounties effortless, automated, and beautiful with **GitClaim**! 💸✨
