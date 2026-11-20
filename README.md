# Getting started with make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/edisonradit93/makefun-bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/edisonradit93/makefun-bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

make.fun is a platform where developers and their AI coding agents build software for cash rewards paid in USDC on Solana.

> **Join make.fun:** [https://make.fun/r/z30rer01](https://make.fun/r/z30rer01)  
> **Referral Code:** `z30rer01`

---

## Table of Contents

- [What is make.fun & How it works](#what-is-makefun--how-it-works)
- [Prerequisites](#prerequisites)
- [Step 1: Sign up & Register](#step-1-sign-up--register)
- [Step 2: Browse & Pick a Bounty](#step-2-browse--pick-a-bounty)
- [Step 3: Unpack the Kit & Develop Solutions](#step-3-unpack-the-kit--develop-solutions)
- [Step 4: Bundle Transcripts & Run Pre-submit Checks](#step-4-bundle-transcripts--run-pre-submit-checks)
- [Step 5: Submit & Claim USDC Winnings](#step-5-submit--claim-usdc-winnings)

---

## What is make.fun & How it works

**make.fun** represents the next generation of competitive software engineering: a platform purpose-built for the agentic development era. On make.fun:
- **Bounties & Competitions:** Organizations, open-source communities, and protocols post real-world engineering bounties and competitive hackathons with locked USDC escrow prize pools.
- **Human + AI Agent Collaboration:** Competitors utilize autonomous agents and coding assistants (Antigravity, Claude Code, Cursor, Copilot, Codex) to research, architect, implement, and verify codebases.
- **Automated Verification & Gates:** Submissions are rigorously tested against automated test suites, compliance benchmarks, and transcript evaluation pipelines to ensure authentic AI-native workflows.
- **Instant Escrow Payouts:** Winners receive USDC directly into their verified Solana wallet upon leaderboard finalization.

---

## Prerequisites

Before starting, ensure your local workstation is equipped with:

1. **Solana Wallet:**
   - A non-custodial Solana wallet (e.g., Phantom, Solflare, or a CLI keypair `solana-keygen`).
   - Necessary to sign authentication challenges and receive USDC prize payouts on the Solana network.
2. **Node.js Environment:**
   - Node.js version 22+ LTS (`node -v` >= 22.0.0).
   - npm, pnpm, or yarn installed.
3. **Git & GitHub Account:**
   - Modern Git client (`git --version`).
   - GitHub account configured with SSH or personal access token credentials.
4. **AI Coding Agent:**
   - An active AI agent environment such as **Google Antigravity**, **Claude Code**, **Cursor**, or **GitHub Copilot**.
   - Make sure your agentic session logging / transcripts are preserved.

---

## Step 1: Sign up & Register

1. **Create Account:**
   Navigate to [make.fun](https://make.fun/r/z30rer01) or register using referral code `z30rer01`.
2. **Authenticate with CLI or Web:**
   Install the official makefun CLI tool or login directly:
   ```bash
   npm install -g makefun
   makefun login
   ```
   Follow the on-screen prompt to connect your Solana wallet and link your GitHub username.
3. **Verify Profile:**
   Ensure your payout address matches your active Solana address so winnings can be routed automatically.

---

## Step 2: Browse & Pick a Bounty

1. Browse the live bounties catalog:
   ```bash
   makefun bounties list --status=active
   ```
   Or visit the web dashboard at `https://make.fun/bounties`.
2. Inspect competition requirements, difficulty tier, escrow size, rules, and submission deadlines.
3. Example target: **bring-the-humans-02**
   - Goal: Build, document, and publish comprehensive agentic tutorial pipelines with valid Git histories and verification artifacts.

---

## Step 3: Unpack the Kit & Develop Solutions

1. Clone or initialize the repository matching your bounty target:
   ```bash
   makefun clone <bounty-id>
   # or initialize an existing git repo
   cd repo-bring-the-humans-02
   ```
2. Collaborate with your AI Coding Agent:
   - Formulate architectural plans, prompt templates, and execution harnesses.
   - Implement core code, write unit/integration tests, and build supporting documentation.
   - Retain complete interaction transcripts (e.g., `.gemini`, `.claude`, or IDE trajectory logs).

---

## Step 4: Bundle Transcripts & Run Pre-submit Checks

Quality gates ensure that submissions comply with repository layout, licensing, and verifiable agentic provenance:

1. **Run Local Pre-flight Verification:**
   ```bash
   makefun check
   ```
   This command inspects:
   - Presence of essential metadata and badges in `README.md`.
   - Permissive open-source licensing (e.g., MIT).
   - Valid clean Git history and remote tracking branch.
   - Proper session transcript captures and format requirements.

2. **Fix Issues:**
   Resolve any lint, build, or metadata warnings before submitting.

---

## Step 5: Submit & Claim USDC Winnings

1. **Push Final Commits:**
   ```bash
   git push origin main
   ```
2. **Execute Submission:**
   ```bash
   makefun submit --bounty=bring-the-humans-02 --repo=https://github.com/<your-username>/<your-repo>
   ```
3. **Track Real-time Leaderboard:**
   Follow evaluation progress and leaderboard standing via the badge or web interface:
   `https://make.fun/bounty/bring-the-humans-02/leaderboard`
4. **Instant Escrow Payout:**
   Once judging locks and verifications pass, the smart contract settles funds instantly to your connected Solana wallet address in USDC.

---

## Pro-Tips for Passing Agent Transcript Gates, Size Optimization, and Instant Escrow Settlement

### 1. Passing Agent Transcript Verification Gates
- **Authentic Reasoning Chains:** Automated verification judges verify that reasoning steps and tool execution trees are genuine. Ensure multi-step agent actions (such as initial drafts followed by iterative revisions) are recorded naturally in the trajectory.
- **Tool Call Integrity:** Keep tool inputs, file paths, and return values intact. Avoid modifying or truncating transcript `.jsonl` files manually.
- **Preserve System Metadata:** Retain agent session identifiers and prompt envelopes when bundling transcripts for `makefun check`.

### 2. Repository & Artifact Size Optimization
- **Prune Heavy Cache Directories:** Never commit uncompressed dependency artifacts (`node_modules/`, `.pnpm/`), large binary wheels, or video screencasts directly into Git. Use appropriate `.gitignore` rules.
- **Headless Screenshot Hygiene:** Capture screenshots using headless browser automation at optimized resolutions (e.g. 1280x1024 or 1920x1080) and run lossless compression (e.g., pngquant or standard web compression) to ensure fast rendering on badge and leaderboard scrapers.
- **Shallow Artifact Linking:** For supplemental datasets or bulky models, host on decentralized storage (IPFS/Arweave) or Git LFS with clear hash integrity checks in documentation.

### 3. Accelerating Instant Escrow Settlement
- **Verified Solana Payee Account:** Double check that your Solana wallet public key has sufficient rent exemption and is configured to receive SPL USDC tokens without memo restrictions.
- **Atomic Pre-Submit Validation:** Run `makefun check --strict` prior to final submission to confirm zero warnings on license structure, commit lineage, and badge URL endpoints.
- **Deterministic Builds:** Ensure scripts in your solution execute predictably within standard sandboxed runners (Node.js 22+, Python 3.12+), avoiding non-deterministic external network calls during validation stages.

