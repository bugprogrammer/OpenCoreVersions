OpenCore Changelog
==================

#### v0.5.0
- Added builtin firmware versions for new models 2019
- Fixed LogoutHook leaving random directories in `$HOME`
- Fixed FSBFrequency calculation on Xeon Scalable CPUs (thx @mrmiller)
- Fixed ARTFrequency specifying on Intel server and atom models
- Increased log size to 256 KB by default
- Added `ReplaceTabWithSpace` quirk to improve Shell experience
- Added `ClearScreenOnModeSwitch` quirk to avoid visual glitches
- Added `MISC_PWR_MGMT` patch to `AppleXcpmExtraMsrs` quirk (thx @mrmiller)
- Added `DevirtualiseMmio` quirk to `Booter` section
- Added FileVault 2 user interface protocols formerly in AppleUiSupport
- Improved kernel patch logging to include configuration comments
- Added MSFT basic data and Linux root fs recognition to `ScanPolicy`
- Fixed RT region protection restoration regression (thx Sniki)
- Added `OPT`, `CMD+R`, `CMD+OPT+P+R` boot action hotkey support
- Added `PollAppleHotKeys` to register boot.efi hotkeys in the picker
- Added `DisableSingleUser` quirk to prohibit single user mode
- Upgraded EDK II base package to edk2-stable201908
- Prohibited argument changing by BootNext
