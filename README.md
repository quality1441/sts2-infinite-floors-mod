# Infinite Floors

A mod for [Slay the Spire 2](https://store.steampowered.com/app/2868840/Slay_the_Spire_2/) that adds an **Infinite Floors** custom-run modifier. Clear Acts 1–3 as usual, then keep climbing through new random biomes instead of facing the Architect and ending the run.

**Tested with STS2 v0.103.3** (Early Access). New game patches may require a mod update.

## Requirements

- Slay the Spire 2 with **mods enabled** (`--enable-mods` launch flag or the in-game mods setting)
- A full restart of the game after installing or updating the mod

## Install

1. Download the latest release zip (or copy the files from this folder).
2. Extract or copy into your STS2 mods folder:

   ```
   <Slay the Spire 2 install>\mods\Sts2InfiniteFloors\
   ```

   Example (Steam default):

   ```
   C:\Program Files (x86)\Steam\steamapps\common\Slay the Spire 2\mods\Sts2InfiniteFloors\
   ```

   This folder must contain:

   - `Sts2InfiniteFloors.dll`
   - `Sts2InfiniteFloors.json`
   - `README.md` (optional but included in releases)

3. **Fully quit and restart Slay the Spire 2.** Updating the DLL while the game is running will not apply changes.

4. On the main menu, confirm mods are loaded (you should see a modded indicator if your build shows one).

## How to play

1. Start a **Custom Run**.
2. Select the **Infinite Floors** modifier.
3. Play through Acts 1–3 normally.
4. After the Act 3 boss, the run continues into Act 4+ with a random **Hive** or **Glory** biome (and more acts after each act boss).
5. Watch the map top bar for **Act N | Floor X** — floor count drives difficulty.
6. Only the **act boss node** at the top of the map advances to the next act. Other fights return you to the map.
7. The run ends when you die (including after Act 3 — you meet the Architect on death instead of an instant game-over screen in the normal path).

## What changes as you climb

| Approx. floor | What to expect |
|---------------|----------------|
| Early infinite | More elites on the map; fewer events over time |
| 45+ | Harder monster fights (elite-tier encounters) |
| 65+ | Elite-only fights; occasional mini-boss elites; enemies gain stats over time |
| 85+ | Most fights are bosses; some bosses spawn with extra elite minions |
| 100+ | Boss pool pulls from **all act bosses**; boss fights get tougher |
| 110+ | Chance of **dual-boss** fights (two bosses at once) |
| 115+ | Boss fights gain +Strength/+Dexterity each new infinite act |

Exact thresholds are tuned in the mod; the table is a rough guide.

## Troubleshooting

**Mod does not appear in the mod list**

- Check that both `Sts2InfiniteFloors.dll` and `Sts2InfiniteFloors.json` are in `mods\Sts2InfiniteFloors\` (not loose in `mods\`).
- Fully restart the game.

**Custom Run is locked**

- The mod tries to unlock Custom Run automatically. If it stays locked, earn three Act 3 clears in normal progression, or check `%APPDATA%\SlayTheSpire2\logs\godot.log` for errors.

**Changes not applied after update**

- You must **fully exit and restart** STS2 after replacing the DLL.

**Logs**

- Windows: `%APPDATA%\SlayTheSpire2\logs\godot.log`
- In-game: press `` ` `` and type `open logs`
- Search for `Sts2InfiniteFloors` or `InfiniteFloors`

## Multiplayer

All players should run the same mod version. Infinite Floors is primarily tested in single player.

## License

Not specified. Modding STS2 is subject to Mega Crit’s modding terms.
