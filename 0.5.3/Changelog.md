OpenCore Changelog
==================
#### v0.5.3
- Update builtin firmware versions
- Fixed interpreting letters in boot menu
- Fixed timeout abortion with PollAppleHotKeys quirk
- Fixed rare kext injection failure due to plist-only kext in prelinkedkernel
- Fixed error reporting for dmg loading
- Added various debugging improvements
- Added new crypto stack resulting in vault key format changes
- Added `UnblockFsConnect` UEFI quirk to fix missing filesystems on some laptops
- Added `RequestBootVarFallback` UEFI quirk to circumvent firmware boot option issues
- Added `ThirdPartyDrives` kernel quirk fixing SSD trim and 10.15 SATA hibernation (thx @lvs1974)
- Removed `ThirdPartyTrim` kernel quirk in favour of `ThirdPartyDrives`
- Added Intel Xeon E5 (Broadwell-EP) support (thx @crazyi)
- Switched to edk2-stable201911, which is now the minimum supportd EDK II version
- Deprecated `DiscardHibernateMap`, which is now scheduled for removal
