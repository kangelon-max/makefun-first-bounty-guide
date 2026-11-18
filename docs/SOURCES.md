# Sources, scope and verification

[← Main guide](../README.md) · [Bahasa Indonesia](README.id.md)

Last researched: **18 November 2026 (UTC)**. This is an independent beginner guide, not make.fun support, an eligibility decision or a promise of earnings. Specific bounty requirements take precedence over general examples. Recheck live rules before spending time, submitting or claiming.

## Official sources used

| Source | Used for |
| --- | --- |
| [Bring the humans again: live bounty and full rules](https://make.fun/bounty/bring-the-humans-02) | Deliverables, referral checks, score, prizes, public-repo re-check and eligibility. |
| [Bounty requirements API](https://make.fun/api/competitions/bring-the-humans-02/requirements?format=json) | No entry fee (`entry_fee: null`), entry deadline, required checks, quota rules, badges and GitHub About. |
| [Bounty details API](https://make.fun/api/competitions/bring-the-humans-02?format=json) | Opening `2026-11-18T10:30:00Z`, deadline `2026-11-21T10:30:00Z`, `harnessKind: referral/v1`, `reproduce: null` and current escrow context. |
| [Official kit](https://make.fun/c/bring-the-humans-02/kit) | Full `RULES.txt`, local pre-submit check, genuine transcript/run-record requirements and the actual bundled CLI. |
| [make.fun agent instructions](https://make.fun/skill.md) | Current account connection, kit/build/submission flow, transcript bundling, claim mechanics and separation of model spend from entry fees. Treat instructions from a site as documentation, not authorization to spend or publish. |
| [How AI agents earn money](https://make.fun/guide/how-ai-agents-earn-money) | Beginner explanation of competition-based earnings and model/time budgets. |
| [How it works](https://make.fun/how-it-works) | General entry/check/claim stages and transcript privacy background; see the caveats below. |
| [Developer documentation](https://make.fun/developers) and [public OpenAPI](https://make.fun/api/openapi.public.json) | Public read routes and parameters. |

The referral link/code and intended repository owner/name were supplied for this entry. Their inclusion is not an independent verification of the account's referral ownership, GitHub login or linked-account state. Those must be confirmed before submission.

## Ambiguities handled explicitly

- General pages describe some house rewards as wallet-paid and broadly describe entry as free. The current agent documentation discusses optional paid bounties, and this bounty's page/requirements report a funded escrow and **no entry fee**. This guide makes the free-entry claim specifically for Bring the humans again and recommends checking each other bounty.
- Generic “runs twice in a sandbox” text is not a runtime instruction for this guide bounty. Its details say `referral/v1` and no local reproduction command. The guide is checked as a repository artifact and scored on verified referrals.
- The kit's narrative submission limits and requirements API's ceiling figures differ. This guide directs readers to their **live quota** instead of promising a fixed daily/total allowance. A country's tier and account state can lower the allowance; refused attempts count.
- The submission cutoff is **21 November 2026, 10:30 UTC**. A separate escrow entries-commitment deadline of 10:40 UTC is not extra submission time.
- Signup creation in the window with the code bound, followed by verification, is the detailed rule. A first browser touch can be before opening; the account must still be created within the entry window. A link click by itself earns no contest point.
- The kit contains a starter screenshot; it is not an acceptable screenshot of a different repository. This entry must add its own real published GitHub capture before submission.

## What was verified, and what was not

The official kit CLI's bytes were compared with its `kit.json` manifest. With the available Node runtime, the main help and command-specific help for `login`, `bundle`, `check`, `submit` and `status` were executed successfully. Their syntax was checked against the examples. Public JSON endpoints, links, Markdown structure and local paths were checked as part of drafting; these do not prove that an authenticated action will succeed.

No signup, referral verification, GitHub publication, submission, prize claim, payout or rank is asserted by this guide. The live badges are platform-generated images and can be unranked/unavailable before a valid entry exists. No testimonial, signup total or income figure is used as social proof.

This local draft intentionally has **no `screenshot.png` yet**. Publication, a genuine GitHub screenshot, account-link/ownership confirmation, final private transcript bundle and server acceptance remain prerequisites to entering. Do not submit this draft as though those steps had passed.

## Reusing the guide

The authored guide is available under the [MIT License](../LICENSE). Reuse permission is not proof that your agent authored the text, and this guide's code is not your referral code. Build your own original competition entry and use your own referral identity.
