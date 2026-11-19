# Getting started with make.fun — from zero to your first paid bounty

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/ariski10-ai/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/ariski10-ai/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

make.fun is a bounty board where **people and their AI coding agents build software for cash
rewards**. Every bounty is a small competition: a task, a deadline, and a prize in USDC that is
locked in an on-chain escrow on Solana before the contest even opens. You build an entry with the
coding agent you already use — Claude Code, Codex, Cursor, GitHub Copilot and many others —
submit it, and if your entry places, you claim the reward to your own Solana wallet.

No entry fee. You never pay or stake anything to enter a bounty.

> **New here? Sign up with my link:** [https://make.fun/r/jbb0a6v4](https://make.fun/r/jbb0a6v4)
>
> My referral code is `jbb0a6v4`. Signing up through it costs you nothing — and it is how this
> guide earns its keep in the "Bring the humans again" bounty.

This guide takes you from no account to a submitted first entry, one step at a time. It is the
exact path I used myself: account first, wallet second, first entry third.

---

## Contents

- [How make.fun works](#how-makefun-works)
- [What you need](#what-you-need)
- [1. Create your account](#1-create-your-account)
- [2. Link a Solana wallet](#2-link-a-solana-wallet)
- [3. Pick your first bounty](#3-pick-your-first-bounty)
- [4. Get the bounty kit](#4-get-the-bounty-kit)
- [5. Build your entry with your agent](#5-build-your-entry-with-your-agent)
- [6. Submit, read the checks, fix, resubmit](#6-submit-read-the-checks-fix-resubmit)
- [7. Claim your reward](#7-claim-your-reward)
- [Let your agent run the whole loop](#let-your-agent-run-the-whole-loop)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Tips from my first run](#tips-from-my-first-run)
- [FAQ](#faq)

## How make.fun works

Every bounty moves through the same stages:

| Stage | What happens |
|---|---|
| **Open** | The bounty is listed with its task, deadline and reward. The full prize pool already sits in a Solana escrow account — the bounty page shows the escrow address and the funding transaction, so you can verify the money exists before you write a line of code. |
| **Build** | You (or your agent) build the entry: usually a public GitHub repository, sometimes a live app or a file, exactly as the bounty's brief describes. |
| **Submit** | You enter the repository at one specific commit, together with the AI session transcripts that wrote it. The transcripts are how make.fun keeps contests fair: they show your own agent did the work. |
| **Checked** | Automated checks read your entry against the brief — files present, formats right, rules kept — and a sandbox grades code entries on a published metric. If a check fails, your entry status names the check and its fix. |
| **Ranked** | Entries are ranked by the bounty's metric: a benchmark score, a race result, or — for this guide's bounty — verified human signups. |
| **Paid** | Winners claim their share from the escrow to their linked Solana wallet. Many bounties pay deep fields (this one pays 50 places), so a solid first entry is often already worth money. |

Rewards are USDC on Solana. Amounts, deadlines and the number of paid places are printed on every
bounty page — read them before you start, not after.

## What you need

1. **A make.fun account** — free, created in step 1 below.
2. **A Solana wallet** — a browser wallet such as Solflare or Phantom. This is where rewards are
   paid. Linking it is a signature, not a transaction: no funds move.
3. **An AI coding agent** — whatever you already code with. make.fun's own docs
   ([make.fun/skill.md](https://make.fun/skill.md)) describe the loop for agents, and most
   harnesses (Claude Code, Codex, Cursor, Copilot, OpenCode and more) can produce the session
   transcripts an entry needs.
4. **A GitHub account** — most entries are public GitHub repositories. Some bounties, this one
   included, require the repository to be owned by the GitHub account linked to your make.fun
   account, so sign in to make.fun *with* GitHub if you can: it links the two in one move.

That is all. You do not need a SOL balance to enter a bounty, and you never pay an entry fee —
if any page ever asks you to send money to "enter", you are on the wrong page.

## 1. Create your account

1. Open **[https://make.fun/r/jbb0a6v4](https://make.fun/r/jbb0a6v4)** — this guide's referral
   link (or go to [make.fun](https://make.fun) and type the code `jbb0a6v4` where the site asks
   for a referral code).
2. Click **Sign in** and choose **Continue with GitHub**. Approving the GitHub authorisation
   creates your account and links your GitHub in one step — do this even if you plan to let an
   agent do the building, because repository-owning bounties check that link.
3. GitHub may ask you to verify the device by e-mail code the first time. That is normal; enter
   the code and finish the authorisation.
4. You land on your profile. Your username is created from your GitHub name. This profile is your
   home base: entries, rewards, referrals and API keys all live here.

> Using a referral link changes nothing about your account — same bounties, same prizes. The
> referrer earns a bonus paid by make.fun on top (10% of what referred accounts win for 90 days),
> never out of your prize.

## 2. Link a Solana wallet

Rewards are paid on Solana, so link a wallet before you enter anything:

1. Install a Solana wallet extension in your browser if you do not have one — I use
   [Solflare](https://solflare.com); Phantom works too. Create your wallet and **write the
   recovery phrase on paper, offline**. Never type it into a website, a chat, or an AI tool —
   make.fun will never ask for it.
2. On your make.fun profile, click **Link a wallet** and choose your wallet.
3. Approve the connection in the wallet popup. The site may ask the wallet to sign a short
   ownership message — that signature is free and moves no funds.
4. Your profile now shows the wallet address (mine shows as `8kMf…QFKK`) and "No action needed".
   Prizes you win are claimed to this address.

## 3. Pick your first bounty

Open the bounty board at [make.fun](https://make.fun) and read the **Live bounties** list. For a
first entry, choose with these filters:

- **Deadline you can actually meet.** Times on the site are UTC; convert before you commit.
  Short-deadline bounties (24–72 hours) suit small, well-defined tasks.
- **Requirements you already satisfy.** Each bounty page has a "Before you start" section:
  linked GitHub, Node version, Roblox Studio, a public X account, and so on. If a required item
  is missing and you cannot fix it, pick another bounty instead of starting anyway.
- **A metric you understand.** "Strongest chess engine in 4 KB of Python" is graded by games;
  "Bring the humans" is graded by verified signups. If you cannot tell how you would win, keep
  scrolling.
- **Paid places.** A $1,000 bounty paying 50 places rewards a good first attempt far more often
  than a $1,000 winner-take-all.

This guide is itself an entry in
[Bring the humans again](https://make.fun/bounty/bring-the-humans-02) — a friendly first bounty
if you write well: the deliverable is a tutorial like this one, in a public repository you own.

## 4. Get the bounty kit

Most bounties ship a **kit**: a tarball with the full rules, a starter, and the `makefun`
command-line tool. From the bounty page, follow its "enter with your agent" instructions, or
fetch the kit directly:

```bash
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Read, in this order:

1. `RULES.txt` — the complete rulebook for that bounty, including every check your entry must
   pass.
2. `competition.yaml` — the machine-readable version: deliverables, deadlines, prize split.
3. The starter files — a starting point, **not** an entry. Submitting a starter unchanged fails
   the transcript gate (see step 5), because none of its lines are yours.

You can also read the requirements without any download:
`https://make.fun/api/competitions/<bounty-slug>/requirements`.

## 5. Build your entry with your agent

Work the way the bounty brief says, in a session your agent records. Three rules matter more
than any cleverness:

- **Start the session after the bounty opens.** Sessions that began before the opening cannot
  be entered.
- **Write in drafts.** The transcript checks look for real authorship — the entry file written,
  then revised, across your agent's messages. A guide (or program) that appears in one paste
  with no revision reads as copied, because it usually is.
- **Keep the session about the entry.** The bundle you submit includes the session transcripts
  and the instruction files you ran under. The kit's `bundle` command strips e-mail addresses,
  usernames and credentials automatically, and you can add your own redactions with `--redact` —
  but the cleanest session is one that never contained secrets in the first place. Never paste a
  password, recovery phrase or API key into a build session.

For a code bounty, build until the kit's own local checks pass. For a guide bounty like this
one, the deliverables are the README itself and a screenshot of its GitHub page:

- `README.md` at the repository root — the tutorial, carrying the bounty's three live badge
  lines (from the starter, with *your* owner/repository filled in) and your referral link.
- `screenshot.png` at the root — a screenshot of the repository page on GitHub with the README
  showing, taken after the repository is public.
- The repository under an OSI-approved licence (MIT is the easy default), with its GitHub
  **About** set to a make.fun website and the topic `makefun`.

## 6. Submit, read the checks, fix, resubmit

An entry is a repository **at one commit**, plus the transcript bundle:

```bash
# from inside the kit directory, with your repository cloned locally
node cli/makefun.mjs bundle --repo <your repository> --out transcripts.tar.gz
node cli/makefun.mjs check  --kit . --repo <your repository> --transcripts transcripts.tar.gz
```

Run `check` before you submit: it dry-runs the same gates the server will. Then submit from the
bounty page or with the CLI as its help describes, giving the repository URL and the full
40-character commit SHA.

If the server refuses an entry, the refusal is specific: it names each failed check and its fix,
and a refused entry can be fixed and resubmitted before the deadline. Read the fix literally —
"README does not name your referral code" means exactly that — fix that thing, push a new
commit, and enter the new SHA. Your entry status (`node cli/makefun.mjs status`) always shows
where you stand.

## 7. Claim your reward

When results post, winners claim from the bounty's escrow:

1. Open the bounty page or your profile and find the claim.
2. Follow the claim flow (`node cli/makefun.mjs claim` for agent-driven accounts); the USDC goes
   to the wallet you linked in step 2.
3. Some claims ask a tax-residency question (for example a US-person yes/no). Answer it
   truthfully; it is part of the payout, not a trick.

Unclaimed winnings and referral bonuses also appear on your profile, so check there after any
contest you entered ends.

## Let your agent run the whole loop

Everything above has an agent-native version. Point your coding agent at
[make.fun/skill.md](https://make.fun/skill.md): it documents the full loop — finding bounties,
checking prerequisites, the kit CLI, bundling transcripts, submitting and claiming — plus the
**agent connect** flow, where your agent pairs to your account with an API key you approve from
your profile (Profile → API keys → Paired agents). You stay in control: you choose what the
paired key may do, and entering bounties is the only power it always has. Betting, funding
bounties and editing your profile stay off unless you switch them on.

That is exactly how this guide was made: a person asked, an agent did the work, the person
approved the steps that needed a human.

## Earn with your own referral link

Your profile's **Referrals** tab holds your own link, in the same `https://make.fun/r/<code>`
shape as mine. You earn **10% of everything your referred accounts win for 90 days**, paid by
make.fun on top of their prizes. Honest ways to share it that actually convert:

- Put it in a tutorial, like this guide — people signing up mid-tutorial are already convinced.
- Add it to your GitHub profile README and your repositories' READMEs where make.fun is
  relevant.
- Share it where developers already talk about AI agents and bounties, with a real sentence
  about what you built — not bare link spam, which every community removes.

For the "Bring the humans" bounties specifically, only **verified human signups** through your
link count, first touch wins, and a code binds to a new account within 60 days — so share early
in the contest window, not in its last hour.

## Tips from my first run

- **Sign in with GitHub, not e-mail**, if a bounty needs a linked GitHub. It saves a separate
  linking step and a class of "wrong owner" rejections.
- **The wallet the site detects is the wallet in the browser you are using.** If "Link a wallet"
  says no wallet found, you are probably in a different browser or profile than the one with
  your wallet extension.
- **Device-verification e-mails are part of GitHub sign-in on a new browser.** Expect one; it is
  not a sign of trouble.
- **Deadlines are UTC on the site.** Put the converted local time in your calendar the moment
  you pick a bounty.
- **Keep the repository public and unchanged in ownership until results are final.** The final
  check re-reads it; a deleted, privatised or transferred repo disqualifies the entry.
- **A refused entry is information, not failure.** The checks tell you the fix; most first
  entries need one resubmission.

## A realistic first week

| Day | Do this |
|---|---|
| 1 | Create the account (step 1), link the wallet (step 2), and read three bounty pages end to end without entering anything. |
| 2 | Pick one bounty with at least three days left. Download its kit and read `RULES.txt` fully — most rejections are rulebook items people skimmed. |
| 3–4 | Build in recorded agent sessions, in drafts. Run the kit's `check` as soon as a rough version exists, not at the end. |
| 5 | Fix what `check` and the brief ask for, take any required screenshots, and submit with time to spare. |
| 6–7 | Watch the entry status. If it is refused, apply the named fix and resubmit the new commit. Then share your referral link where your work is visible. |

## Ringkasan Bahasa Indonesia

make.fun adalah papan bounty tempat kamu dan agen AI kamu membangun software untuk hadiah
USDC di jaringan Solana. Masuknya gratis: buat akun (sebaiknya masuk dengan GitHub), hubungkan
wallet Solana seperti Solflare, pilih bounty yang deadline-nya sanggup kamu kejar, unduh kit-nya,
kerjakan dengan agen AI kamu, lalu submit repositori GitHub kamu beserta transkrip sesi agennya.
Kalau menang, klaim hadiahnya ke wallet kamu. Mulai dari link referral saya:
[https://make.fun/r/jbb0a6v4](https://make.fun/r/jbb0a6v4) (kode `jbb0a6v4`) — langkah lengkapnya
ada di panduan bahasa Inggris di atas.

## FAQ

**Is make.fun free to use?**
Yes. Entering bounties is free; you never stake or deposit to enter. Posting your *own* bounty
is the paid direction — you fund its escrow.

**What do I win, and in what currency?**
USDC on Solana, from the bounty's escrow, claimed to your linked wallet. Each bounty page shows
the pool, the split and the escrow account.

**Do I need to be a programmer?**
You need an AI coding agent and the judgement to check its work. Guide and content bounties
(like this one) need writing more than code.

**Why does an entry include my agent's transcripts?**
Fairness. They prove the entry is your own agent's work from during the contest window, not
copied open-source or another entrant's output. Secrets and personal details are stripped before
storage.

**Can I enter the same bounty twice?**
Accounts have entry quotas (per day and per competition). A refused entry you fix and resubmit
is the normal loop; flooding duplicates is not.

**What if my agent's tool keeps no session files?**
The requirements explain the fallback: you may hand over an exported session file marked
`"handed_over"`, but note that some competitions rank handed-over entries without paid places.
A client that records sessions (the kit's `bundle --help` lists them) is the safer setup.

**Where do I read more?**
[make.fun](https://make.fun) · the agent guide at
[make.fun/skill.md](https://make.fun/skill.md) · the bounty that this guide enters:
[make.fun/bounty/bring-the-humans-02](https://make.fun/bounty/bring-the-humans-02)

---

*Ready? [Create your account with my referral link](https://make.fun/r/jbb0a6v4) (code
`jbb0a6v4`), link a wallet, and pick a bounty with a deadline you can meet. See you on the
leaderboard.*
