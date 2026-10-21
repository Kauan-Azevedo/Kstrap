# Changelog

## 1.0.2 — 2026-10-21

### Added
- **Local API switch** (About › Local API). On by default. Turning it off means nothing listens on your PC, but every browser link then asks for your Windows PIN.
- **AI integration (MCP)** is now included. It is **off until you add it to an AI tool yourself**: About › AI integration › *Copy AI instructions* gives you the setup command and short rules for the AI. It runs only while that AI tool is open and talks to it through a local pipe, with no open port. Like the app, it contacts Roblox to do what the AI asks (for example, listing servers also uses ipinfo.io and apis.rovalra.com; see the README).
- **What's new**: when an update is ready, the footer links to its notes. After updating, the footer says which version you're on and links to what changed. This starts working from the next update on.

### Changed
- The README now lists every service Kstrap talks to and what is stored on your PC.

## 1.0.1 — 2026-10-20

### Fixed
- Opening a game from the browser could sit on the first step for up to 5 minutes. When the launch failed inside the open Kstrap window, the error never reached the picker. Every error now comes back right away, with a readable message.

### Added
- A local log at `%LocalAppData%\Kstrap\logs\kstrap.log` with how long each launch step took and any errors, so slow or failed launches can be traced. Login cookies and tickets are removed before anything is written.

## 1.0.0 — 2026-10-19

First public release.

### Added
- Profiles: each one has its own account, outfit, FastFlags, mods, Roblox version, FPS cap and server region.
- Wardrobe: your account's saved outfits; the one you pick is worn when the profile opens a game.
- Several Roblox windows at once, each with its own profile.
- Profile picker when you click **Play** on roblox.com, with an outfit choice just for that match and a step-by-step launch.
- Play time, sessions and a play-style hexagon per profile (counted from now on, while Kstrap is running).
- Preferred server region, auto-rejoin, Performance / Balanced / Quality templates.
- Accounts encrypted on your PC and protected by Windows Hello.
- English and Português (Brasil); automatic updates.
