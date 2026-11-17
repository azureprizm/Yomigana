# Third-Party Notices

Yomigana's original work is copyright (c) 2026 Joshua Holmes (AzurePrizm).
The Yomigana Restricted-Use License applies only to that original work.
It does not replace or limit the licenses of the components below.

## Scope

This inventory covers the declared mod/build/test dependencies and third-party
APIs directly imported by Yomigana, inspected on 2026-11-17. It is not a license
inventory of the entire Minecraft installation, JDK, or every transitive build
tool dependency. Version numbers refer to this development build, not a promise
about future Minecraft installations.

The mod build uses no dependency shading or `include` declarations. These
libraries are external dependencies, not licensed as part of Yomigana's original
code. The release JAR must be checked for embedded libraries before each release.
Do not distribute the development cache, Minecraft client, JDK, or Gradle
distribution as part of the mod.

## Runtime and Integration Dependencies

| Component | Version inspected | License | Evidence / upstream |
| --- | --- | --- | --- |
| Minecraft: Java Edition | 26.2 | Proprietary Minecraft EULA and applicable usage guidelines | [EULA](https://www.minecraft.net/en-us/eula); supplied by the player's installation |
| Fabric Loader | 0.19.3 | Apache-2.0 | `LICENSE_fabric-loader` in the cached Loader JAR; [project](https://github.com/FabricMC/fabric-loader) |
| Fabric API | 0.155.2+26.2 | Apache-2.0 | `LICENSE-fabric-api` in the cached API JAR; [project](https://github.com/FabricMC/fabric-api) |
| Mod Menu (optional integration) | 20.0.2 | MIT | `LICENSE_modmenu` in the cached JAR, copyright (c) 2018-2020 Prospector; [project](https://github.com/TerraformersMC/ModMenu) |
| ICU4J (Minecraft runtime, kana/romaji conversion) | 78.3 | Unicode-3.0; retain any accompanying third-party notices | Cached `icu4j-78.3.pom`; [version-family license](https://raw.githubusercontent.com/unicode-org/icu/maint/maint-78/LICENSE) |
| Gson (Minecraft runtime, configuration JSON) | 2.14.0 | Apache-2.0 | Cached `gson-parent-2.14.0.pom`; [project](https://github.com/google/gson) |
| SLF4J API (runtime logging) | 2.0.17 | MIT | `META-INF/LICENSE.txt` in the cached JAR, copyright (c) 2004-2022 QOS.ch Sarl; [project](https://www.slf4j.org/) |
| Sponge Mixin (Fabric fork, injection infrastructure) | 0.17.3+mixin.0.8.7 | MIT | `LICENSE.txt` in cached `sponge-mixin` JAR; [upstream](https://github.com/SpongePowered/Mixin) |
| MixinExtras (Fabric runtime) | 0.5.4 | MIT | `LICENSE_MixinExtras` in cached JAR, copyright (c) 2022-present LlamaLad7; [project](https://github.com/LlamaLad7/MixinExtras) |

## Development and Tests Only

| Component | Version inspected | License / evidence |
| --- | --- | --- |
| Fabric Loom | 1.17.20 | MIT; [1.17 branch license](https://raw.githubusercontent.com/FabricMC/fabric-loom/dev/1.17/LICENSE), copyright (c) 2016 FabricMC |
| Gradle and wrapper | 9.5.1 | Apache-2.0 for Gradle; wrapper script headers and local distribution `LICENSE`. The distribution's additional components retain their own notices. |
| JUnit Jupiter / JUnit Platform | 5.13.4 / 1.13.4 | EPL-2.0; cached Jupiter POM and JAR `META-INF/LICENSE.md` / `LICENSE-notice.md`. Test dependencies are not shipped in the mod. |

The Gradle wrapper is third-party material in the private source tree. Its
original Apache license headers are retained; it is not covered by Yomigana's
custom license. The local Java toolchain and other build tools likewise retain
their own terms and are not part of the public information-only showcase.

## License Obligations

This table identifies licenses; it is not a substitute for their full texts.
If external components are later bundled or redistributed, audit that new
package first and supply the actual required license texts and notices:

- MIT components require retention of their copyright and permission notices.
- Apache-2.0 components require the license, applicable attribution/NOTICE
  material, and notices of modifications where required.
- Unicode-3.0 components require their copyright and permission notices; keep
  additional notices accompanying the specific ICU distribution.
- EPL-2.0 redistribution has license, notice, and source-availability obligations
  for covered material. Do not treat a credit as satisfying them.
- Minecraft code/assets may not be redistributed merely because a mod depends
  on them. Follow Mojang/Microsoft terms separately.

These statements describe upstream terms, not new permissions from Joshua
Holmes to redistribute Yomigana or third-party material.

## Inspiration and Separate Materials

The classic Rubi markup format inspired compatibility with `§^base(ruby)`.
This acknowledgment is not a claim to Rubi's code or a license to copy it.
Any incorporated third-party source would require its own provenance and
license review. The current authorship basis is the creator's statement that
Yomigana is original work with no outside human contributors; it is not an
independent legal certification of provenance.

Third-party code, tools, dependencies, and resource packs retain their respective
copyright notices and licenses. These project credits do not replace those notices.
Separately installed resource packs are not relicensed by this change.

Minecraft is a product of Mojang Studios. Yomigana is an independent project
and is not an official Minecraft product.
