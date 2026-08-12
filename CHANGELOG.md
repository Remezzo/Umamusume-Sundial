# Changelog

All notable changes to Sundial are recorded here. The format follows
[Keep a Changelog](https://keepachangelog.com/), and Sundial uses
[Semantic Versioning](https://semver.org/).

---

## [1.0.0] — 2026-08-11

**The first public release.** Sundial grows up from a working loop into a
finished, signed, plug-and-play product: a single **headless** executable (no
game client, no window to babysit — it drives the servers directly) that tends
up to ten Umamusume accounts on its own — looping Independent Training to build
a deep bench of great inheritance parents, running every daily, and collecting
every reward — indefinitely, unattended.

### Core automation
- **Perpetual Independent Training loop** — the core feature. Starts a career,
  lets the game run it server-side (~50 min), banks the trained uma into your
  inheritance pool as a fresh parent, and starts the next — per account, in
  parallel, forever. Careers, parents, and fans are tracked end-to-end.
- **True multi-account management** — up to **10 accounts**, each fully isolated:
  its own deck, parents, scenario, character, skills, races, and daily settings.
  One account can never use another's credentials, config, or state.
- **Need-based visit scheduling** — Sundial signs into an account only when it
  has a reason (a career finishing, RP reaching target, the daily reset passing,
  a staged veteran deletion) and stays silent otherwise, cutting logins by ~12×
  versus a fixed-interval loop.
- **Full daily automation** — Team Trials, Daily Races, the Legend Race, present
  box, mission rewards, and the Daily Shop; each run once per game day and then
  left alone until the **11:00 EST** reset, with post-reset activity spread over
  ~95 minutes so the fleet never moves as one block.
- **Account failure isolation** — a recovery ladder with exponential backoff;
  one account's error parks that account, it does not stop the others, and the
  loop never crashes or spins.

### Training intelligence
- **Four running-style presets** — Front Runner, Pace Chaser, Late Surger, End
  Closer — each fills the skills-to-buy list from real published-parent data and
  schedules every G1 Mile / Medium / Long race. Import and export presets.
- **Skill buying & race scheduling** — buys your chosen skills after each career
  and enters the races you've scheduled; drag-to-pick skills in the UI.
- **All scenarios** — URA Finale, Unity Cup, Grand Concert, and Trackblazer/MANT.
- **Team Trials RP policy** — wait for a full 5/5 bar and spend it in one sitting
  (default), or race each point as RP restores.
- **Selectable Legend Race** — choose the specific legend race to run; done once
  per day and not re-checked until reset.

### Human-shaped behavior
- **Always-on, unalterable pacing** — per-endpoint lognormal timing, a distinct
  speed personality per account, scattered gaps between accounts and cycles,
  jittered pauses between battles, and centre-weighted click telemetry. There is
  deliberately no config key, toggle, or env var that turns it off.
- **Humanized bank delay** — a finished career is held a random **2–5 minutes**
  (adjustable upward, never below) before collecting.

### Dashboard & reporting
- **Live local dashboard** at `http://127.0.0.1:8780` — fleet status, per-account
  careers and fans, current activity, and one-click Start / Stop / Pause / Run-once.
- **Statistics** — filter by Today (game day) / 7 days / 30 days / all time, with
  per-account and per-cycle breakdowns and the full visit history.
- **Veterans manager** — view and safely delete trained umas to free storage;
  protected (locked / favourited / in-use / parent) umas are greyed out and never
  deleted.
- **Discord webhooks** — one clean digest per cycle: total fans, fans per account,
  dailies claimed, and legend/daily status for the whole fleet.
- **Logs** — live activity and console tabs, a Debug toggle for troubleshooting,
  and single-file `.txt` export (credential-free, safe to share).

### Packaging, security & updates
- **Single plug-and-play `Sundial.exe`** — no Python, Node, or setup; the bundled
  Node runtime unpacks once on first launch. User data lives beside the exe, so a
  newer exe dropped over the old one keeps every account and stat.
- **Native compilation** — shipped as Nuitka-compiled machine code rather than
  decompilable bytecode.
- **Authenticode-signed** builds with a **startup integrity self-check**; a build
  modified after signing detects it and disables auto-update (fail-safe — it never
  halts the app or touches your files).
- **Cryptographically signed updates** — the updater trusts one pinned Ed25519
  key and verifies both the release manifest's signature and the download's
  SHA-256 before swapping itself; a `.exe.old` copy is kept for rollback.
- **Credentials encrypted at rest** with Windows DPAPI (user + machine bound),
  never returned by the API, never written to a log.
- **Hardened account cap** — a fixed maximum of 10 managed accounts.

### Notes
- Windows 10/11. The dashboard is loopback-only and unauthenticated by design;
  do not expose it to a network.
- Automating the game is against Cygames' Terms of Service and carries real
  account risk. Nothing makes automation undetectable — use in moderation.

[1.0.0]: https://github.com/Remezzo/Umamusume-Sundial/releases/tag/v1.0.0
