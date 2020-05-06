OpenCore Changelog
==================
#### v0.5.4
- Added Enter key handling in boot menu for quick proceed
- Update builtin firmware versions
- Bundled FwRuntimeServices driver with OpenCore
- Allowed writing to non-volatile variables with disabled write
- Fixed microcode reading on Intel CPUs
- Fixed SMBIOS Type4 External Clock values
- Improved Windows compatibility on some setups (acidanthera/bugtracker#614)
- Added `SupportsCsm` and option in `PlatformInfo/Generic`
- Added `OSInfo` protocol support
- Added `SignalAppleOS` `Booter` quirk to enable IGPU on Macs in other OS
- Added `AppleSmcIo`protocol support (replaces `VirtualSmc` UEFI driver)
- Added `AuthRestart` security property for VirtualSMC authenticated restart
- Fixed input protocol initialisation on VMware fusion
- Added arrow key handling in boot menu
- FileVault 2-like key input is now the only supported input in boot menu
- Fixed 5 second delay when exiting Shell to OpenCore Picker
- Added default boot option update and `AllowSetDefault` `Security` option
- Fixed CPU package detection on configurations with multiple CPUs
- Bundled CleanNvram and VerifyMsrE2 tools for debugging
- Added screen clearing after choosing boot entry in picker
- Added `WriteFlash` NVRAM option to enable writing variables in `Add`
- Added `LegacyOverwrite` NVRAM option to allow overwriting variables by nvram.plist
- Added `AppleXcpmForceBoost` kernel quirk to maximise select Xeon performance
- Bundled NvmExpressDxe and XhciDxe drivers for platforms that need them
- Added `IncreasePciBarSize` kernel quirk for select platforms with PCI space issues
