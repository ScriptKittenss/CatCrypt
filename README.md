<div align="center">

# 🐱 CatCrypt

**Licensing & authentication backend for software products.**

HWID machine binding · License keys · Live operator dashboard · SDKs for Python, C# & C++

[![Live](https://img.shields.io/badge/Live-auth.script--kittens.com-brightgreen)](https://auth.script-kittens.com)
[![Discord](https://img.shields.io/badge/Discord-Script_Kittens-5865F2)](https://discord.gg/wYZeuJQNCy)
[![License](https://img.shields.io/badge/License-Proprietary-red)](https://auth.script-kittens.com)

[Live Site](https://auth.script-kittens.com) · [Discord](https://discord.gg/wYZeuJQNCy) · [Pricing](#pricing) · [SDKs](#sdks)

</div>

---

![CatCrypt landing page](docs/landing.jpg)

## What is CatCrypt?

CatCrypt protects your software with account-based licensing. Your users log in, their machine gets bound by HWID, and every session, key, and file download is checked against your rules — all from one live dashboard.

Built for developers who sell software and are tired of shared logins, leaked keys, and cracked copies.

## How it works

| Step | What happens |
| --- | --- |
| **1. Create your app** | Add your product in the dashboard and get your App ID. |
| **2. Integrate the SDK** | Drop the SDK into your app — login, register, validate, done. |
| **3. Sell keys, stay in control** | Generate license keys, watch live sessions, ban abusers, push updates — all live. |

## Features

- 🔐 **HWID machine binding** — each account locks to a trusted machine. Shared accounts stop working.
- 🎫 **License keys** — generate, track, redeem, and delete keys (free / starter / pro / lifetime).
- 👥 **Users** — plans, expiry, HWID reset, ban/unban, API keys, and per-user session limits.
- 🟢 **Live sessions** — real-time view of active logins with instant revocation.
- 📁 **Runtime Vault** — serve protected files to authenticated, entitled users only.
- ⚙️ **Variables** — push runtime configuration to your apps from the dashboard, no rebuild needed.
- 🚫 **Blacklist** — block HWIDs, IPs, or usernames, per app or platform-wide.
- 👨‍👩‍👧 **Teams** — invite admins and viewers by email with distinct permissions.
- 📜 **Event logs** — full audit trail of logins, bans, redemptions, and changes.
- 🤖 **Cat Agent** — an AI assistant in the dashboard that answers questions from your live data and runs operator actions for you (users, keys, sessions, variables, blacklist, events).
- 📡 **Real-time dashboard** — stats, sessions, and logs update live without refreshing.
- 📱 **Mobile-ready** — the landing page and dashboard work beautifully on phones too.

## Pricing

| Plan | Price | What's included |
| --- | --- | --- |
| **Free** | **$0** | Core licensing, 1 app, community support |
| **Starter** | **$1** | More apps, Runtime Vault file hosting |
| **Pro** | **$2** | Everything — all features included |

## SDKs

Integrate CatCrypt into your app in minutes. All SDKs have full feature parity — login, register, redeem, validate, variables, file download, HWID lock, and `is_paid` check.

| Language | Repository |
| --- | --- |
| Python | [CatCrypt-Python-Example](https://github.com/ScriptKittenss/CatCrypt-Python-Example) |
| C# | [CatCrypt-CSharp-Example](https://github.com/ScriptKittenss/CatCrypt-CSharp-Example) |
| C++ | [CatCrypt-CPP-Example](https://github.com/ScriptKittenss/CatCrypt-CPP-Example) |

> **Security note:** never put your app secret in client code. The secret is server-side only.

## Architecture

```
Your app (SDK) ──HTTPS──► CatCrypt ──► MongoDB
                              │
                              ├── Live dashboard (real-time SSE)
                              ├── Cat Agent (AI operator)
                              └── Runtime Vault (protected files)
```

## FAQ

**Can I try it for free?**
Yes — the Free plan is $0 and includes core licensing for 1 app.

**Do my users need anything installed?**
No. They log in through your app with the SDK — no extra software.

**What if someone shares their account?**
HWID binding ties each account to one machine. A shared login on a new machine gets blocked, and you can see it in the event log.

**Can I sell CatCrypt licenses to my own customers?**
Yes — that's what the Starter and Pro plans are for. Generate keys, hand them out, and manage everything from the dashboard.

## Get started

1. Go to [auth.script-kittens.com](https://auth.script-kittens.com)
2. Create an account and your first app
3. Grab the SDK for your language and integrate it

Questions? Join the [Discord](https://discord.gg/wYZeuJQNCy) and open a ticket.

---

<div align="center">

**CatCrypt** — by [Script Kittens](https://discord.gg/wYZeuJQNCy)

*Private Session* イメージ.

</div>
