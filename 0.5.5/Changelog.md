OpenCore Changelog
==================

#### v0.5.5
- Fixed CPU bus ratio calculation for Nehalem and Westmere
- Fixed CPU package calculation on MacPro5,1 and similar
- Improved OpenCore rerun detection for new versions
- Fixed loading picker on boot failure when it is hidden
- Added PMC ACPI sample for 300-series chipsets
- Improved driver connection performance on APTIO IV
- Fixed boot option saving in LogoutHook.command
- Added support for OEM information in `ExposeSensitiveData`
- Improved `SanitiseClearScreen` to avoid mode switching
- Replaced `SupportsCsm` with `AdviseWindows` enabling UEFI mode
- Fixed issues with default boot path selection on some boards
- Update builtin firmware versions
- Fixed `AdviseWindows` not setting `FirmwareFeatures` in NVRAM
- Added `TakeoffDelay` option for improved action hotkey support
- Added Mac GOP support to `ProvideConsoleGop` quirk
- Added experimental `BuiltinTextRenderer` boot option
- Added `DummyPowerManagement` kernel quirk to disable CPU PM
