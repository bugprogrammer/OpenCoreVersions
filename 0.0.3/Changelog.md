OpenCore Changelog
==================

#### v0.0.3
- Added complete modern platform database (2012+)
- Added `DisableIoMapper` kernel quirk
- Fixed ACPI modification failures with nested multiboot
- Dropped `IgnoreForWindows` quirk legacy
- Added basic AMD Zen CPU support
- Added `Misc` -> `Tools` section to add third-party tools
- Added `Kernel` -> `Emulate` section for CPUID patches
- Added `CustomSMBIOSGuid` quirk for Custom SMBIOS update mode
- Added `PanicNoKextDump` quirk to avoid kext dump in panics
- Switched to EDK II stable and reduced image size
- Added `LapicKernelPanic` kernel quirk
- Added `AppleXcpmExtraMsrs` quirk and improved XCPM patches
- Added `(external)` suffix for external drives in boot menu
- Added `UsePicker` option, do enable for OC boot management
- Added nvram.plist loading for legacy and incompatible platforms
- Improved instructions for legacy and Windows installation
- Added Windows Boot Camp switching support
- Added basic hibernation detection & support
- Added `ResetHwSig` ACPI quirk to workaround hibernation
- Removed `Custom` subfolder requirement from `ACPI` tables
- Fixed kext injection in 10.7.x and 10.8.x
- Added ESP partition type detection to ScanPolicy
- Added support for third-party user interfaces
