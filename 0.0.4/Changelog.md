OpenCore Changelog
==================

#### v0.0.4
- Fixed kext injection issues with dummy dependencies
- Fixed kext injection issues with reused vtables
- Fixed Custom SMBIOS table update patches
- Added timestamp to the log file and changed extension to txt
- Enhanced `LogoutHook` script used for emulated NVRAM saving
- Fixed multiple operating system support in APFS containers
- Added `AvoidHighAlloc` UEFI quirk to avoid high memory allocs
- Updated builtin firmware versions for 10.15 beta support
- Added `Booter` section for Apple bootloader preferences
- Dropped `AptioMemoryFix.efi` support for `Booter` and `FwRuntimeServices.efi`
- Fixed hibernation issues in Windows with `RequestBootVarRouting`
- Significantly improved boot stability on APTIO
- Added support for Windows & OpenCore on the same drive through `BlessOverride`
- Added advanced user-specified boot entries through `Misc` -> `Entries`
- Added `DisableVariableWrite` quirk to disable hardware NVRAM write in macOS
