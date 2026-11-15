# About this fork

This repository is a fork of [bitfix](https://github.com/trumank/bitfix) by trumank (Truman Kilen; MIT license, see
[LICENSE](LICENSE)). It exists so that bitfix, with a ready package for each game, can be listed on
[openmods](https://openmods.nexus), which reads `openmods.json` and `openmods.md` from the default branch of a GitHub
repository, and so that players get one zip to unpack.

- The branch `release` starts at upstream commit
  [`80af6c231cb9bb1d441f02b3c66da3dbd4af115e`](https://github.com/trumank/bitfix/commit/80af6c231cb9bb1d441f02b3c66da3dbd4af115e)
  (2024-12-11, bitfix 0.1.0), the source of the DLL in the packages. Upstream's later commits change only the
  examples in its README.
- The bitfix code is unchanged. This fork adds only `FORK.md`, `openmods.json`, `openmods.md`, the cover image
  `docs/cover.webp`, and the game patches in `games/<game>/` (for Wuchang: Fallen Feathers:
  `games/wuchang/bitfix/sig.lua`). It is unofficial: trumank did not make it and does not support it.
- The release `v0.1.0-80af6c23` holds:
  - `wuchang_bitfix_v0.1.0-80af6c23.zip`: the package for Wuchang: Fallen Feathers as it is used in the game, with
    the paths below the game's main folder: `Project_Plague/Binaries/Win64/d3d9.dll` and `dsound.dll` (the same
    bitfix DLL, SHA-256 `a4fee8a1a1d6b396b1335fb1226dce91ad70a8ab2995fe9dbb76ec94f59b52ea`; its log line names the
    commit `80af6c23`), `Project_Plague/Binaries/Win64/bitfix/sig.lua` (the same file as
    `games/wuchang/bitfix/sig.lua`) and `Project_Plague/Binaries/Win64/bitfix-LICENSE.txt` (bitfix's `LICENSE`,
    unchanged).
  - `SHA256SUMS.txt`.
- The DLL in the package is the tested file, not a new build of this repository.

## Changes

| Date | Version | Change | Files |
|---|---|---|---|
| 2026-11-15 | v0.1.0-80af6c23 | Fork made; openmods files, cover and the Wuchang: Fallen Feathers patch added; no code change | `FORK.md`, `openmods.json`, `openmods.md`, `docs/cover.webp`, `games/wuchang/bitfix/sig.lua` |
