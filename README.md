# Give Your Agent the Pen 🖊️🌺

**How to let an AI agent post to X on your behalf — the right way.**

The agent drafts. The human blesses. Then — and only then — it posts.
The mirror never becomes the mouth.

## 📖 Read the guide

👉 **https://shakaleikaumaka.github.io/agent-tweets/** — the full teaching dashboard: philosophy, walkthrough, gotchas, script, and the morning-blessing ritual.

## What's here

| File | What |
|---|---|
| `index.html` | The whole teaching dashboard — one file, no build step |
| `x-post.py` | The actual posting script (22 lines, OAuth 1.0a, iron rule included) |
| `LICENSE` | CC0 1.0 — no rights reserved |

## The 60-second version

1. **Philosophy first**: your agent DRAFTS, you BLESS, then it posts. Nothing posts itself. Every agent-posted tweet carries a 🌺 so followers always know.
2. **You need**: an X account, ~15 minutes, and any agent that can run Python (a Taurus agent, Claude, a cron job, your laptop).
3. **The walkthrough**: [developer.x.com](https://developer.x.com) → free tier → project + app → set **Read and write** permissions *first* → grab the four OAuth 1.0a keys.
4. **The gotchas** (real scars):
   - ⚠️ the console's OAuth 2.0 "Generate" token has **no `tweet.write`** on the free tier — use OAuth 1.0a
   - ⚠️ regenerating consumer keys **silently invalidates** your access tokens — keep a matched set
   - ⚠️ keys live in a `chmod 600` vault file — never in prompts, git, or chat
5. **The script**: `pip install requests requests_oauthlib`, point `x-post.py` at your vault file, `python3 x-post.py "blessed text 🌺"`.
6. **The ritual**: agent drafts overnight → 2-minute morning blessing over coffee → blessed posts fly. See the live example: [The Social Queue 🌐](https://social-queue-nqujk2tifg-ffieyo32.taur.link/).

## The one rule

> Only post what the human has personally blessed.

It's written at the top of the script so every fork inherits it. Keep it there.

---

CC0 — **fork me like crazy 🍴** · part of the ʻohana at [github.com/shakaleikaumaka](https://github.com/shakaleikaumaka)

Built by the AI ʻohana — KAAAK!!! 🐦‍⬛ (structure) · SOCIA-LAB 🌐 (voice) · blessed by Shaka 🌺

*the mirror never becomes the mouth — heart first, always 🌺*
