OpenCore Changelog
==================
#### v0.6.3
- Added support for xml comments in plist files
- Updated underlying EDK II package to edk2-stable202008
- Provide fallbacks for NULL memory SMBIOS strings
- Fixed `BOOTx64.efi` and `BOOTIA32.efi` convention
- Fixed SMBIOS handling with multiple memory arrays
- Fixed memory array handle assignment on empty slots
- Fixed CPUID patching on certain versions of macOS 10.4.10 and 10.4.11
- Fixed incorrect core/thread counts on Pentium M processors
- Added `SSDT-UNC.dsl` ACPI sample to resolve X99 issues, thx @RemB
- Updated builtin firmware versions for SMBIOS and the rest
- Increased slide allocation reserve to 200 MB for Big Sur beta 10
- Fixed assert when trying to enable direct renderer on blit-only GOP
- Added support for custom memory properties
- Fixed intermittent 32-bit prelinking failures caused by improper Mach-O expansion
- Fixed failures in cacheless injection dependency resolution
- Fixed detection issues with older Atom CPUs
- Fixed `ScanPolicy` NVMe handling on MacPro5,1
- Fixed I/O issues on platforms incapable of reading over 1MB at once
- Fixed plist-only kext injection in Big Sur
- Add `ForceResolution` option for enabling non-default resolutions
- Fixed Ps2MouseDxe not properly loading under OpenDuetPkg
- Added workaround for read-only errors on some X299 boards
- Added support for `x86legacy` Secure Boot model
- Added missing Secure Boot NVRAM variables required by 11.0
- Added setting of `system-id` NVRAM variable
- Added `ForceSecureBootScheme` quirk for virtual machines
- Fixed kernel and ACPI patches failing to replace last bytes of memory