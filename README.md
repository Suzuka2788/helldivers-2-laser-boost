# Suzuka‘s Laser Boost v1.0.0

Laser weapon enhancements for Helldivers 2 in one Bingus Shared Loader addon.

[Download v1.0.0](https://github.com/Suzuka2788/helldivers-2-laser-boost/releases/tag/v1.0.0)

| Weapon | Normal / durable damage | Armor penetration |
| --- | --- | --- |
| LAS-16 Sickle / LAS-17 base projectile | 120 / 36 | Unchanged |
| LAS-17 heat stages | 110 / 30, 140 / 42, 140 / 42 | Unchanged |
| LAS-5 Scythe / LAS-22 shared beam | 600 / 600 | 3 / 3 / 3 / 0 |
| LAS-98 Laser Cannon / A/LAS-98 Laser Sentry | 600 / 600 | 5 / 5 / 5 / 5 |

## Installation

1. Use Bingus Shared Loader v15 or newer (API 1).
2. Disable older standalone Sickle, Scythe and Cannon/Sentry boost packages and older combined versions.
3. Keep Suzuka‘s Shotgun Boost enabled; its verified settings-table locations are reused without a full memory scan. A compatible AR Family addon can also provide tables through its runtime state.
4. Install the release ZIP, deploy and fully restart the game.

## Compatibility

Beam changes are guarded for game DLL SHA-256 `2e2c3b7c2500646dadd5f2b4c6e0504dbb7e7896139f64cddc0d1813c718f51e`. Updates may require a revision. Baseline records are checked and writes read back.

Preview3 reported all three groups applied in the 2026-09-27 runtime logs. v1.0.0 changes branding and log identifiers while preserving damage values and targets. Combined write, restore and refusal tests pass; these checks do not replace in-game damage measurements.

The Cannon/Sentry row is also used by an internal beam component labelled E/MG-101 HMG Emplacement (Laser). Ordinary HMG projectile records are not modified.

Logs: `%LOCALAPPDATA%\CowboyBingus\Helldivers2\Logs`. `SuzukasLaserBoost.log` reports `APPLIED_ALL` after all groups write and verify. Details: `SuzukaSicklesDamageAdaptive.log`, `SuzukaLAS5ScytheBoost.log`, `SuzukaLAS98BeamBoost.log`.

This repository provides release packages and documentation, not the local development source tree.

## Credits

[Bingus Shared Loader](https://github.com/CowboyBingus/BingusSharedLoader) and [FileDiver](https://github.com/xypwn/filediver).
