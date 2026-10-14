# Wildlife Park Modern Patch

Community patch research and tools for **Wildlife Park Gold** and the **Wild Creatures** expansion. Current patch snapshot: **0.38.2**.

## Features

- Widescreen resolution choices and wider interface artwork.
- Fullscreen focus recovery, launcher transitions and startup audio fixes.
- Windowed gameplay cursor confinement.
- Timestamped default save names and action feedback.
- Consistent real-time repeat timing for price and work-area buttons.
- Expanded rain/snow artwork and a 50% minimum zoom in Wild Creatures.
- Calendar pacing correction at higher TPS.
- Main-menu logos that switch between the games and glow on hover.
- Native F2 panel with shortcuts, scrolling, cheat/weather controls and landscape switching.

The experimental debug HUD, console and developer-mode controls were reverted. Their research remains in the history.

## Source download

Download and extract `wildlife-park-modern-patch-source-0.38.2.zip` from this repository to access the full source tree and research archive.

## Repository contents

`tools/` contains Python patch builders, asset utilities, historical installers and native regression checks. `analysis/` records investigations and verification metadata. `docs/` preserves the development and version history; earlier notes describe intermediate builds and may have stale paths or status statements. `VERSION` identifies the latest workspace snapshot.

This initial source publication is a research archive, **not a one-click installer**. A complete rebuild requires exact original and intermediate files, local path configuration and version-specific inputs that are not included here. Owning a compatible copy of the game is required. Do not run historical install/rollback scripts against an arbitrary installation.

## Development environment

The scripts use Python 3, `pefile` and Pillow. Many builders and native checks also need GNU binutils (`as`, `ld`, `objcopy`, `objdump`, `nm`) and a Linux environment able to execute 32-bit x86 test programs. Some optional utilities use Wine or FFmpeg. Local installation paths in the published archive have been replaced with placeholders.

```sh
python3 -m venv .venv
. .venv/bin/activate
python -m pip install -r requirements.txt
```

## Compatibility and status

Development used the German Wildlife Park Gold installation with both executables. Other editions and languages have not been verified. 0.38.2 changes only the F2 caption height relative to 0.38.1; the two executables each passed exact one-byte preservation checks. Broader game behavior was checked during the development history, with remaining limitations recorded in the reports.

Original game executables, packed game assets, music, saves, local logs and backup builds are excluded from this repository. Wildlife Park and its original assets belong to their respective rights holders. This project is unofficial.

## License

The community patch source is published under GPL-3.0; see `LICENSE`. This does not grant rights to the original game or its assets.
