# Changelog

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
