OpenCore Changelog
==================
#### v0.5.2
- Fixed `MinKernel` and `MaxKernel` logic (thx @dhinakg, @reitermarkus)
- Fixed ASSERT when booting non-Apple OSes without arguments from the DEBUG version
- Added `MmioWhitelist` configuration option
- Added `PowerTimeoutKernelPanic` kernel quirk
- Fixed erratic cursor appearing in release builds
- Moved `ReconnectOnResChange` to a user-configurable quirk to avoid freezes
- Added OpenCore version to picker ui, configured by `ExposeSensitiveData`
- Added hypervisor CPUID support to work with virtualization (thx @Leoyzen)
