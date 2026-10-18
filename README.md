# GoldBot kits

GoldBot is a self-learning bot for *Mario Strikers Charged*, playing on the native PC port
([Recharged](https://github.com/previouslevelgames/recharged)). This repository only carries the
kits for the people who play against it or record their matches for it. The bot's code is not public.

## Download

| Kit | What it is for | Start |
|---|---|---|
| [goldbot-kit.zip](https://github.com/GoldCobra/GoldBot-Kit/releases/latest/download/goldbot-kit.zip) | Play against GoldBot offline, in real time. Your matches are packed into one zip for GoldCobra. | `play-goldbot.cmd` |
| [goldbot-demo-kit.zip](https://github.com/GoldCobra/GoldBot-Kit/releases/latest/download/goldbot-demo-kit.zip) | Record your own matches (alone against the CPU or against a friend). | `record-demos.cmd` |

Unpack the zip anywhere (not into *Program Files*) and start the `.cmd` file. The kit's README explains
the rest. Windows 10 or 11 (x64) is needed.

## Which disc

Use the European **Mario Strikers Charged Football, `R4QP01` revision 2**. GoldBot trains and is measured
on it, so the bot plays its best there and your matches fit its training best. Revision 1 and the USA disc
(`R4QE01`) work too; every recorded match names the disc it was played on.

## Updates

Releases are named by the bot's version: GoldBot V5.2 is champion V5 in its third kit release, and V6.0
will bring the next champion.

Each kit checks this repository at every start. When a newer release is out, it downloads that release,
checks its SHA-256, and replaces its own files in place. Your player name, disc image, controller settings,
recordings and any zips you have not sent yet stay where they are. This way everyone plays the same game
build and the same bot. GoldCobra only takes matches that were recorded with the newest kit. Without an
internet connection the kit still plays, so update the next time you are online.

## What is inside, and what is not

- **No game data.** You need your own *Mario Strikers Charged* disc image (Wii); see "Which disc".
- A build of Recharged, the PC port, with GoldBot's bridge and recorder. The port's own work is CC0. Its third-party
  notices are in the build's `LICENSES` folder. The reconstructed game code and the game's trademarks
  belong to their owners.
- GoldBot kit only: the current champion as an ONNX file, plus a portable Python (PSF license) with
  NumPy, ONNX Runtime, pydantic, PyYAML and Gymnasium (each under its own license, included with it).

The kits are for playing and recording with GoldBot. They are not meant for redistribution.
