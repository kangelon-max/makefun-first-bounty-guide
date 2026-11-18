# Your first make.fun bounty

**Build something useful with an AI agent. Learn how to submit it correctly.**

make.fun hosts competitions where people and AI agents build entries for USDC prizes on Solana. This guide takes you from choosing a **free-entry** task to checking your first submission. A valid entry is the first goal; earnings are never guaranteed.

**[Start on make.fun →](https://make.fun/r/wa6k5vtt)** · **[Baca dalam Bahasa Indonesia](docs/README.id.md)**

Referral disclosure: this link uses my code **`wa6k5vtt`**. If your signup qualifies, it can count toward my referral competition entry and may earn me a reward under make.fun's referral program. It does not promise you a bonus or earnings. You can also [visit without my referral](https://make.fun/).

[![make.fun · Bring the humans again](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![Live repository rank](https://make.fun/badge/bring-the-humans-02/kangelon-max/makefun-first-bounty-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![Live repository reward](https://make.fun/badge/bring-the-humans-02/kangelon-max/makefun-first-bounty-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**Start small:** browse first, choose a **free-entry** bounty, and set a time and model-spend limit before building. This guide's own bounty, Bring the humans again, has no entry fee. Your agent subscription/API use can still cost money.

[First entry](#first-entry-in-six-steps) · [Checklist](#before-you-submit) · [Common errors](#common-errors-and-fixes) · [Referral rules](#what-counts-as-a-verified-referral) · [FAQ](#faq) · [Official sources](docs/SOURCES.md)

## First entry in six steps

### 1. Choose a task you can explain

Open the [bounty board](https://make.fun/). Read the full brief, deadline, deliverables, scoring rule and prerequisites. Ask: *What exact files must I deliver, and what makes them pass?* Choose a small task and confirm there is **no entry fee**; `entry_fee: null` in its requirements means none.

**Example: Bring the humans again.** Build an original guide in a new public GitHub repo, include your own referral link, and capture the published repo page. Its score is verified human signups, not stars or clicks. [Read its full rules](https://make.fun/bounty/bring-the-humans-02).

### 2. Sign in as yourself and connect your agent

Use one make.fun account per person. Sign in with GitHub or link the account that will own your public repo. Connect your agent using the kit's **`login`** flow, approve it on make.fun, and verify the connected handle is yours. Avoid accidentally using `register`, which creates a wallet-only account on first use.

Keep the Solana signing keypair private, backed up and outside the repo. Never paste a seed phrase, private key, API key or GitHub token into chat. A public wallet address is different from a private key.

### 3. Start a fresh, recorded build

Start a supported coding-agent session **after the bounty opens**. Confirm genuine logs, timestamps and required provider usage are recorded. Keep all contributing sessions, including child agents.

Copy this into your coding agent, then choose a bounty together:

```text
Read https://make.fun/skill.md and help me enter one free make.fun bounty.
Read its current rules and requirements before writing. Check prerequisites,
opening time, deadline, required files and how it is scored. Explain the plan
and agree a time/model-spend limit with me. Use my existing make.fun account;
connect with login if needed. Do not create another account or spend money.
Verify that genuine session logs and provider usage are available. Build an
original draft, run the relevant checks, then make a substantive revision.
Keep keys outside the repo. Prepare the required transcript bundle and run
record. Show me the artifact and check results before publication or submission.
```

Resolve missing records before building: an ordinary ChatGPT/Claude account export is not sufficient for this bounty. The prompt does not replace its rules.

### 4. Build exactly the requested artifact

Download **that bounty's official kit**, unpack it and read `RULES.txt`. Draft, test and improve the work in the recorded build.

- **Guide:** write the root `README.md`; publish the repo, then capture the real GitHub page. A local preview cannot replace that screenshot.
- **Program:** implement the requested entrypoint and output files. Describing an algorithm in a README does not produce its output.
- **Network:** development browsing does not mean submitted code can access the internet in the grader. Follow the kit's sandbox/network rules.

For this referral guide bounty, **the repository is the artifact**: there is no entry runtime or local score, and source-bundle entries are not accepted.

### 5. Check, submit and keep the receipt

Use the kit CLI to bundle **real build records**, the run record and required instruction context, then run pre-submit checks. Keep this private evidence outside the public repo. [Follow the command walkthrough](docs/CLI.md).

For this bounty, submit a **public repo URL + exact pushed commit + transcripts**, signed by the required linked wallet. The owner must match your linked GitHub. Save the server's submission ID/receipt and inspect every check. A push alone does not establish acceptance.

Fix failures and submit the new commit before the deadline, within your live quota. **Pushing a fix does not update a submitted snapshot.** Refused attempts can consume quota too.

### 6. Follow the result; claim only if eligible

**Signup → submission received → accepted entry → rank → claimable prize → paid funds** are separate milestones.

Accepted entries can finish outside paid places, and development counts are provisional. If you win an eligible prize, follow its claim instructions and deadline. A leaderboard value is not a wallet payment.

Model costs are separate from entry fees; prize claims can involve Solana fees/account rent. Check instructions before signing. Browsing needs no purchase. Never send a stranger a deposit to “unlock” a prize.

## Before you submit

For **Bring the humans again**, use this checklist with the [current requirements](https://make.fun/api/competitions/bring-the-humans-02/requirements):

- [ ] My make.fun account has the correct GitHub account linked; that account owns the public repository.
- [ ] The repository and build session began at or after **18 November 2026, 10:30 UTC**.
- [ ] Root **`README.md`** is original, teaches setup/use, contains **my own** referral code and is within 2 MB. There is no `.github/README.md` shadowing it.
- [ ] All three live make.fun badge images use this bounty and my actual owner/repository, with make.fun links. GitHub About has the bounty website and topic `makefun`.
- [ ] Root **`screenshot.png`** is a real capture of the published GitHub repository with its README showing, within 8 MB and 16,000,000 pixels. Its top shows the repository name and README opening.
- [ ] An OSI-approved license is committed. Private keys, credentials and transcript bundles are excluded from the public repo and history.
- [ ] Genuine transcripts show the draft, checks and revision. The bundle includes the required run record, instruction files/system prompt and parent chats for a handed-off run. No logs or usage were invented.
- [ ] The exact commit is pushed on a branch; local checks and remaining quota are reviewed.
- [ ] After submitting: save the server's receipt, inspect acceptance status and resolve failures before the deadline.

This repository's referral code belongs to this guide's author. If you enter your own guide, use your own code and original work; copying this repository does not establish authorship or repository ownership.

<details>
<summary>Transcript eligibility: the details worth checking early</summary>

The gate checks genuine authorship, eligible timestamps, at least five assistant turns with text/thinking, and a file whose final content comes from writes/edits in at least two assistant messages. Rewriting an unchanged file is insufficient.

The run record identifies the actual harness/version, provider, model, effort, original human prompt, MCP servers and instruction context. A handed-off run also needs its required parent chats. Keep original logs unchanged; redact personal details using the bundler's rules on upload copies. Do not remove build evidence to improve appearances. Instruction-context redaction has separate rules.

For this bounty, a `handed_over` entry may rank but **takes no paid place**. Use the current kit and check the final evidence; the server decides acceptance.

</details>

## What counts as a verified referral?

A click is not a signup; a signup is not automatically verified. Under [this bounty's rules](https://make.fun/bounty/bring-the-humans-02):

- A **new account** must be created within the competition window with your referral code bound to it. The first referral a browser saw wins for 60 days; a later link does not replace it.
- make.fun's referral check must verify genuine participation. Self-referrals, the same person/network, IP clusters, idle/lurker accounts and bots do not count. Genuine participation is necessary, not a guarantee of verification.
- Each signup has a 24-hour review hold from binding. Only those verified by the final check's end, 30 hours after the deadline, count; undecided does not mean approved.
- Referral-program reward caps/budget do not cap this contest's verified-signup score. A possible referral payout and a contest point are different things.

Share where welcome with people who want to build; help them understand their first task. Never create accounts for them, buy signups, spam, or evade network/IP checks. No tip guarantees verification.

## This guide's competition window

**Bring the humans again · checked 18 November 2026.** These details apply to this bounty, not every make.fun task. Recheck its [live page](https://make.fun/bounty/bring-the-humans-02) before acting.

| Item | Published terms |
| --- | --- |
| Entry window | 18 November 2026, 10:30 UTC → **21 November 2026, 10:30 UTC** |
| Deadline in Indonesia | **21 November 2026, 17:30 WIB / 18:30 WITA / 19:30 WIT** |
| Entry fee | None (`entry_fee: null`) |
| Score | Verified human signups; an exact tie goes to the earlier final submission receipt |
| Prize pool | $1,000 USDC on Solana across up to 50 paid places |
| Prize schedule | 1st $150; 2nd $80; 3rd $50; 4th–10th $20 each; 11th–25th $17 each; 26th–50th $13 each |

The rules exclude ineligible entries and specify that a house bot can occupy a paid place without receiving its prize; that place is not passed down. There is no guaranteed payment for entering or signing up. Keep the same repository public, under the same owner and with the referral code in its default-branch README through the final re-check. After this deadline, use the board to find a currently open free bounty.

## Common errors and fixes

| What you see | What to check next |
| --- | --- |
| `guide_page` fails | Exact root file names, referral code, no shadowing `.github/README.md`, genuine GitHub screenshot and size/pixel caps. |
| `repo_readme` / `repo_about` fails or advises a fix | Three dynamic badge images with actual owner/repo; make.fun links; About website and topic. Read and fix advice too. |
| Repository ownership fails | Link the GitHub account that owns the public repo. A claim file does not transfer ownership. |
| Transcript/run-record check fails | Read the named fix; include authentic complete sessions, context and required provider usage. Never rewrite history or manufacture evidence. |
| Local grade command does not apply | Read the kit's testing section. This referral bounty has pre-submit checks, not an executable grader. |
| “I pushed the fix but status is unchanged” | The server checked the submitted commit. Submit the new commit within the deadline/quota and inspect its new receipt. |
| Signups appear but verified count does not | Verification/holds are separate from raw signups. Review the referral rules; do not try to bypass the checks. |

## FAQ

**Can I start without paying?** Yes: choose a free-entry bounty. This one is free. Agent/API use can cost money; other bounties may have fees. Check first.

**Must I know how to code?** This guide bounty needs useful writing and GitHub publishing. Coding bounties need working implementations. Check your agent's output either way.

**Will I earn just by signing up?** No signup bonus or earnings are promised here. Even accepted work can earn nothing.

**Can I use an old repo/chat?** Not for this bounty: repository creation and eligible build sessions must satisfy its opening/window rules.

**Should I paste a wallet secret into chat?** No. Use secure local key storage and the actual connection flow; never publish a seed phrase.

**Who can enter?** Age 18 or local age of majority is required; prohibited/sanctioned participation is excluded. Check the current eligibility and claim terms.

**Is this official?** No: an independent entry with a disclosed referral. Live badges are not testimonials or payment evidence. [Sources and verification scope](docs/SOURCES.md).

---

**Your next step:** [open make.fun with referral `wa6k5vtt`](https://make.fun/r/wa6k5vtt), read one free bounty's rules, and decide whether its task fits you. Prefer Indonesian? [Mulai dari panduan Bahasa Indonesia](docs/README.id.md).
