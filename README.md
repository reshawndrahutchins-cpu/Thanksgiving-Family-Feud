# 🦃 Thanksgiving Family Feud: Beta Club Edition

A browser-based Family Feud game for projector play. It's a single `index.html` file with no build step and no server, so it runs on **GitHub Pages**. You can also just double-click the file to run it offline.

## Put it on GitHub Pages

1. Go to [github.com/new](https://github.com/new) and create a **public** repository (for example `thanksgiving-feud`).
2. Click **Add file → Upload files**, drag in `index.html` (and this README), then click **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main`, folder `/ (root)`, then click **Save**.
4. Wait about a minute and refresh. Your game will be live at:
   `https://YOUR-USERNAME.github.io/thanksgiving-feud/`

## Running the game

The game uses **two windows** in the same browser on the same computer:

| Window | URL | Who sees it |
|---|---|---|
| 📺 Audience screen | `.../thanksgiving-feud/` | Projected for the room. Answers stay hidden until revealed. |
| 🎙️ Host controls | `.../thanksgiving-feud/#host` | Host's laptop only. Shows the answer key and all buttons. |

1. Open the `#host` URL on the laptop. Set the team names.
2. Click **📺 Open audience screen** and drag that window to the projector (use *Extend* display mode, not *Mirror*). Press **F** for full screen.
3. **Click once on the audience screen** so the browser allows sound.
4. Click **Start Round 1** and follow the step-by-step hints on the host screen.

The game auto-saves, so a refresh won't lose your scores. **↺ Reset game** starts over.

### Keyboard shortcuts (either window)
- `1`–`6`: reveal that answer
- `X`: strike (or a face-off miss)
- `F`: full screen (audience screen)
- `H`: open host controls (from the audience screen)

## What's included
- 5 rounds (Round 5 is double points) with a live round bank, strikes, face-off → play/pass → steal flow
- Sudden-death tie-breaker (only Pumpkin Pie wins!)
- Fast Money with 20s / 25s timers, a duplicate-answer **BUZZ!**, a hide-Player-1 toggle, and a +200 bonus
- Ding, buzzer, and fanfare sounds, plus a big red ❌ overlay

## Editing questions
Open `index.html` and edit the `GAME` object near the top of the `<script>` section. Each answer is written as `["Answer text", points]`. Rounds can have any number of answers.
