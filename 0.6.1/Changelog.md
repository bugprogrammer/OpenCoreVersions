OpenCore Changelog
==================
#### v0.6.1
- Improved recognition of early pressed hotkeys, thx @varahash
- Made DMG loading support configurable via `DmgLoading`
- Added iMac20,1 and iMac20,2 model codes
- Fixed display name for older Xeon CPUs like Xeon E5450
- Added kext injection support without kernel caches
- Added Comet Lake-LP HDA device code
- Fixed OS boot selection on SATA controllers with legacy OPROMs
- Fixed RSDP ACPI table checksum recalculation
- Added immutablekernel loading support for 10.13+
- Fixed solving some symbols to zero in 11.0 kext inject
- Reduced OpenCanopy size by restricting boot management access
- Added `BuiltinText` variant for `TextRenderer` for older laptops
- Fixed `SyncRuntimePermissions` creating invalid MAT table
- Added EFI FAT image loading support (macOS 10.8 and earlier)
- Added 64-bit cacheless kext injection and patching support (macOS 10.9 and earlier)
- Added 64-bit mkext kext injection and patching support (macOS 10.6 and earlier)
- Fixed XNU hook matching non-kernel files
- Updated builtin firmware versions for SMBIOS and the rest
- Fixed patching of ACPI tables in low memory
- Fixed macOS 11.0 DMG recovery loading without hotplug