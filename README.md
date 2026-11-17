# Yomigana

**Japanese reading support for Minecraft: Java Edition.** Yomigana is a client-side Fabric mod for Minecraft 26.2. It places small kana readings (furigana) above Japanese words, so you can see how to pronounce a word without replacing its kanji.

For example, a sword named **剣** can show **けん** above it and **ken** below it. With the Japanese Learning Pack's bilingual option, an item can also keep its English name alongside the Japanese.

## What it looks like in play

- **Inventory:** Hover over an item or a Creative tab to see its readings. You can still search for an item in English, such as `diamond sword`, while playing in Japanese.
- **Chat, signs, and books:** Add a reading with `§^剣(けん)`. In supported displays, the reader sees the kanji and its pronunciation instead of the markup.
- **Reading preferences:** Place furigana above or below the base text, replace the base with its reading, or hide the reading. In Above mode, an optional romaji line helps learners who are still getting comfortable with kana.
- **Writing:** Kana conversion lets you turn roman letters such as `ken` into **けん** or **ケン** using a standard English keyboard.

Yomigana displays readings supplied by the text or resource pack. It does not guess the pronunciation of arbitrary kanji or automatically translate player-written messages.

## Project status

In development. The Minecraft 26.2 build has been demonstrated in-game with the Japanese Learning Pack. This repository is an **information-only showcase**; it does not distribute the mod, its source code, or the resource pack.

Created and maintained by [Joshua Holmes (AzurePrizm)](https://github.com/azureprizm).

Official project: [AzurePrizm/Yomigana](https://github.com/azureprizm/Yomigana).

See the [showcase copyright notice](LICENSE.md) and the
[Yomigana Restricted-Use License, Version 1.0](MOD-LICENSE.md).
The mod uses a custom restricted-use license, not an open-source license.
Authorized gameplay, personal modpacks, and gameplay videos or streams are
permitted; modification and redistribution require prior written permission.
This page does not provide a download or grant paid-distribution rights.

The classic Rubi markup inspired Yomigana's annotation compatibility. Yomigana
uses Fabric Loader, Fabric Loom, and Fabric API; Mod Menu provides access to
configuration, and ICU4J provides kana transliteration through Minecraft's runtime.
These credits do not replace third-party notices or licenses.

Copyright (c) 2026 Joshua Holmes (AzurePrizm). All Rights Reserved.
