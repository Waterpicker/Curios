# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this project adheres to [Forge Recommended Versioning](https://mcforge.readthedocs.io/en/latest/conventions/versioning/).

## [1.19.4-5.1.5.3] - 2023.05.05
### Fixed
- Fixed default curio slot texture not showing properly

## [1.19.4-5.1.5.2] - 2023.04.28
### Changed
- Updated `ru_ru` localization (thanks Heimdallr-1!) [#302](https://github.com/TheIllusiveC4/Curios/pull/302)

## [1.19.4-5.1.5.1] - 2023.04.20
### Changed
- Curios swapping will now take into account all valid slots instead of just the first valid slot
### Fixed
- Fixed duplication bug when equipping from use in the hotbar

## [1.19.4-5.1.5.0] - 2023.04.16
### Added
- Added `CurioAttributeModifierEvent` for editing curio attribute modifiers in slots [#292](https://github.com/TheIllusiveC4/Curios/issues/292)
### Changed
- Curios that can be equipped from use in the hotbar will now swap with existing curios in valid slots [#301](https://github.com/TheIllusiveC4/Curios/issues/301)

## [1.19.4-5.1.4.3] - 2023.04.06
### Fixed
- Fixed toggle visibility buttons causing menu issues when clicked [#296](https://github.com/TheIllusiveC4/Curios/issues/296)

## [1.19.4-5.1.4.2] - 2023.03.16
### Changed
- Updated to Minecraft 1.19.4
- Updated slot textures to match new Minecraft slot textures

## [1.19.3-5.1.4.1] - 2023.03.15
### Added
- Added `vi_vn` localization (thanks ZzThanhBaozZ!) [#289](https://github.com/TheIllusiveC4/Curios/pull/289)
### Changed
- Updated `it_it` localization (thanks WVam!) [#288](https://github.com/TheIllusiveC4/Curios/pull/288)
### Fixed
- Fixed crashes when slots get resized to negative amounts dynamically

## [1.19.3-5.1.4.0] - 2023.02.27
### Added
- Added `/curios drop` command for dropping curio items
### Changed
- Updated `zh_cn` localization (thanks WadjetSama!) [#285](https://github.com/TheIllusiveC4/Curios/issues/285)
- Updated `it_it` localization (thanks WVam!) [#284](https://github.com/TheIllusiveC4/Curios/pull/284)
### Fixed
- Fixed curio entity selectors counting slots with size 0 erroneously

## [1.19.3-5.1.3.1] - 2023.02.15
### Fixed
- Fixed `SlotModifiersUpdatedEvent` not always firing

## [1.19.3-5.1.3.0] - 2023.02.13
### Added
- Added `SlotModifiersUpdatedEvent` to listen for broadcasted dynamic changes to slot sizes on players due to slot
modifiers [#276](https://github.com/TheIllusiveC4/Curios/issues/276)
- Added two commands:
  - `/curios replace <slot> <index> <player> with <item> [count]` for setting items to curio slots
  - `/curios list` for listing all registered slots and which mods they come from [#261](https://github.com/TheIllusiveC4/Curios/issues/261)
- Added `ICuriosHelper#setEquippedCurio` and `ICuriosHelper#findCurio()` for setting items into curio slots and getting
items from curio slots respectively
### Changed
- `ICurio#onEquipFromUse` now fires when items are placed into slots in inventory screens
### Fixed
- Fixed equip sounds not playing properly in the Curios screen (thanks bconlon!) [#281](https://github.com/TheIllusiveC4/Curios/pull/281)

## [1.19.3-5.1.2.0] - 2023.01.09
### Added
- Added new `ICurio#canWalkOnPowderedSnow` method for curio implementations that allow walking on Powdered Snow blocks
  (thanks bconlon!) [#273](https://github.com/TheIllusiveC4/Curios/pull/273)

## [1.19.3-5.1.1.2] - 2022.12.08
### Fixed
- Fix version requirements for Minecraft and Forge

## [1.19.3-5.1.1.1] - 2022.12.08
### Changed
- Updated to Minecraft 1.19.3
- Updated to Forge 44.0.0+
- Updated Portuguest (pt_br) localization (thanks FITFC!) [#265](https://github.com/TheIllusiveC4/Curios/pull/265)
### Removed
- Removed JEI integration temporarily until the mod is ported to 1.19.3

## [1.19.2-5.1.1.0] - 2022.08.08
### Added
- Re-added JEI integration
### Changed
- Updated to Minecraft 1.19.2
- Updated to Forge 43.0.0+
- Updated Polish (pl_pl) localization (thanks Greg-21!) [#247](https://github.com/TheIllusiveC4/Curios/pull/247)
- Updated Ukranian (uk_ua) localization (thanks Sushomeister!) [#245](https://github.com/TheIllusiveC4/Curios/pull/245)

## [1.19.1-5.1.0.5] - 2022.07.28
### Changed
- Updated to Minecraft 1.19.1
- Updated to Forge 42.0.0+

## [1.19-5.1.0.4] - 2022.07.11
### Changed
- Updated to and requires Forge 41.0.94+

## [1.19-5.1.0.3] - 2022.07.10
### Changed
- Updated to and requires Forge 41.0.64+
### Removed
- Temporarily removed JEI integration as the mod is not compatible currently with the required versions of Forge

## [1.19-5.1.0.2] - 2022.06.20
### Added
- Re-added JEI integration
### Fixed
- Fixed datapack functions failing to load when utilizing Curios slot commands [#240](https://github.com/TheIllusiveC4/Curios/issues/240)
- Fixed null attributes crashing clients when hovering over curio tooltips [#242](https://github.com/TheIllusiveC4/Curios/issues/242)

## [1.19-5.1.0.1] - 2022.06.09
### Changed
- Revert `CurioSlot` patch
- Updated to and requires Forge 41.0.8+

## [1.19-5.1.0.0] - 2022.06.07
### Changed
- Updated to Minecraft 1.19+
- Updated to Forge 41+
