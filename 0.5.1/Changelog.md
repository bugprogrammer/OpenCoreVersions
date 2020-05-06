OpenCore Changelog
==================

#### v0.5.1
- Added support of kernel resource kext injection
- Added support for 0.25% clock slowdown on Xeon Scalable CPUs (thx @mrmiller)
- Replaced `MatchKernel` with `MinKernel` and `MaxKernel`
- Added `Arguments` to `Tools` and `Entries` sections
- Fixed broken timer for 300 series Intel chipsets
- Added `Input` section for mouse and keyboard aggregation
