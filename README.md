<div align="center">

<img src="icarus.png" alt="Icarus" width="120" />

# Sundial

### Independent Training that never stops. On every account. Forever.

**Sundial runs the game's own Independent Training on a perpetual loop — career after career, parent after parent — across up to twelve accounts at once, unattended, for as long as you leave it on.** It starts the career, lets it run, buys every skill point's worth of skills, banks the trained uma into your inheritance pool and starts the next one. It also clears every daily, claims every reward, runs your clubs and keeps your follow list tidy. No game client, no window to babysit: it talks to the game's servers directly, so your PC is free and your bench keeps growing.

[![Download](https://img.shields.io/badge/Download-Sundial.exe-D4A017?style=for-the-badge)](https://github.com/Remezzo/Umamusume-Sundial/releases/latest)
&nbsp;
[![Discord](https://img.shields.io/badge/Discord-Join_the_Icarus_hub-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/wpbd3hTBDc)

![Platform](https://img.shields.io/badge/platform-Windows-0078D6)
![Version](https://img.shields.io/badge/release-1.2-D4A017)
![Signed updates](https://img.shields.io/badge/updates-Ed25519_signed-1f7a4d)
![License](https://img.shields.io/badge/license-Proprietary-c02626)

</div>

---

## Independent Training is the whole point

Every strong uma you train is only as good as the **parents** it inherits from — their factors, their aptitudes, their sparks. The most reliable way to build a deep bench of great parents is **Independent Training**, the game's own idle career mode: run a career, bank the trained uma into your inheritance pool, and you have another parent to breed from. Run it again. And again. The deeper and better your pool, the stronger every future uma starts.

The catch: one career takes about **50 minutes**, and by hand you babysit every one — start it, wait, buy the skills, collect it — then do the whole dance again, **one account at a time.** Across a roster it stops being a game and becomes a second job.

**Sundial turns that grind into a loop that runs itself** — a parent factory that never clocks out.

---

## The Independent Training engine

This is the heart of Sundial. Point it at your accounts and it runs this cycle, **on every account at once, forever:**

```
   ┌───────────────────────────────────────────────────────────────┐
   │                                                               ▼
   │   START a career  ──►  the game runs it (~50 min)  ──►  hold 2–5 min (humanized)
   │        ▲               racing the schedule you set               │
   │        │                                                          ▼
   │        │                                              BUY skills with every point
   │        │                                                          │
   │        │                                                          ▼
   │        │                                                       BANK it
   │        │                                                          │
   │        │                                                          ▼
   └────────┴───────────────────────────────────────── a new trained parent
```

What that means in practice:

- **It banks a fresh parent, career after career.** Sundial opens a career, lets the game's servers run it, waits a human-looking moment once it finishes, then buys the skills and banks the trained uma into your inheritance pool — and the next career starts on the same visit. No timers to watch, no "did I collect that one?"
- **It never wastes a skill point.** Your skills-to-buy list gets the budget first, in your order — from the whole shop, your trainee's own potential skills included, hinted or not. A list entry marked ○ buys the ○, never the ◎ upgrade; three-step gold skills are bought with their prerequisites. Whatever your list can't use goes to the best remaining skills, ◎ upgrades last, so **no career is ever banked with points left on it.** When the game refuses a skill, the career report says which and why.
- **It runs the races you schedule — and farms fans on its own.** Your G1 mile/medium/long schedule (or a preset's) goes into every career. Turn on **fan farming** and Sundial adds the aptitude-suited G1s a career needs to clear its fan targets, around your picks and the trainee's objectives. The Racing card tells you exactly how many races the last career entered and how many the next one will.
- **It builds the setup on its own.** No recorded setup? Sundial builds a valid start from the account itself — trainee, deck, parents, succession and scenario. If your chosen parents were deleted, the career still starts on your best available pair (and says which). A combination the game never accepts — a trainee with a support card of her own character — is flagged on the account's page before a single request is sent.
- **It keeps the friend card you chose.** Pick a support card to borrow and Sundial hunts for it at every start — re-rolling the friend list until someone offers it, taking the best copy from any lender, and waiting a few minutes before looking again. It never swaps in a different card. With no pick, it borrows an SSR at max limit break or nothing.
- **It never deletes a parent you're using.** The Racing Uma, your chosen parents and backups, a recorded setup's parents and the pair the last career actually used are all fenced off — from the Veterans page, the delete queue and the box-full auto-delete alike.
- **It stops when you tell it to.** Set **Careers to run** or **Stop at fans** per account and Independent Training switches itself off when the target is met — however the careers were banked.
- **It runs your whole roster in parallel.** While one account's career runs on the game's servers, Sundial banks another's and starts a third. Twelve accounts don't take twelve times as long — they overlap. An account with a career to bank or start is served first, because an uncollected career leaves that account idle.
- **It never stops, and one bad account never stops the rest.** Out of TP, a full veteran box, a career you left half-played in the game: that account parks with a plain reason and the others keep looping. No single stuck account can hog the rotation. It's built to run for days.
- **It keeps working when the game changes.** New banner characters, a new game version, a change to what a career costs: Sundial reads the game's own data, notices, and adapts — no reinstall. Game data refreshes over the air, checked against a signed hash before a byte of it is used.
- **It works in every scenario** — URA Finale, Unity Cup, Grand Concert, and Trackblazer.

> In continuous testing, a four-account fleet banked a **fresh trained parent roughly every 50 minutes per account, completely unattended** — careers rolling over one after another, around the clock, with nobody at the keyboard.

**That's the sell: set it up once, press Start, and your inheritance pool builds itself.**

---

## And it handles everything else, too

The training loop is the star — but a real account needs its dailies done, its rewards claimed and its club looked after. Sundial does all of it in the same rounds:

| | |
|---|---|
| **Up to 12 accounts, fully isolated** | Each account is its own world — deck, parents, scenario, skills, races, dailies. Nothing leaks between them. |
| **Every daily, once each** | Team Trials, Daily Races, your pick of Legend Race, the present box, missions and the shop — reset-aware, done once per game day. Choose each account's Daily Race (Moonlight Sho for Monies, Jupiter Cup for Support Points) and its difficulty. |
| **Team Trials, handled** | The game's Auto-Select picks the strongest veteran for every slot, one per character, each on her best style — now, or every day before Team Trials. Each account wears its Team Trials rank as a badge. |
| **Parfaits, if you want them** | Optional per account: a Pleasing Parfait before each Team Trials battle, Daily Race and Legend Race, so runners go in with Great mood. Stock-aware, and never spent on a mood that's already Great. |
| **Inventory, with selling and vouchers** | See every item an account holds, sell what you don't need for Monies, and redeem trainee vouchers — the game's own confirmation, one click. |
| **Clubs, run for you** | Found a club, edit it from the leader account, invite trainers by ID, remove members, accept invites, donate to members' requests and request shoes and sashes — by hand, or automatically within the game's daily limits. |
| **Your follow list, managed** | Follow trainers by ID, see followers and follows with their last login, and clear out inactive ones in one run — mutuals protected, at a human pace. |
| **A week you draw yourself** | Give each day its own run windows, add breaks, and keep the week under a name. Sundial starts and stops the loop on the window edges — and when you press Stop inside a window, it stays stopped until the next one. |
| **Visits only when there's a reason** | No mindless polling. Sundial signs in when a career finishes, RP fills or the reset passes, and sits silent otherwise — about twelve times fewer logins than a naive loop. |
| **Acts human — always** | Per-account speed personalities, jitter on every action, a 2–5 minute hold before each bank, and a natural pause after a daily becomes ready before it's run — about 20 minutes, never the same twice. There is no off switch, by design. |
| **Skill lists by the group** | Add a whole category at once — every green, every acceleration skill, every ◎ upgrade, everything that only fires on dirt — to your buy list or your never-buy list. Twenty-three groups, read from the game's own effect data, with **Undo** for all of it. |
| **One-click running-style presets** | Front Runner, Pace Chaser, Late Surger, End Closer — each fills your skills-to-buy list and schedules every suited G1. Save your own, import and export them. |
| **Decks recommended from your cards** | **Recommend from card data** builds a deck from the supports the account actually owns — portraits, rarity and limit break shown — and saves it as a new in-game deck in one click. |
| **Pickers that show the real cards** | Deck, friend card, trainee and parents show the game's own art with type, rarity and limit break. Search, sort and filter trainees by aptitude, friend cards by type and lender, parents by any spark in the game with a minimum star count. |
| **Veterans manager** | Browse and safely delete trained umas to free storage, with a 0–100 keep score that flags the weak and shields your best. Parents in use are never touched. |
| **Live local dashboard** | Fleet status, careers and fans per account, filterable statistics and a full visit history. **Ctrl-K** jumps to any account, setting or page; settings save as you change them. |
| **Help that answers** | Every error code in the game's own words, a full reference of what each feature does, and a glossary — built into the app. **Settings › Data & health** checks your game data, version, Steam sign-in, loop and webhooks at a glance, and **Copy diagnostics** makes a bug report that never carries your Windows user name. |
| **Webhooks, plural** | Send cycle digests to as many endpoints as you like. Career posts carry the trainee's portrait, all six cards (your five and the borrowed one), the sparks it produced grouped by type, the skills it bought, plus stats, grade and fans — every figure one the game reported, or left out. |
| **Open it from anywhere — on your terms** | **Settings › Running › Remote access** lets the dashboard answer at a hostname you choose, for a tunnel you run yourself (Cloudflare Tunnel, Tailscale). Everything else is still refused. |
| **Looks after itself** | **Restart** from Settings, a **dashboard port** you can change (and if another program holds it, Sundial simply takes the next free one), and signed updates it checks for on its own every six hours. |

---

## Quick start

> **Download → double-click → sign in with Steam → press Start.** No Python, no Node, no setup.

1. **Grab [`Sundial.exe`](https://github.com/Remezzo/Umamusume-Sundial/releases/latest)** and drop it in a folder of its own.
2. **Double-click it.** A console window opens — that window *is* the bot; closing it stops everything — and the dashboard opens at **`http://127.0.0.1:8780`**.
3. **Sign in with Steam, once** — the Steam account that owns Umamusume (Global). Enter the Steam Guard code if asked. Sundial keeps an encrypted session so it signs in unattended from then on.
4. **Add your accounts** under **Accounts → Add account** — a label, the Trainer ID and each account's Data Link password. Several at once? **Add several** takes one per line.
5. **Pick a preset** to fill skills and races in one click, then **turn on Independent Training** for the account.
6. **Press Start** and watch the careers bank and the fan totals climb.

Closing the browser tab changes nothing — reopen `127.0.0.1:8780` any time. Your accounts, settings and stats live *beside* the exe, so dropping a newer `Sundial.exe` over the old one keeps everything.

**Requirements:** Windows 10/11 and a Steam account that owns Umamusume: Pretty Derby. That's it.

---

## Built to be trusted

Sundial is engineered as a finished product, not a script dump:

- **The shipped binary is machine code with no Python source or bytecode inside, not lift-and-decompile bytecode.
- **Authenticode-signed** and **integrity-checked at startup** — a build whose files were changed after it was built refuses to start, and one whose signature doesn't check out never auto-updates.
- **Signed updates** — the updater trusts one pinned Ed25519 key and checks both the manifest's signature and the download's hash before it swaps anything. A tampered or unofficial "update" is rejected, not installed.
- **Your credentials never leave your machine** — Data Link passwords and your Steam session are encrypted with Windows DPAPI, bound to your user and machine, and never returned by the API or written to a log.
- **Local-only by default** — the dashboard answers only its own pages on your PC. A request from any other website, another program's page or an unlisted address is refused before it does anything. Remote access exists only if you switch it on, for the addresses you list.
- **Steam handled with care** — one Steam account at a time; a passing network or Steam hiccup never throws away your saved sign-in; a refused Steam Guard code is called out as refused, not "needed" again.
- **Honest about what it's doing** — a career shows as running only once the game has confirmed the start, progress streams live, and every refusal names its real cause. When Sundial doesn't know something, it says so.
- **Hard limits that don't bend** — one Sundial per PC, at most 12 accounts, and the shipped human-scale delays, all sealed into the build. Nothing in `config.json`, the environment or the command line changes them; try, and Sundial refuses to run and tells you why.

---

## Part of the Icarus Suite

Sundial is one tool in a family of Umamusume utilities by **Icarus**. Join the hub for releases, help and the wider toolset:

<div align="center">

### [→ discord.gg/wpbd3hTBDc](https://discord.gg/wpbd3hTBDc)

</div>

---

## FAQ

**How many parents can it produce?**
As many as your accounts can train. Independent Training loops continuously, so a fresh parent lands in your inheritance pool at the end of every career, for as long as you leave it running. More accounts train in parallel, and each banks career after career, fans and all.

**Is this safe for my account?**
Automating the game is against Cygames' Terms of Service and carries real, inherent account risk. Sundial's always-on, human-shaped pacing is designed to make its activity look natural, but **nothing makes automation undetectable.** Use it in moderation, at your own risk.

**Does it need me to leave the game open?**
No. Sundial talks to the game's servers directly — the game client stays closed. (The game and Sundial share one device seat, so playing an account yourself while the loop runs will sign the other out; press Stop first if you want to play.)

**A career won't start / a picker looks empty.**
An empty picker just means that account hasn't been visited yet — open the account and press **Visit now** to load its decks, veterans, friends and races.

A start refusal is always **named** in the log. By far the most common cause is a **career you left half-played in the game**: the game allows one career at a time, so it blocks Independent Training. Sundial tells you which account; finish or quit that career in the game, or turn on *Delete the unfinished career* for the account and let Sundial clear it. Other named causes: out of TP, a full veteran box, an event window that has closed, the friend card you chose not on offer right now, or a support card the game won't allow with that trainee. The loop retries on its own, and the in-app **Help** covers the rest.

**Can I open the dashboard from my phone?**
Yes, through a tunnel you run yourself (Cloudflare Tunnel, Tailscale): add its hostname under **Settings › Running › Remote access**. Sundial has no password of its own, so protect the tunnel first — Cloudflare Access, for example.

**Where do my accounts and settings live?**
In folders right next to `Sundial.exe`. Back up that folder and you've backed up everything. Update by dropping a new exe on top — your data is untouched.

**Windows Defender flagged or deleted Sundial.**
Sundial unpacks itself **once**, into `%LOCALAPPDATA%\Icarus\Sundial\<version>`, and reuses that folder. If Defender objects, exclude that one folder. Sundial is signed with its own certificate rather than one bought from a public authority, so Windows may call it an unknown publisher on first run; that is expected, and the build checks its own signature at startup.

---

## Disclaimer & license

Sundial is an independent, unofficial tool. It is **not affiliated with, endorsed by, or sponsored by Cygames, Inc.** "Umamusume: Pretty Derby" and all related names and marks are the property of their respective owners.

Sundial is **proprietary software** — see [LICENSE](LICENSE). You may download and run the official build for personal use; you may **not** copy, modify, redistribute, or reuse it or its code. All rights reserved © 2026 Remezzo / Icarus.
