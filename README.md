<div align="center">

<img src="web/sundial.png" alt="Sundial" width="120" />

# Sundial

### Independent Training that never stops. On every account. Forever.

**Sundial is a headless bot that runs the game's own Independent Training on a perpetual loop — training uma after uma into your inheritance pool — start a career, bank the parent, buy the skills, run the races, start the next — across up to twelve accounts in parallel, unattended, indefinitely.** No game client, no window to babysit: it drives the servers directly and builds you a deeper, stronger bench of parents while you do anything else.

[![Download](https://img.shields.io/badge/Download-Sundial.exe-D4A017?style=for-the-badge)](https://github.com/Remezzo/Umamusume-Sundial/releases/latest)
&nbsp;
[![Discord](https://img.shields.io/badge/Discord-Join_the_Icarus_hub-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/wpbd3hTBDc)

![Platform](https://img.shields.io/badge/platform-Windows-0078D6)
![Version](https://img.shields.io/badge/release-1.0.16-D4A017)
![Signed updates](https://img.shields.io/badge/updates-Ed25519_signed-1f7a4d)
![License](https://img.shields.io/badge/license-Proprietary-c02626)

</div>

---

## Independent Training is the whole point

Every strong uma you train is only as good as the **parents** it inherits from — their factors, their aptitudes, their sparks. And the most reliable way to build a deep bench of great parents is **Independent Training**, the game's own idle career mode: run a career, bank the trained uma into your inheritance pool, and you've got another parent to breed from. Run it again. And again. The deeper and better your pool, the stronger every future uma starts.

The catch: a single career takes about **50 minutes**, and doing it by hand means babysitting every one — start it, wait, collect it, pick the factors, remember the skills, enter the races — then do the entire dance again, **one account at a time.** Multiply that by a roster and it stops being a game and starts being a second job.

**Sundial turns that grind into a loop that runs itself** — a parent factory that never clocks out.

---

## 🔁 The Independent Training engine

This is the heart of Sundial. Point it at your accounts and it runs this cycle, **on every account at once, forever:**

```
   ┌──────────────────────────────────────────────────────────┐
   │                                                          ▼
   │   START a career  ──►  the game runs it (~50 min)  ──►  BANK it
   │        ▲                                                  │
   │        │                                                  ▼
   │        │                                    a new trained parent
   │        │                                                  │
   │        │                                                  ▼
   │        │                                    BUY your skills · RUN your races
   │        │                                                  │
   └────────┴──────────────  hold 2–5 min (humanized)  ◄───────┘
```

What that means in practice:

- **It banks a fresh parent, career after career.** Sundial opens a career, lets the game's servers run it to completion, then banks the trained uma into your inheritance pool and immediately queues the next one. No babysitting, no timers, no "did I collect that one?"
- **It buys the skills you want.** After each career it spends the skill points on your skills-to-buy list — or on a running-style preset that fills the list from real published-parent data — so your parents carry the skill sparks worth inheriting.
- **It runs the races you schedule.** Your G1 mile/medium/long schedule (or a preset's) is entered automatically, so each career finishes as a richer parent — better aptitudes, more fans banked along the way.
- **It figures out the setup on its own.** No recorded setup? Sundial auto-builds a valid start from the account itself — trainee, deck, parents, succession, scenario — and if a saved parent no longer exists it picks a working replacement and keeps going instead of stalling.
- **It runs your whole roster in parallel.** While one account's career is cooking on the game's servers, Sundial is banking another's and starting a third. Twelve accounts don't take twelve times as long — they overlap. Careers come first, too: an account with a career to bank or start is served before accounts that only owe dailies, because an uncollected career leaves that account idle while dailies keep until the reset.
- **It never stops and it never crashes the loop.** One account hitting a snag (out of TP, storage full, a career you left half-played) parks *that* account with a clear reason and keeps the rest looping — and no single stuck account can hog the rotation and starve the others. The bot is built to run for days.
- **It keeps working when the game changes.** New banner characters, a new game version, even a change to what a career costs: Sundial reads the game's own data, notices the difference, and adapts on its own — no reinstall, no waiting for an update. Game data refreshes over the air, verified against a signed hash before a single byte is trusted.
- **It works in every scenario** — URA Finale, Unity Cup, Grand Concert, and Trackblazer/MANT.

> In continuous testing, a four-account fleet banked a **fresh trained parent roughly every 50 minutes per account, completely unattended** — careers rolling over one after another, around the clock, with nobody at the keyboard.

**That's the sell: you set it up once, press Start, and your inheritance pool builds itself indefinitely.**

---

## And it handles everything else, too

The training loop is the star — but a real account needs its dailies done and its rewards collected, so Sundial does all of that in the same rounds:

| | |
|---|---|
| 🎴 **Up to 12 accounts, fully isolated** | Each account is its own world — deck, parents, scenario, skills, races, dailies. No cross-contamination, ever. |
| 🏆 **Every daily, once each** | Team Trials, Daily Races, your pick of Legend Race, present box, missions, and the shop — all reset-aware, done once per game day. Pick each account's Daily Race — Moonlight Sho for Monies, Jupiter Cup for Support Points — and the difficulty to run it at. |
| 🍨 **Parfaits, if you want them** | Optional per account: spend a Pleasing Parfait before each Team Trials battle, Daily Race and Legend Race so runners go in with Great mood. Stock-aware, shows your balance, and never spends one on a mood that's already Great. Off by default. |
| 🗓️ **A week you draw yourself** | Give each day its own run windows — evenings on weekdays, all day at the weekend, as many per day as you like — and keep the whole week under a name to put back later. Sundial starts and stops the loop on the window edges and stays quiet outside them. |
| ⏰ **Visits only when there's a reason** | No mindless polling. Sundial signs in when a career finishes, RP fills, or the reset passes — and sits silent otherwise. ~12× fewer logins than a naive loop. |
| 🧠 **One-click running-style presets** | Front Runner, Pace Chaser, Late Surger, End Closer — each fills your skills-to-buy list and schedules every G1 mile/medium/long automatically. Import and export them. |
| 🥇 **Run every G1 it's suited for** | Optional per account: extend the auto-scheduled G1s across all three years instead of just the first two. A legacy parent is judged on its G1 wins, so for parent farming this is the shape you want. Aptitude-gated, never clashes with a compulsory race. |
| 🧯 **Clears its own blockers** | A career left half-played in the game blocks Independent Training entirely — Sundial names it and, if you opt in per account, discards it and starts fresh. Off by default: it deletes a real career and can't be undone. |
| 👤 **Acts human** | Per-account timing personalities, jitter on every action, and the randomized 2–5 minute banking hold — always on, no off switch. |
| 🧹 **Veterans manager** | View and safely delete trained umas to free storage, so a full box never stalls training — listed newest-first so fan-race extras sit at the top, with Score and Name a click away. Protected umas are greyed out and never touched. |
| 📊 **Live local dashboard** | Fleet status, per-account careers and fans, filterable statistics, and a full visit history — all at `127.0.0.1:8780`. **Ctrl-K** jumps straight to any account, setting or page. |
| 🔔 **Discord digests** | One clean webhook per cycle: total fans, fans per account, dailies claimed, legend/daily status. A glance, not a firehose. |
| 🔄 **Safe self-update** | Cryptographically-signed updates — Sundial only ever installs a build signed by the real publisher's key. |

---

## Quick start

> **Download → double-click → press Start.** No Python, no Node, no setup.

1. **Grab [`Sundial.exe`](https://github.com/Remezzo/Umamusume-Sundial/releases/latest)** and drop it in a folder of its own.
2. **Double-click it.** A console window opens (that window *is* the bot — closing it stops everything) and the dashboard opens at **`http://127.0.0.1:8780`**.
3. **Add your accounts** under **Accounts → Add account** — a label and each account's Data Link password.
4. **Pick a preset** to fill skills and races in one click, then **turn on Independent Training** for the account.
5. **Press Start** and watch the careers bank and the fan totals climb.

Closing the browser tab changes nothing — reopen `127.0.0.1:8780` any time. Your accounts, settings, and stats live *beside* the exe, so dropping a newer `Sundial.exe` over the old one keeps everything.

**Requirements:** Windows 10/11. That's it.

---

## Built to be trusted

Sundial is engineered as a finished product, not a script dump:

- **Native-compiled** with Nuitka — the shipped binary is machine code, not lift-and-decompile bytecode.
- **Authenticode-signed** and **integrity-checked at startup** — a build modified after signing detects it and refuses to auto-update.
- **Signed updates** — the updater trusts one pinned Ed25519 key and verifies both the manifest signature and the download's hash before ever swapping itself. A tampered or unofficial "update" is rejected, not installed.
- **Your credentials never leave your machine** — Data Link passwords are encrypted at rest with Windows DPAPI (user + machine bound) and are never returned by the API or written to a log.
- **Local-only by design** — the dashboard binds to loopback and does nothing over the network except talk to the game and check for its own updates. It also **only answers its own pages**: a request from any other site, or aimed at Sundial through another domain, is refused rather than acted on.
- **Honest about what it's doing** — the dashboard only reports a career as running once the game has actually confirmed the start, progress streams live while long work happens rather than arriving in one burst, and every refusal names its real cause instead of guessing. When Sundial doesn't know something, it says so.

---

## Part of the Icarus Suite

Sundial is one tool in a family of Umamusume utilities by **Icarus Network**. Join the hub for releases, help, and the wider toolset:

<div align="center">

### [→ discord.gg/wpbd3hTBDc](https://discord.gg/wpbd3hTBDc)

</div>

---

## FAQ

**How many parents can it produce?**
As many as your accounts can train — Independent Training loops continuously, so a fresh parent lands in your inheritance pool at the end of every career, for as long as you leave it running. Throughput scales with your roster: more accounts train in parallel, and each banks career after career (fans and all) on its own.

**Is this safe for my account?**
Automating the game is against Cygames' Terms of Service and carries real, inherent account risk. Sundial's always-on human-shaped pacing is designed to make its activity look natural, but **nothing makes automation undetectable.** Use it in moderation, at your own risk.

**Does it need me to leave the game open?**
No. Sundial drives the game's own servers directly and headlessly — the game client stays closed. (The game and Sundial share one device seat, so playing an account yourself while the loop runs will sign the other out; pause Sundial first if you want to play.)

**A career won't start / a picker looks empty.**
Empty pickers just mean that account hasn't been visited yet — open the account and press **Visit now** to sign in and load its decks, veterans, friends and races.

A start refusal is always **named** in the log rather than left as a mystery. By far the most common cause is a **career you left half-played in the game**: the game allows one career at a time, so it blocks Independent Training completely. Sundial tells you which account, and you either finish or quit that career in the game — or turn on *Delete the unfinished career* for that account and let Sundial clear it. Other named causes: out of TP, veteran storage full, a missing parent, or an event window that has closed. The loop retries on its own, and the in-app **Help** page covers the rest.

**Where do my accounts and settings live?**
In folders right next to `Sundial.exe`. Back up that folder and you've backed up everything. Update by dropping a new exe on top — your data is untouched.

**Windows Defender flagged or deleted Sundial.**
Since 1.0.16 Sundial unpacks itself **once**, into `%LOCALAPPDATA%\Icarus Network\Sundial\<version>`, and reuses that folder — older builds wrote a brand-new copy to `%TEMP%` on every launch, which is exactly the pattern Defender's heuristics flag ("Error 225 … contains a virus or potentially unwanted software"). If Defender still objects, exclude that one folder. Sundial is signed with its own certificate rather than one bought from a public authority, so Windows may still call it an unknown publisher on first run; that is expected, and the build verifies its own signature at startup.

---

## Disclaimer & license

Sundial is an independent, unofficial tool. It is **not affiliated with, endorsed by, or sponsored by Cygames, Inc.** "Umamusume: Pretty Derby" and all related names and marks are the property of their respective owners.

Sundial is **proprietary software** — see [LICENSE](LICENSE). You may download and run the official build for personal use; you may **not** copy, modify, redistribute, or reuse it or its code. All rights reserved © 2026 Remezzo / Icarus Network.

