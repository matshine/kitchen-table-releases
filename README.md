# Kitchen Table

**A virtual kitchen table for playing Magic: The Gathering with 2–6 friends, wherever they are.**

One player hosts a game and shares a short room code. Everyone else joins with it from their own
copy of the app. Then you play like you would in person: you move your own cards, and the table
keeps the game honest together. There are no accounts and no rules engine.

- **Your decks:** build them in the app's Commander deck builder, or paste a list exported from
  Moxfield, Archidekt, Arena or MTGO.
- **A real table:** a hand, library, graveyard and battlefield for each player, with drag and drop,
  tapping, counters, tokens and face-down cards. Point at cards and draw arrows on everyone's screen.
- **Life tracking built in:** life, poison, commander damage and turns, shared live with everyone.
- **Play solo** to goldfish a deck, or **Watch** a friend's game.

Free to use. Card data and images come from [Scryfall](https://scryfall.com).

## Download

**[Get the latest version](https://github.com/matshine/kitchen-table-releases/releases/latest)**,
and under **Assets** pick the file for your computer:

| Computer                             | File                                                                      |
| ------------------------------------ | ------------------------------------------------------------------------- |
| Windows 10 or 11                     | `Kitchen-Table-Setup-<version>.exe`                                       |
| Mac with Apple silicon (M1 or later) | `Kitchen-Table-<version>-arm64.dmg`                                       |
| Mac with an Intel chip               | `Kitchen-Table-<version>-x64.dmg`                                         |
| Linux (Ubuntu, Debian and others)    | `kitchen-table_<version>_amd64.deb` or `Kitchen-Table-<version>.AppImage` |

Not sure which Mac you have? Open the Apple menu → **About This Mac**: it says **Chip: Apple M…**
or **Processor: Intel**.

Everyone at the table needs the app, ideally the same version.

## Install

### Windows

1. Open `Kitchen-Table-Setup-<version>.exe`.
2. Windows may say **"Windows protected your PC"**, because the app isn't signed with a paid
   certificate yet. Click **More info**, then **Run anyway**.
3. Follow the installer. Kitchen Table is then in the Start menu.

### Mac

1. Open the `.dmg` and drag **Kitchen Table** into **Applications**.
2. The first time you open it, macOS says it can't check the app for malicious software, because
   the app isn't registered with Apple. Open **System Settings → Privacy & Security**, scroll down
   and click **Open Anyway**. (Or Control-click the app in Applications and choose **Open**.) You
   only have to do this once.
3. If macOS says the app **"is damaged and can't be opened"**, open Terminal and run the line below,
   then open the app again:
   ```
   xattr -cr "/Applications/Kitchen Table.app"
   ```

### Linux

- **The `.deb`** (Ubuntu, Debian, Mint and others): run
  `sudo apt install ./kitchen-table_<version>_amd64.deb`. Kitchen Table is then in your apps menu.
  Use this one on Ubuntu 24.04 and later.
- **The AppImage** (any distribution): make it runnable with
  `chmod +x Kitchen-Table-<version>.AppImage`, then open it.

## Getting the latest version

**On Windows and with the AppImage, the app updates itself.** When a new version is out, it
downloads it in the background while you play. A banner then says **"Kitchen Table … is ready"**:
click **Restart to update**, or **Later** and it updates the next time you close the app.

**On a Mac and with the `.deb`**, the app tells you when a new version is out, and **Download**
opens this page. Install it the same way as the first time: your decks and settings are kept.

The app updates itself from version 0.7.0. If you have an older version, download the latest one
here once.

## Playing your first game

1. Open the app and type your name.
2. Click **Build one…** to make a deck, or paste a list from another site.
3. **To host:** pick your deck and click **Host a game**. Click the room code at the top to copy it,
   and send it to your friends.
4. **To join:** pick your deck, paste the room code (or invite link) and click **Join**.
5. When everyone's in, the host clicks **Start game**.

Press **?** in the app for help with the controls.

**Can't connect?** Some school, office and hotel networks block games like this. Try another
network, or see **Network…** in the app's lobby.

## Your data

Your decks and settings are saved on your own computer, in the `Kitchen Table` folder in your
Documents. Uninstalling the app leaves them there.

Games connect the players' computers to each other directly when their networks allow it. A free
public server (PeerJS) introduces the players by room code and, on networks that need it, relays
the game's encrypted traffic.

## About this page

This repository holds Kitchen Table's installers only; every version is listed under
[Releases](https://github.com/matshine/kitchen-table-releases/releases).

Kitchen Table is unofficial Fan Content permitted under the
[Fan Content Policy](https://company.wizards.com/en/legal/fancontentpolicy). Not approved or
endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast.
©Wizards of the Coast LLC.
