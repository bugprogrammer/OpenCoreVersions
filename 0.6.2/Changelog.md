OpenCore Changelog
==================
#### v0.6.2
- Updated builtin firmware versions for SMBIOS and the rest
- Added `ProcessorType` option to `Generic` allowing custom CPU names
- Fixed `UnblockFsConnect` option not working with APFS JumpStart
- Added IA32 binary variant to the release bundles
- Fixed improper handling of cacheless kexts without an Info.plist
- Fixed improper calculation of kext startup address for blocking
- Added mkext 32-bit kext injection (10.4-10.6)
- Added cacheless 32-bit kext injection (10.4-10.7)
- Added 32-bit kernel/kext patching/blocking support
- Fixed issues loading 10.7 EfiBoot
- Added `Type` to `ReservedMemory` to fulfil hibernation hack needs
- Added workaround to displaying `Preboot` instead of `Macintosh HD`
- Added prelinkedkernel 32-bit kext injection (10.6-10.7)
- Added `SystemMemoryStatus` to override memory replacement on some models
- Added older Pentium CPU recognition in SMBIOS 
- Added `ExtendBTFeatureFlags` to properly set `FeatureFlags` for Bluetooth (which substitutes BT4LEContinuityFixup) 
- Added `MinKernel`/`MaxKernel` to CPUID emulation and `DummyPowerManagement`
- Fixed `-legacy` not being added in `KernelArch` `Auto` mode
- Fixed `i386-user32` not forcing `i386` on macOS 10.7 on X64 firmwares
- Fixed `i386-user32` being incorrectly enabled in macOS 10.4, 10.5, and 10.7
- Disabled prelinked boot for macOS 10.4 and 10.5 in `KernelCache` `Auto` mode
- Fixed `macserial` compatibility with iMac20,x serials and other models from 2020
- Added `LegacyCommpage` quirk to improve pre-SSSE3 userspace compatibility
- Fixed legacy SATA HDDs displaying as external drives in the picker