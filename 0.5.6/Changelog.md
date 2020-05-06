OpenCore Changelog
==================

#### v0.5.6
- Various improvements to builtin text renderer
- Fixed locating DMG recovery in APTIO IV firmwares on FAT32
- Fixed loading DMG recovery in APTIO IV firmwares on FAT32
- Removed `AvoidHighAlloc` quirk due to removed I/O over 4GB
- Moved `ConsoleMode`, `Resolution` options to `Output` section
- Moved console-related UEFI quirks to `Output` section
- Replaced `ConsoleControl` and `BuiltinTextRenderer` with `TextRenderer`
- Removed `ConsoleBehaviourOs` and `ConsoleBehaviourUi`
- Fixed providing ConsoleOutHandle GOP when running from Shell
- Added `PickerAttributes` option to colour picker
- Added `ProtectSecureBoot` option through FwRuntimeServices
- Replaced `RequireVault` and `RequireSignature` with `Vault`
- Added `BootKicker` tool to support launching Apple BootPicker
- Added BootPicker support as an external UI in OC through `PickerMode`
- Added `DirectGopRendering` option to use direct GOP output
- Multiple memory corruption and performance fixes for PNG support
- Fixed `DefaultBackgroundColor` variable handling
- Added `HideAuxiliary` and `Auxiliary` options
- Fixed picker timeout and log timestamps for VMware
- Fixed NULL parent DeviceHandle for launched tools
- Added bundled HiiDatabase driver for very old firmwares
- Added SSE2 support in memory intrinsics for better performance
- Improved ACPI PM timer CPU frequency calculation performance
- Improved LapicKernelPanic compatibility with newer macOS versions
- Fixed drivers starting with `#` not being skipped
- Added audio support through AudioDxe with optional boot chime
- Added VoiceOver accessability support in boot.efi for 10.13+
- Added `PickerAudioAssist` option for audio assistance in picker
- Added `HdaCodecDump.efi` tool in default package
- Added legacy AudioDxe and Microsoft namespaces to Reset NVRAM
- Merged `OcSupportPkg` with `OpenCorePkg` for easier bisection
- Disabled warnings in release versions of NVMe and XHCI drivers
