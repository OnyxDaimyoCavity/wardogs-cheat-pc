<div align="center" id="top">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0E1410,55:3A2F1C,100:E0B25C&height=215&section=header&text=WARDOGS&fontSize=64&fontColor=ffffff&fontAlignY=30&desc=PC%20%C2%B7%20tactical%20overlay%20%C2%B7%20recon%20%C2%B7%20fire%20control&descAlignY=54&descSize=15&descColor=E0B25C&animation=fadeIn" width="100%" alt="WARDOGS">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=3000&pause=900&color=E0B25C&center=true&vCenter=true&width=830&lines=One+hundred+players.+Three+teams.+One+control+zone.;Read+the+zone+before+your+squad+walks+into+it.;Weak+spots+on+armour%2C+not+on+the+silhouette.;Silent+correction+%E2%80%94+the+camera+never+snaps.;External+build.+No+driver%2C+no+injection." alt="typing">

<br><br>

<a href="https://github.com/OnyxDaimyoCavity/wardogs-cheat-pc/releases/latest">
  <img height="70" alt="Download WARDOGS overlay v1.0.0 for Windows" src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD%20v1.0.0%20%C2%B7%20WARDOGS%20OVERLAY-E0B25C?style=for-the-badge&labelColor=141414&logo=windows&logoColor=white">
</a>

<br><br>

![build](https://img.shields.io/badge/build-Season%203-9DB24B?style=for-the-badge&labelColor=141414)
![platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011-7C8A96?style=for-the-badge&labelColor=141414)
![eac](https://img.shields.io/badge/EAC-external%20%C2%B7%20no%20driver-4CAF50?style=for-the-badge&labelColor=141414)
![status](https://img.shields.io/badge/status-undetected%20as%20of%202026--11--23-C0502B?style=for-the-badge&labelColor=141414)

<br>

[![releases](https://img.shields.io/badge/all%20releases-1F1F1F?style=for-the-badge&logo=github&logoColor=white)](../../releases)
[![bugs](https://img.shields.io/badge/%F0%9F%90%9E%20report%20a%20bug-1F1F1F?style=for-the-badge)](../../issues/new?template=bug.yml)
[![wiki](https://img.shields.io/badge/%F0%9F%93%96%20wiki-1F1F1F?style=for-the-badge)](../../wiki)

</div>

<img width="100%" height="3" src="https://capsule-render.vercel.app/api?type=rect&color=0:C0502B,55:E0B25C,100:0E1410&height=3&section=header">

<table align="center" width="100%">
<tr>
<td align="center" width="25%">🛰<br><b>ZONE INTEL</b><br><sub>control-zone pressure,<br>hot-zone payout timer</sub></td>
<td align="center" width="25%">🎯<br><b>SILENT FIRE</b><br><sub>correction on the frame,<br>camera stays still</sub></td>
<td align="center" width="25%">🛡<br><b>ARMOUR FACING</b><br><sub>weak side on tanks,<br>occupant count</sub></td>
<td align="center" width="25%">🧱<br><b>BUILDING READ</b><br><sub>FOB walls and cover<br>through the concrete</sub></td>
</tr>
</table>

<img width="100%" height="3" src="https://capsule-render.vercel.app/api?type=rect&color=0:0E1410,55:E0B25C,100:C0502B&height=3&section=header">

## 📋 Situation

A WARDOGS match is one hundred players, three teams, and a 2×2 km control zone that shifts
inside a bigger map. Points tick from presence, not from kills, and the first team to a hundred
takes it. You start every life with ten thousand in the bank, buy a kit out of it, and the cash
carries between matches — so the thing that actually dies with you is the loadout you paid for.

That makes two kinds of blindness expensive. Standing in a zone you can't see the edges of, and
walking armour or a ghillie you never spotted. The overlay closes both: it reads the zone, reads
the field, and never tells the camera to move.

<table>
<tr><th align="left" width="50%">🪖 Without</th><th align="left" width="50%">🛰 With this build</th></tr>
<tr><td>Zone edge is a guess, pressure is a rumour</td><td>Zone boundary, both teams' presence and hot-zone double-cash timer</td></tr>
<tr><td>Scan the skyline for a tank that already ranged you</td><td>Vehicle box, occupant count and the weak side marked</td></tr>
<tr><td>Fire into concrete and hope the wall was thin</td><td>Destructible cover and FOB walls called out before you commit</td></tr>
<tr><td>Buy blind, die expensive</td><td>Kit cost versus threat readout, cheapest viable loadout suggested</td></tr>
<tr><td>Squad spread over 2 km with no shape</td><td>Squad outline and separation distance, always the same colour</td></tr>
<tr><td>Correction yanks your aim and clips look sloppy</td><td>Silent mode — nothing moves on camera</td></tr>
</table>

<details>
<summary><sub>📑 <b>Contents</b> — expand</sub></summary>

<br>

[In the archive](#-in-the-archive) · [Quick start](#-quick-start) · [Modules](#-modules) ·
[Field cards](#-field-cards) · [Comparison](#-comparison) · [Rig requirements](#-rig-requirements) ·
[Hotkeys](#-hotkeys) · [Presets by role](#-presets-by-role) · [Supported builds](#-supported-builds) ·
[EAC surface](#-eac-surface) · [Performance](#-performance) · [Limits](#-limits) ·
[FAQ](#-faq) · [Troubleshooting](#-troubleshooting) · [Changelog](#-changelog) ·
[Roadmap](#-roadmap) · [Repository layout](#-repository-layout) · [Build from source](#-build-from-source) ·
[Credits](#-credits) · [Disclaimer](#-disclaimer)

</details>

---

## 📦 In the archive

> [!CAUTION]
> Only this repository's Releases. There are mirrors with the same name and older tags.

| File | Purpose |
|---|---|
| `wardogs.exe` | The overlay loader. This is the one you run. |
| `wardogs.json` | Default config — keep it, it survives updates |
| `\data\` | Season offsets and the EAC-safe branch table |
| `\profiles\` | Shipped presets — assault, marksman, armour, logi |
| `README.txt` | Offline install sheet and key card |

`wardogs.exe` is unsigned, so SmartScreen raises the blue prompt on the first run: **More info →
Run anyway**. Check the hash against the first line of the release notes before launching:

```powershell
Get-FileHash .\wardogs.exe -Algorithm SHA256
```

---

## 🚀 Quick start

| # | Step | |
|---|---|---|
| 1 | Take the build on **[Releases](https://github.com/OnyxDaimyoCavity/wardogs-cheat-pc/releases/latest)** | <kbd>⬇</kbd> |
| 2 | Unpack to `C:\WARDOGS-CFG\` — never into `Program Files` | <kbd>📁</kbd> |
| 3 | Game to **Borderless**, fullscreen off | <kbd>🖥</kbd> |
| 4 | Launch the game, sit in the deploy screen | <kbd>🎮</kbd> |
| 5 | Start `wardogs.exe`, press <kbd>Insert</kbd>, take a role preset | <kbd>⌨</kbd> |
| 6 | Bind <kbd>Delete</kbd> as panic, save the profile | <kbd>💾</kbd> |

> [!NOTE]
> Load the overlay in the deploy screen, not mid-life. EAC runs its check at process start, and a
> deploy screen gives it the cleanest handshake.

---

## 🧩 Modules

> Every module is a checkbox that applies live and lands in the active profile. Nothing is
> mandatory, nothing needs a restart.

### 🛰 Recon

| Module | Behaviour | Range |
|---|---|---|
| `Player ESP` | Box, team, class and distance | 15 – 600 m |
| `Team colours` | Three fixed hues, never reused | — |
| `Squad outline` | Teammates boxed separately, separation shown | — |
| `Loadout read` | Visible kit class and rough value | 300 m |
| `Vehicle ESP` | Tank, APC, heli, truck — with occupant count | 700 m |
| `Armour facing` | Rear, track and turret-ring weak sides marked | 400 m |
| `Emplacement ESP` | Static guns, FOB walls, deployed cover | 300 m |
| `Zone overlay` | Boundary, own pressure, enemy pressure share | map-wide |
| `Hot-zone timer` | Double-cash window and remaining time | map-wide |
| `Death markers` | Where the last squad wiped, with age | 200 m |
| `Bearing tape` | Compass strip with target bearings | — |
| `Distance fade` | Boxes thin past range instead of popping | — |

<details>
<summary><sub>🧩 draw options</sub></summary>

| Option | Effect |
|---|---|
| `Box · bracket · chevron` | Three marker styles |
| `Through-cover` | Keeps markers over concrete and FOB walls |
| `Crowd limit` | Cap on simultaneous markers, nearest first |
| `Label scale` | Text scale independent of menu scale |
| `Off-screen arrows` | Marker for armoured threats on your flanks |

</details>

### 🎯 Fire control

| Module | Behaviour |
|---|---|
| `Silent assist` | Correction applied on the shot frame — camera untouched |
| `Aim assist` | Visible pull, adjustable strength |
| `Bone priority` | Head · chest · pelvis, per-class presets |
| `Lead` | Moving-target lead for rifle and DMR |
| `Vehicle weak spots` | Rear and track hand-off for AT work |
| `Hitbox draw` | Real damage volume over the model |
| `Range gate` | Holds the shot until true reach |
| `FOV slider` | 5° – 360° |
| `Smooth curve` | 0.0 – 1.0, the anti-flick knob |
| `Humanise` | Micro-jitter so trails stop being dead straight |

> [!IMPORTANT]
> `Silent assist` and `Aim assist` don't stack. Silent for recordings and ghillie play, visible
> pull for close assault where you want the flick.

### 💰 Economy

<sub>Cash carries between matches. So does a bad kit decision.</sub>

| Module | Behaviour | Default |
|---|---|---|
| `Budget tracker` | Bank, spend and bleed per life | on |
| `Kit value sort` | Loadout list ordered by cost per usefulness | on |
| `Hot-zone ping` | Payout window push, even off-screen | on |
| `Squad payout meter` | Revive and ferry income estimate | off |
| `Reserve warning` | Flags a kit above your remaining bank margin | on |

### 🏃 Mobility

| Module | Behaviour |
|---|---|
| `Sprint multiplier` | 1× – 4× |
| `Fly` | Free movement, <kbd>Space</kbd> / <kbd>Ctrl</kbd> altitude |
| `Fast redeploy` | Teleport to squad, FOB or map ping |
| `Waypoints` | Named, exported with the profile |
| `No fall damage` | Roof and cliff drops are free |
| `Vehicle entry range` | Extended hand-off distance |

> [!WARNING]
> A 2 km hop across an active zone rubber-bands. `Fast redeploy` is reliable to squad and FOB,
> not to a point on the far side of the map.

### 🌫 Environment

| Module | Behaviour |
|---|---|
| `No foliage` | Strips the grass layer that eats hitboxes |
| `No fog` | Clear draw distance |
| `No rain` | Rain and its grey grade removed |
| `Full bright` | Flat ambient, night becomes a palette |
| `Time of day` | Pin the sun to any hour |
| `Destructible highlight` | Cover that will break, tinted |
| `Stream grade` | Contrast that survives compression |
| `Crosshair` | Dot · chevron · custom |

### 🎛 Interface

- Drag-anywhere menu, `80 %` – `150 %` scale
- Search on <kbd>Ctrl</kbd> + <kbd>F</kbd>, conflicts flagged before apply
- Profiles bound to role and map, auto-loaded on spawn
- `Stream mode` hides the watermark
- `wardogs.json` readable, diffable, exportable
- OSD: FPS · markers · zone score · build
- `Panic key` clears every draw in one press

---

## 🗂 Field cards

<table>
<tr><td width="50%" valign="top">

**Through the concrete**

Walls are destructible in this game, so a marker that vanishes behind a building is a marker you
paid for and can't use. `Through-cover` keeps boxes over concrete, FOB walls and rubble, with the
cover type named on the label so you know what will eat the round.

`through-cover on` · `label cover`

</td><td width="50%" valign="top">

**Armour, not silhouette**

A tank shows a box and an occupant count; the weak side is drawn as a wedge that rotates with the
hull. Aim hand-off for AT weapons lands on the marked face, and `Range gate` refuses the shot
outside real reach instead of wasting the rocket.

`facing on` · `gate 12 m`

</td></tr>
<tr><td valign="top">

**Zone math**

Boundary, your team's presence share and theirs. The score moves on presence, so the readout
tells you whether standing here wins or feeds — and the hot-zone timer says when standing here
pays double.

</td><td valign="top">

**Silent for the ghillie**

Correction computes on approach and applies on the shot frame, so the scope never slides. On a
clip it reads as a very good day rather than a very good program.

</td></tr>
</table>

---

## 🥊 Comparison

| | This build | Driver cheat | Free paste |
|---|:---:|:---:|:---:|
| External, no driver | ✅ | ❌ | ⚠ |
| No injection | ✅ | ❌ | ⚠ |
| Survives a season patch | ✅ re-anchor ≤48 h | ❌ new bypass | ❌ |
| Vehicle and armour intel | ✅ | ⚠ | ❌ |
| Zone and economy readout | ✅ | ❌ | ❌ |
| Through-cover marking | ✅ | ⚠ | ❌ |
| Role profiles | ✅ | ⚠ | ❌ |
| Time to first match | ~2 min | 10+ min, reboot | depends |

---

## 🖥 Rig requirements

| | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 21H2 x64 | Windows 11 23H2 x64 |
| CPU | 6 threads | 8 cores / 16 threads |
| RAM | 16 GB | 32 GB |
| GPU | DX12 · 6 GB VRAM | DX12 · 10 GB VRAM |
| Game | WARDOGS on Steam — Early Access | — |
| Runtime | .NET Desktop 8 | — |
| Display | Borderless, 1080p | Borderless, 1440p, ≥120 Hz |
| Mic | not required | local voice on for squad play |

---

## ⌨ Hotkeys

<table align="center">
<tr>
<td align="center"><kbd>Insert</kbd><br><sub>menu</sub></td>
<td align="center"><kbd>End</kbd><br><sub>all draws</sub></td>
<td align="center"><kbd>Delete</kbd><br><sub>panic</sub></td>
<td align="center"><kbd>Home</kbd><br><sub>fire assist</sub></td>
<td align="center"><kbd>F1</kbd><br><sub>recon</sub></td>
</tr>
<tr>
<td align="center"><kbd>F2</kbd><br><sub>zone overlay</sub></td>
<td align="center"><kbd>F3</kbd><br><sub>armour facing</sub></td>
<td align="center"><kbd>F4</kbd><br><sub>save state</sub></td>
<td align="center"><kbd>F5</kbd><br><sub>reload config</sub></td>
<td align="center"><kbd>Ctrl</kbd>+<kbd>F</kbd><br><sub>search</sub></td>
</tr>
</table>

---

## 🎖 Presets by role

Presets sit in `\profiles\` and load on role and map, so a marksman doesn't inherit an assault
FOV.

| Role | Preset | Tuned for |
|---|---|---|
| Assault | `Assault` | wide FOV, visible pull, close ranges |
| Marksman | `Marksman` | silent, lead, drop and long ranges |
| Armour | `Armour` | weak-side hand-off, vehicle boxes first |
| Logi / pilot | `Support` | squad outline, FOB markers, sightline map |
| Squad lead | `Command` | zone math, separation, death markers |

```jsonc
{
  "name": "Marksman",
  "auto": { "role": "marksman", "map": ["*"] },
  "recon": { "players": true, "range": 450, "facing": true, "throughCover": true, "crowd": 24 },
  "fire": { "mode": "silent", "bone": "head", "fov": 28, "smooth": 0.25, "lead": true, "gate": 30 },
  "economy": { "budget": true, "reserveWarn": true },
  "env": { "noFoliage": true, "streamGrade": false }
}
```

---

## 🧩 Supported builds

| Build | Status | Notes |
|---|---|---|
| Season 3 | ✅ full | every module |
| Season 2 | ⚠ partial | no `Armour facing`, no `Zone overlay` |
| Season 1 | ⚠ read-only | recon and fire control only |
| Open tests / preview | ⚠ untested | offsets drift, expect greyed modules |

> [!NOTE]
> Season rolls are the real patch here. The changelog names what broke and what was re-anchored,
> and the tag lands inside 48 h — wait for it instead of launching on the old build.

---

## 🛡 EAC surface

WARDOGS ships **Easy Anti-Cheat** at kernel level. This build stays fully external: it reads and
writes the process from outside, no driver, no injection, nothing added to the module list at boot.

| Surface | This build | Driver-based |
|---|---|---|
| Kernel driver | none | loaded, signed or not |
| Injection | none | yes |
| Boot-time scan target | process memory | driver + memory |
| What a season breaks | offsets | driver + offsets |
| Recovery | tag ≤48 h | often a new bypass |

**Undetected as of `2026-11-23`** — a dated line, so it ages honestly instead of turning into a
ban guarantee. Re-read the badge the day you install and watch Releases, not the comment section.

---

## 📊 Performance

| Configuration | Frame cost |
|---|---|
| Recon only · 300 m · 20 markers | ~1.4 ms |
| Everything on · 600 m · crowd 40 | ~5.2 ms |
| Idle, menu closed | ~0.1 ms |

Drawing runs on its own thread against a snapshot buffer. In a hundred-player zone, cut `crowd`
before anything else — it is the only knob that scales with what's actually on your screen.

---

## 🚧 Limits

- `Fast redeploy` is client-side; long hops across an active zone rubber-band.
- `Armour facing` needs fresh offsets — a season-day patch greys it out until the tag lands.
- Weak spots are geometry, not a damage model: the game still decides penetration.
- Cash readout sees values, never the enemy's bank balance.
- `Zone overlay` reads the minimap state; a server with a modified HUD can flatten it.
- Windows only — no Proton, no Linux, no cloud rigs.

---

## ❓ FAQ

<details>
<summary><b>Does it hold on Season 3?</b></summary>

Yes, against current Season 3 offsets. After a season roll, wait for the matching `v1.0.x` tag.
</details>

<details>
<summary><b>Does EAC catch it?</b></summary>

Nothing kernel-side to find: the process lives outside the game. That's a structural argument, not
immortality — the badge date is what you check.
</details>

<details>
<summary><b>Will viewers spot it on stream?</b></summary>

Not with `Stream mode` and silent assist. Visible pull is the one that reads on camera.
</details>

<details>
<summary><b>Does it aim for me at long range?</b></summary>

It leads and gates, and holds the shot until the target is inside real reach. You still own the
trigger — that's deliberate, unlimited range looks worse on vehicles.
</details>

<details>
<summary><b>Can it see through buildings?</b></summary>

Yes, and it names the cover type. Destructible walls are flagged differently from solid concrete,
so you know what the round will go through.
</details>

<details>
<summary><b>Do I keep my config between versions?</b></summary>

Yes. Update in place — `wardogs.json` and `\profiles\` are untouched by an update.
</details>

<details>
<summary><b>Does it help the economy?</b></summary>

It reads your bank, sorts kits by value and warns before a kit eats your margin. It never touches
the server-side wallet.
</details>

<details>
<summary><b>100-player zones and a mid laptop?</b></summary>

Default profile is under 2 ms. Start at recon 250 m, `crowd 16`, zone overlay on, through-cover off.
</details>

---

## 🔧 Troubleshooting

| Symptom | Fix |
|---|---|
| Menu never appears | Borderless, start the loader in the deploy screen |
| Draws show, mouse is dead | Run as administrator, close overlay hooks |
| Boxes lag behind players | Offsets/season mismatch — install the matching tag |
| Crash at launch | Another overlay or a second anticheat is loaded |
| Redeploy rubber-bands | Short hop to squad or FOB, not across the zone |
| Frame drops in a big zone | Lower `crowd`, cut range, disable through-cover |
| Profile won't save | Folder is read-only — leave `Program Files` |
| EAC kicks on start | Verify in Steam, launch vanilla once, then the loader |

Escalate with build tag, season, map and the tail of `\logs\wardogs.log`:
[bug template](../../issues/new?template=bug.yml).

---

## 📝 Changelog

| Version | Date | |
|---|---|---|
| `v1.0.0` | 2026-11-23 | first public build: recon, fire control, economy, mobility, environment |
| `v0.9.2` | 2026-11-18 | armour facing wedge, occupant count |
| `v0.9.0` | 2026-11-11 | zone overlay, hot-zone timer |
| `v0.8.1` | 2026-11-04 | through-cover, destructive tint |
| `v0.8.0` | 2026-10-28 | silent assist, role profiles |
| `v0.7.0` | 2026-10-19 | snapshot renderer, OSD |

---

## 🗺 Roadmap

- [x] Snapshot renderer off the main thread
- [x] Role profiles
- [x] Silent fire control
- [ ] Season 3 vehicle database, every hull
- [ ] FOB structure map
- [ ] Squad bearing relay
- [ ] Replay-safe marker log
- [ ] EN · RU · DE · PL

---

## 🗂 Repository layout

```
wardogs-cheat-pc/
├─ docs/            install, module reference, offset notes
├─ profiles/        role presets
├─ src/
│  ├─ render/       drawing, snapshot buffer
│  ├─ game/         offsets, season adapters
│  └─ ui/           menu, keys
├─ CMakeLists.txt
├─ wardogs.json
└─ README.md
```

---

## 🛠 Build from source

```powershell
git clone https://github.com/OnyxDaimyoCavity/wardogs-cheat-pc.git
cd wardogs-cheat-pc
cmake -B build -A x64 -DCMAKE_BUILD_TYPE=Release
cmake --build build --config Release
# output: build\Release\wardogs.exe
```

Visual Studio 2022 with the C++ workload and the .NET 8 SDK. Offsets re-dump through
`tools\dump.ps1` after a season roll — read `docs\offsets.md` first.

<div align="center">

![cpp](https://img.shields.io/badge/C%2B%2B20-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![cmake](https://img.shields.io/badge/CMake-064F8C?style=flat-square&logo=cmake&logoColor=white)
![dx12](https://img.shields.io/badge/DirectX%2012-107C10?style=flat-square)
![win32](https://img.shields.io/badge/Win32-0078D6?style=flat-square&logo=windows&logoColor=white)

</div>

---

## 🙏 Credits

- Offset work and season re-anchors by the [contributors](../../graphs/contributors)
- Everyone who filed a season tag instead of *"broken"*

<div align="center">

<a href="https://contrib.rocks"><img src="https://contrib.rocks/image?repo=OnyxDaimyoCavity/wardogs-cheat-pc" alt="contributors"></a>

</div>

---

## ⚖ Disclaimer

Unofficial fan build. Not affiliated with BULKHEAD, Team17 or WARDOGS. Use where third-party
software is allowed, at your own risk — no guarantee of account safety.

<img width="100%" height="3" src="https://capsule-render.vercel.app/api?type=rect&color=0:C0502B,55:E0B25C,100:0E1410&height=3&section=header">

<div align="center">

<a href="https://star-history.com/#OnyxDaimyoCavity/wardogs-cheat-pc&Date">
  <img src="https://api.star-history.com/svg?repos=OnyxDaimyoCavity/wardogs-cheat-pc&type=Date" width="720" alt="star history">
</a>

<br><br>

[![stars](https://img.shields.io/github/stars/OnyxDaimyoCavity/wardogs-cheat-pc?style=for-the-badge&labelColor=141414&color=E0B25C)](../../stargazers)
[![forks](https://img.shields.io/github/forks/OnyxDaimyoCavity/wardogs-cheat-pc?style=for-the-badge&labelColor=141414&color=C0502B)](../../forks)
[![commits](https://img.shields.io/github/last-commit/OnyxDaimyoCavity/wardogs-cheat-pc?style=for-the-badge&labelColor=141414&color=7C8A96)](../../commits/main)

<br>

<sub>**`// hold the zone`**</sub>

<br>

<sub><a href="#top">↑ back to top</a></sub>

</div>
