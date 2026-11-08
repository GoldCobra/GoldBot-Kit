# GoldBot kits

GoldBot is a self-learning bot for *Mario Strikers Charged*, playing on the native PC port
([Recharged](https://github.com/previouslevelgames/recharged)). This repository only carries the
kits for the people who play against it or record their matches for it. The bot's code is not public.

## Download

| Kit | What it is for | Start |
|---|---|---|
| [goldbot-kit.zip](https://github.com/GoldCobra/GoldBot-Kit/releases/latest/download/goldbot-kit.zip) | Play against GoldBot offline, in real time, in your own Recharged with your own settings. The game opens at the captain select, with the bot's team already on its side (one of its twelve captains, in a fair random order); you pick the stadium of every match, and every stadium plays alike (Secure Stadium, Fast terrain, Thunder Island walls). It comes back there after every match. Your matches are packed into one zip for GoldCobra. | `play-goldbot.cmd` |
| [goldbot-demo-kit.zip](https://github.com/GoldCobra/GoldBot-Kit/releases/latest/download/goldbot-demo-kit.zip) | Record your own matches against a friend on one PC. Matches alone against the CPU are kept but no longer train the bot: what beats the CPU does not beat people, so only matches between people and against GoldBot do. | `record-demos.cmd` |

**GoldBot kit:** unpack the zip into your own Recharged folder, the one with `recharged.exe`. That puts
`play-goldbot.cmd` beside `recharged.exe` and the folder `goldbot-kit` beside it. Set everything in
Recharged as usual, then start `play-goldbot.cmd`. It plays only beside the Recharged release the bot was
tested on (the release notes name it) and tells you if yours differs. Your Recharged, its settings and its
save stay as they are. **Demo kit:** unpack it anywhere (not into *Program Files*) and start
`record-demos.cmd`. Each kit's README explains the rest. Windows 10 or 11 (x64) is needed.

## Which disc

Use the European **Mario Strikers Charged Football, `R4QP01` revision 2**. GoldBot trains and is measured
on it, so the bot plays its best there and your matches fit its training best. Revision 1 and the USA disc
(`R4QE01`) work too; every recorded match names the disc it was played on.

## Play Z tricks

Chips over the goalkeeper, chips off the wall beside him and self passes (Waluigi, Boo, Hammer Bro and
Toad play their own chip again in the air) are allowed in competitive play and wanted here: GoldBot
learns them from your matches. The kits' READMEs explain them.

## Updates

Releases are named by the bot's version: GoldBot V12.1 is champion V12 in its second kit release (the one
for Recharged 1.1.5), and V13.0 will bring the next champion.

Each kit checks this repository at every start. When a newer release is out, it downloads that release,
checks its SHA-256, and replaces its own files in place. Your player name, disc image, settings,
recordings and any zips you have not sent yet stay where they are. This way everyone plays the same game
build and the same bot. The GoldBot kit takes a newer release only when it is made for the Recharged you
have. When Recharged has a new release, the bot is brought to it first, and until then the kit says so
(Recharged's update dialog has a *Later* button meanwhile). When the bot is on a newer Recharged than yours,
the kit asks you to update Recharged first: its own update keeps the GoldBot kit in its folder, and the
next start of `play-goldbot.cmd` takes the new kit by itself. GoldCobra only takes matches that were
recorded with the newest kit. Without an internet connection the kit still plays, so update the next
time you are online.

## What is inside, and what is not

- **No game data.** You need your own *Mario Strikers Charged* disc image (Wii); see "Which disc".
- A build of Recharged, the PC port, with GoldBot's bridge and recorder (in the GoldBot kit's
  `goldbot-kit\game\recharged`; it plays only the bot's matches, your own Recharged stays yours). The port's
  own work is CC0. Its third-party notices are in the build's `LICENSES` folder. The reconstructed game code
  and the game's trademarks belong to their owners.
- GoldBot kit only: the current champion as an ONNX file, plus a portable Python (PSF license) with
  NumPy, ONNX Runtime, pydantic, PyYAML and Gymnasium (each under its own license, included with it).

The kits are for playing and recording with GoldBot. They are not meant for redistribution.
