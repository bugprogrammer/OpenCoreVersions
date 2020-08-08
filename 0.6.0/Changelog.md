OpenCore Changelog
==================

#### v0.6.0
- Fixed sound corruption with AudioDxe
- Fixed icon choice for Apple FW update in OpenCanopy
- Fixed APFS driver loading on Fusion Drive
- Added Comet Lake HDA device code
- Fixed audio stream position reporting on non-Intel platforms
- Added `Firmware` mode to `ResetSystem` to reboot into preferences
- Replaced `BlacklistAppleUpdate` with `run-efi-updater` NVRAM variable
- Fixed reset value and detection in `FadtEnableReset` ACPI quirk
- Fixed freezes during boot option expansion with PXE boot entries
- Updated underlying EDK II package to edk2-stable202005
- Added `ProvideMaxSlide` quirk to improve laptop stability, thx @zhen-zen
- Fixed slide choice on platforms when 0 slide is unavailable, thx @zhen-zen
- Fixed assertions caused by unaligned file path access in DEBUG builds
- Renamed `ConfigValidity` utility to `ocvalidate` for consistency
- Added `GlobalConnect` for APFS loading to workaround older firmware issues
- Added 11.0 support for `AvoidRuntimeDefrag` Booter quirk
- Fixed 11.0 lapic kernel quirk as of DP1
- Improved boot selection scripts for macOS without NVRAM
- Added UGA protocol compatibility in `ProvideConsoleGop` quirk
- Added `UgaPassThrough` option to support UGA protocol over GOP
- Added `AppleFramebufferInfo` protocol implementation and override
- Fixed serial initialisation when file logging is disabled
- Fixed FSBFrequency reporting on Meron and similar CPUs
- Fixed incorrect volume icon dimension requirements in OpenCanopy
- Added preview version of KernelCollection injection code
- Fixed ACPI reset register detection in DxeIpl
- Added MacBookPro16,4 model code
- Updated builtin firmware versions for SMBIOS and the rest
- Fixed OSXSAVE reporting when emulating CPUID on newer CPUs
- Added `SerialInit` option to perform serial initialisation separately
- Fixed OpenDuetPkg booting on Intel G33 with SATA controller in RAID mode
- `PlatformInfo` `Automatic` for all models
- Fixed 32-bit OpenDuetPkg booting on machines with over 4 GBs of RAM
- Fixed delays with OpenDuetPkg booting with certain SATA controllers in IDE mode
- Fixed display name for some high core count i9 CPUs like 7920X
- Fixed SSDT-EC-USBX