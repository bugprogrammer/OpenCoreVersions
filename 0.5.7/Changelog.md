OpenCore Changelog
==================

#### v0.5.7
- Added TimeMachine detection to picker
- Added early preview version of OpenCanopy
- Fixed FS discovery on NVMe with legacy drivers
- Added `DirectGopCacheMode` option for FB cache policy
- Added `KeyFiltering` option to workaround buggy KB drivers
- Added tool and custom entry separation in audio assistant
- Added `OpenControl` tool to configure full NVRAM access from Shell
- Added `boot.efi` debug protocol support for 10.15.4+
- Added `boot.efi` performance logging for 10.15.4+
- Added `ProtectUefiServices` quirk to fix `DevirtualiseMmio` on Z390
- Replaced `BOOTCAMP Windows` with `Windows` to match the original
- Added bundled `OpenShell` originally available as OpenCoreShell
- Rework `readlabel` utility into `disklabel` with encoding support
- Renamed `FwRuntimeServices` driver to `OpenRuntime`
- Renamed `AppleUsbKbDxe` driver to `OpenUsbKbDxe`
- Update builtin firmware
- Fixed `PowerTimeoutKernelPanic` on 10.15.4
- Fixed 4K section alignment in `OpenRuntime` to fix Linux booting on SKL
- Introduced `SyncRuntimePermissions` to fix multiple memory permission flaws
- Introduced `RebuildAppleMemoryMap` to fix macOS booting on Dell 5490
- Removed `ShrinkMemoryMap` in favour of more advanced `RebuildAppleMemoryMap`
- Marked `EnableWriteUnprotector` as deprecated on modern systems
- Introduced `ProtectMemoryRegions` to fix memory region handling
- Removed `ProtectCsmRegion` in favour of `ProtectMemoryRegions`
- Renamed `PickerAttributes` to `ConsoleAttributes`
- Introduced `PickerAttributes` as a matter of UI configuration
