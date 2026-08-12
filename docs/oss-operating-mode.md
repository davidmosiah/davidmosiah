# OSS operating mode — 2026-08-04

Canonical rules for the public open-source surface under `davidmosiah`.
This is **not** a product FOCO. It is the **authority / career probe** of the
portfolio cycle (inbound of weight by 2026-09-30), plus hygiene on packages
that already pull.

Related private notes live in the workspace vault when free
(`00-workspace-index/Notes/`). This file is the public, checkable copy.

## Thesis (one line)

**Deepen the few packages that already pull. Never grow the catalog for its own sake.**

Authority arrives via **pull** (issues, PRs, DMs, job/partner inbound) — not via
leaderboard megaphones or Show HN campaigns. Those push surfaces were archived
on 2026-07-06 and only return if real inbound appears.

## Layer model

```
MIT / AGPL connectors & engines  →  free, local-first, npx
            ↑
Commercial convenience           →  setup help, audit, hosted OAuth, x402 utilities
            ↑
Protocol / witness (Delx)        →  always free; never paywall care
```

## Top maintenance surface (SOTA authority wave)

Only these “exist” for proactive work. Everything else is best-effort.
**Agent standard:** MCP packages target **mcp-scorecard ≥90/100** offline; install via public `npx`.

| # | Repo | Why | Scorecard (2026-07-30) |
|---|---|---|---|
| 1 | [`google-health-mcp`](https://github.com/davidmosiah/google-health-mcp) | Discovery hero (~36★); strongest install intent | **100/A** |
| 2 | [`delx-living-body`](https://github.com/davidmosiah/delx-living-body) | Body composition flagship — composes connectors | **100/A** |
| 3 | [`delx-wellness`](https://github.com/davidmosiah/delx-wellness) (+ hermes pack) | Body umbrella / registry / Hermes one-command | hub N/A · hermes CLI pack |
| 4 | [`wellness-nourish`](https://github.com/davidmosiah/wellness-nourish) | Strong npm median; nutrition utility | **100/A** |
| 5 | [`whoop-mcp`](https://github.com/davidmosiah/whoop-mcp) (or wearable with live issues) | Mature connector + real users | **100/A** |
| 6 | [`delx-memory`](https://github.com/davidmosiah/delx-memory) | Local-first agent memory (coord vertical) | **100/A** |
| 7 | [`creative-forge`](https://github.com/davidmosiah/creative-forge) | Public AGPL engine; dogfood in private ops | pytest (not MCP) |
| — | [`mcp-scorecard`](https://github.com/davidmosiah/mcp-scorecard) | The yardstick itself | self-test **100** |

**Hermes community DX (0.3.1+):** generated MCP configs pin `npx -y package@version` for known-good public connectors so agents do not float on accidental breaking latests.

Cadence:

- **Weekly (15–30 min):** external issues/PRs on the top 5
- **Monthly:** refresh public metrics (stars, median npm downloads)
- **Only with inbound:** Show HN, DMs to Anthropic/MCP teams, authority campaigns
- **Never:** new MCP “just because”; polish all 35 READMEs; revive leaderboard push

## Anti-list

- Do not open a 4th product FOCO named “OSS authority”
- Do not clone random OSS apps into the boring-apps factory (use `boring-apps/shared`)
- Do not paywall Protocol/witness
- Do not expose SuperGrok / mediagen as a public OSS or x402 gateway
- Do not treat npm download spikes as human demand (scanners/CI/npx noise)
- Do not re-open BodyPort, Recado, or the Google Health “proof loop experiment”
  as timeboxed FOCOs without a new written criterion

## When a new public repo may ship

All of:

1. Already dogfooded in production (or clear equivalent)
2. Fresh history, secret scan clean, no private ops data
3. One clear flagship slot in a vertical (not “another whoop”)
4. LICENSE + README first-screen value + install path + tests

## Vertical flagships

| Vertical | Flagship (2026-07-30) |
|---|---|
| Body | `google-health-mcp` (discovery) · `delx-living-body` (composition) |
| Reach | `short-video-agent-kit` |
| Coordination | `delx-mcp-server` / Delx Protocol |

## Commercial layer (above OSS)

- Wellness: setup concierge, MCP audit (`mcp-scorecard`), private deploy — see
  delx-wellness `docs/open-source-support.md`
- Agent utilities: Delx Commerce / x402 (timeboxed experiment; separate from FOCOs)
- Scorecard “Pro / certification” stays **frozen** until someone asks for a badge
  or Commerce proves willingness to pay

## Metrics that matter

| Signal | Use |
|---|---|
| Stars on hero repos | Discovery proof |
| External issues/PRs | Builder intent |
| npm **median daily** downloads | Install intent (ignore one-day spikes) |
| Inbound of weight (job, partner, acquisition chat) | Cycle-of-7-years success for this probe |

Snapshot helper: regenerate account metrics with the delx-wellness growth scripts
when available; store dated snapshots next to this note or in the vault
`_data/oss-snapshot.json`.

## Snapshot 2026-08-04 (live)

- GitHub: 48 public repos, ~140★ total, 9 followers
- Hero: google-health-mcp **36★** / 7 forks · hub delx-wellness **22★**
- Live pins: GH `0.7.3` · nourish `0.8.0` · whoop `0.6.0` · garmin `0.7.0` · living-body `0.3.3`
- Proof loop: **1/2 closed** (2026-08-08). No second external report by 2026-08-12. Status: [google-health-mcp/docs/proof-loop-status.md](https://github.com/davidmosiah/google-health-mcp/blob/main/docs/proof-loop-status.md). New reports → [#2](https://github.com/davidmosiah/google-health-mcp/issues/2).
- Authority probe runway: **2026-09-30** — [authority-probe.md](https://github.com/davidmosiah/delx-wellness/blob/main/docs/authority-probe.md)
- Recent community: headless OAuth PR landed (@jumpmanjay); series-contract peer thread on garmin-mcp
- npm: treat **median daily** as signal; ignore one-day spikes (scanners/CI)

## Relationship to product FOCOs

Apple/App Store FOCOs (MannaCup, Avemaris, NinaSom) own product attention.
OSS work is **maintenance + inbound** when those FOCOs are blocked (review
queues, etc.). Capacity free ≠ permission to invent a new vertical.
