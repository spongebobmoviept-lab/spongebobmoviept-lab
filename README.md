Self-taught builder. Two things live here: **[Ruthless Controller Relay](https://github.com/spongebobmoviept-lab/RuthlessControllerRelay)**, which turns a gamepad into a HOTAS for flight sims, and a **[family of self-hosted apps for Plex](#plex-apps)**.

<p align="center">
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay"><img src="assets/hero.svg" width="100%" alt="Ruthless Controller Relay. Fly with the controller you already own: it turns a PS4, PS5 or Xbox controller into a real HOTAS joystick, or a clean regular gamepad, in any Windows game."></a>
</p>

<p align="center">
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay/releases/latest"><img src="assets/download.svg" width="340" alt="Download Ruthless Controller Relay for Windows (latest release)"></a>
</p>

<p align="center">
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay/releases"><img src="https://img.shields.io/github/downloads/spongebobmoviept-lab/RuthlessControllerRelay/total?label=downloads&color=eb5e28" alt="Total downloads"></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay/releases/latest"><img src="https://img.shields.io/github/v/release/spongebobmoviept-lab/RuthlessControllerRelay?label=release&color=eb5e28" alt="Latest release"></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#quick-start"><img src="https://img.shields.io/badge/platform-Windows%2010%2F11-3d444d" alt="Platform: Windows 10/11"></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay"><img src="https://img.shields.io/badge/language-C-3d444d?logo=c&logoColor=white" alt="Language: C"></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-3d444d" alt="License: MIT"></a>
</p>

Flight sims and other HOTAS games bind their controls to a joystick, and Windows treats a gamepad as a different kind of device, so those games won't take a controller's sticks. Ruthless Controller Relay shows your controller to them as a virtual joystick, and to everything else as a normal gamepad. Flight-sim and WARDOGS players use it to fly with the controller they already own.

<p align="center">
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#how-it-works"><img src="assets/feature-hotas.svg" width="272" alt="HOTAS mode: your controller shows up as a real joystick, so flight sims and HOTAS games bind to it."></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#how-it-works"><img src="assets/feature-gamepad.svg" width="272" alt="Normal mode: a clean virtual Xbox or PlayStation gamepad for every other game."></a>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#controls"><img src="assets/feature-switch.svg" width="272" alt="Switch live: one hotkey (Ctrl+Alt+H) or one controller button flips modes, with no reboot and no replug."></a>
</p>

<p align="center">
  Rumble, lightbar color and battery level come through wherever the connection allows.<br>
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#quick-start">Quick start</a> ·
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#what-works-and-what-doesnt">What works on which controller</a> ·
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#is-this-safe-to-run">Is it safe to run?</a> ·
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay/blob/main/docs/DEVELOPMENT_JOURNEY.md">How it was built</a> ·
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay">Source code</a>
</p>

<details>
<summary>See it running: the live dashboard</summary>
<br>
<p align="center">
  <a href="https://github.com/spongebobmoviept-lab/RuthlessControllerRelay#how-it-works"><img src="https://raw.githubusercontent.com/spongebobmoviept-lab/RuthlessControllerRelay/main/docs/images/dashboard-normal-mode.png" width="560" alt="The live dashboard with a wired DualSense in Normal mode"></a>
</p>
<p align="center"><sub>The live dashboard: real-time axis and button state, the current mode, and what the game sees next to what is actually plugged in.</sub></p>
</details>

<br>
<br>

<a name="plex-apps"></a>

<p align="center">
  <a href="#plex-apps"><img src="assets/plex-apps.svg" width="100%" alt="Self-hosted apps for Plex: a family of seven apps that plug into Plex, Sonarr, Radarr, Dispatcharr and Discord."></a>
</p>

Seven small apps. Each one installs with Docker Compose (amd64 and arm64) and has its own web setup page.

<br>

<a href="https://github.com/spongebobmoviept-lab/tubarr"><img align="right" width="46%" src="assets/tubarr.webp" alt="Tubarr's web UI: the Channels page, a grid of channel posters (the repo's demo data)"></a>

### [Tubarr](https://github.com/spongebobmoviept-lab/tubarr)

**Your YouTube subscriptions, as a Plex library.**

- Channels become shows and playlists become seasons, with the creator's own titles, chapters and subtitles.
- New uploads land in Plex first; the backlog fills in at a calm, human pace.
- Fills to the size you set, then rolls: newest in, oldest out.
- Comes with **Trimarr**, an ad trimmer for sponsor segments.

[Install guide](https://github.com/spongebobmoviept-lab/tubarr#quick-start) &nbsp; [![Release][tubarr-v]][tubarr-rel] [![Docker: amd64, arm64][docker]][tubarr-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/tunerbox"><img align="left" width="46%" src="assets/tunerbox.svg" alt="Tunerbox sits between Dispatcharr and Plex Live TV, with a guide of regular and event channels"></a>

### [Tunerbox](https://github.com/spongebobmoviept-lab/tunerbox)

**The missing piece between Dispatcharr and Plex Live TV.**

- A tuner Plex accepts, advertising exactly as many tuners as your provider allows connections.
- Sports and pay-per-view event channels that stay put when the provider renumbers them.
- A lineup that cleans itself, re-checked every night.

[Install guide](https://github.com/spongebobmoviept-lab/tunerbox#quick-start) &nbsp; [![Release][tunerbox-v]][tunerbox-rel] [![Docker: amd64, arm64][docker]][tunerbox-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/movienight-player"><img align="right" width="46%" src="assets/movienight-player.svg" alt="Movie Night Player: one movie from Plex, watched by friends in their browsers, in sync"></a>

### [Movie Night Player](https://github.com/spongebobmoviept-lab/movienight-player)

**A watch party for Plex, in everyone's browser.**

- Start a movie from Plex and your friends watch it together, in sync. They need no Plex account and no app.
- Run it from Discord through Servarr, or from the Playback tab on the watch page.
- Two editions: **Server Owner** (you run the Plex server) and **Guest** (a friend shares theirs with you).

[Install guide](https://github.com/spongebobmoviept-lab/movienight-player#readme) &nbsp; [![Release][player-v]][player-rel] [![Docker: amd64, arm64][docker]][player-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/Servarr"><img align="left" width="46%" src="assets/servarr.svg" alt="Servarr: Movie Night, release calendars, leveling and moderation"></a>

### [Servarr](https://github.com/spongebobmoviept-lab/Servarr)

**The Discord bot for a Plex server's community.**

- **Movie Night:** a daily vote among movies you already have, then the winner starts in the Movie Night Player at showtime.
- Release calendars for movies, TV and anime.
- Leveling (`/rank`, `/leaderboard`) and moderation.

[Install guide](https://github.com/spongebobmoviept-lab/Servarr#quick-start) &nbsp; [![Release][servarr-v]][servarr-rel] [![Docker: amd64, arm64][docker]][servarr-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/Requestarr"><img align="right" width="46%" src="assets/requestarr.svg" alt="Requestarr: /movie goes to Radarr, /tv and /anime go to Sonarr, and a thread follows the request until it is available"></a>

### [Requestarr](https://github.com/spongebobmoviept-lab/Requestarr)

**Movie, TV and anime requests, right from Discord.**

- `/movie`, `/tv` and `/anime`: pick from up to five matches, confirm, done.
- Adds straight to Radarr or Sonarr. No Plex account linking, no dashboard to check.
- Posts progress in a thread until the request is ready to watch.

[Install guide](https://github.com/spongebobmoviept-lab/Requestarr#quick-start) &nbsp; [![Release][requestarr-v]][requestarr-rel] [![Docker: amd64, arm64][docker]][requestarr-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/Nyaarr"><img align="left" width="46%" src="assets/nyaarr.svg" alt="Nyaarr sorts anime releases: English subs from a known group, a bare Subbed that waits for you, and foreign subs that never count as English"></a>

### [Nyaarr](https://github.com/spongebobmoviept-lab/Nyaarr)

**Anime release filtering for Sonarr and Radarr.**

- Sub or dub by choice, for the whole library or per show.
- Tells English subs from foreign ones, and cleans up duplicate grabs.
- Never grabs what it isn't sure about: uncertain releases wait for your pick.

[Install guide](https://github.com/spongebobmoviept-lab/Nyaarr#quick-start) &nbsp; [![Release][nyaarr-v]][nyaarr-rel] [![Docker: amd64, arm64][docker]][nyaarr-img]<br clear="all">

<br clear="all">
<br>

<a href="https://github.com/spongebobmoviept-lab/Reclaimarr"><img align="right" width="46%" src="assets/reclaimarr.svg" alt="Reclaimarr: 1080p becomes 4K when someone presses play, and an old 60 GB remux becomes a smaller copy"></a>

### [Reclaimarr](https://github.com/spongebobmoviept-lab/Reclaimarr)

**4K when someone presses play. Smaller files everywhere else.**

- Starts a 4K upgrade the moment someone plays a movie that isn't in 4K yet.
- Swaps huge remuxes nobody has watched lately for a smaller copy of the same movie.
- Nothing is deleted until the replacement is confirmed playing in Plex.

[Install guide](https://github.com/spongebobmoviept-lab/Reclaimarr#quick-start) &nbsp; [![Release][reclaimarr-v]][reclaimarr-rel] [![Docker: amd64, arm64][docker]][reclaimarr-img]<br clear="all">

<br clear="all">

### How they fit around Plex

```mermaid
%%{init: {"flowchart": {"nodeSpacing": 28, "rankSpacing": 40, "padding": 10}}}%%
flowchart LR
    discord(["Discord"]) --> servarr["Servarr"] ----> player["Movie Night Player"]
    discord --> requestarr["Requestarr"] --> arrs(["Sonarr / Radarr"])
    arrs <--> nyaarr["Nyaarr"] & reclaimarr["Reclaimarr"]
    arrs --> plex{{"Plex"}}
    youtube(["YouTube"]) --> tubarr["Tubarr"] ---> plex
    iptv(["IPTV"]) & ersatztv(["ErsatzTV"]) --> dispatcharr(["Dispatcharr"]) --> tunerbox["Tunerbox"] --> plex
    plex --> player

    classDef app fill:#d4af37,stroke:#e8c65a,color:#101010
    classDef hub fill:#1f1f1f,stroke:#e5a00d,stroke-width:2px,color:#e5a00d
    class requestarr,servarr,tubarr,tunerbox,nyaarr,reclaimarr,player app
    class plex hub
```

<sub>Gold boxes are the apps above; rounded ones are the software they plug into.</sub>

---

<a href="https://github.com/spongebobmoviept-lab/Discord-VLC-Audio-Share"><img align="left" width="36%" src="assets/discord-vlc-audio-share.svg" alt="Discord VLC Audio Share: app audio goes through VB-Cable into VLC, and Discord shares the VLC window"></a>

### [Discord VLC Audio Share](https://github.com/spongebobmoviept-lab/Discord-VLC-Audio-Share)

**A small Windows tool for sharing to Discord with clean audio.**

- Shares one monitor or one app window, with that app's own sound.
- Routes the audio through VB-Audio Virtual Cable and VLC, so friends hear the app and nothing else.
- A Stream Deck button can start and stop it.

[Quick start](https://github.com/spongebobmoviept-lab/Discord-VLC-Audio-Share#quick-start)<br clear="all">

[docker]: https://img.shields.io/badge/docker-amd64%20%7C%20arm64-3d444d?logo=docker&logoColor=white
[tubarr-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/tubarr?label=release&color=dcb741
[tubarr-rel]: https://github.com/spongebobmoviept-lab/tubarr/releases/latest
[tubarr-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/tubarr
[tunerbox-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/tunerbox?label=release&color=dcb741
[tunerbox-rel]: https://github.com/spongebobmoviept-lab/tunerbox/releases/latest
[tunerbox-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/tunerbox
[player-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/movienight-player?label=release&color=dcb741
[player-rel]: https://github.com/spongebobmoviept-lab/movienight-player/releases/latest
[player-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/movienight-player
[servarr-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/Servarr?label=release&color=dcb741
[servarr-rel]: https://github.com/spongebobmoviept-lab/Servarr/releases/latest
[servarr-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/servarr
[requestarr-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/Requestarr?label=release&color=dcb741
[requestarr-rel]: https://github.com/spongebobmoviept-lab/Requestarr/releases/latest
[requestarr-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/requestarr
[nyaarr-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/Nyaarr?label=release&color=dcb741
[nyaarr-rel]: https://github.com/spongebobmoviept-lab/Nyaarr/releases/latest
[nyaarr-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/nyaarr
[reclaimarr-v]: https://img.shields.io/github/v/release/spongebobmoviept-lab/Reclaimarr?label=release&color=dcb741
[reclaimarr-rel]: https://github.com/spongebobmoviept-lab/Reclaimarr/releases/latest
[reclaimarr-img]: https://github.com/users/spongebobmoviept-lab/packages/container/package/reclaimarr
