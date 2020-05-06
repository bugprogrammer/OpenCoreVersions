OpenCore Changelog
==================

#### v0.5.8
- Fixed invalid CPU object reference in SSDT-PLUG
- Fixed incorrect utilities and resources packaging
- Fixed `Custom` `UpdateSMBIOSMode` modifying SMBIOSv3 table
- Updated docs to cover separating SMBIOS via `UpdateSMBIOSMode`
- Fixed rendering macOS installer icons in OpenCanopy
- Added APFS support with Fusion Drive and enhanced security
- Added AppleEvent mouse support in OpenCanopy
- Fixed AppleEvent and OpenCanopy compatibility with OVMF TPL restrictions
- Added mouse drivers to the package as OVMF needs one
- Added memory region reservation support
- Added RtcRw tool to manipulate RTC memory
- Added `PatchAppleRtcChecksum` kernel quirk
- Added `AppleRtcRam` protocol implementation
- Renamed `Protocols` to `ProtocolOverrides` for clarity
- Added ResetSystem tool to allow shutdown/reset actions in the menu
- Added experimental `BootProtect` `Security` option
- Fixed kext injection in 10.8 installer
- Added timeout support to OpenCanopy user interface
- Fixed handling 24-bit screen resolutions
- Added `Ps2KeyboardDxe` driver for DuetPkg
- Updated `BootInstall` DuetPkg version (now opensource)
- Added partial HiDPI support in OpenCanopy
- Update builtin firmware
- Fixed invalid checksum checks when creating vault (thx @dakanji)
