## What's Changed

### General
* Fixed critical bug where `is_deleted` could not be found when downloading pools [#67, #60, #62].
* Blacklists can now use `score:`.
* Fixed bug where tags containing a space at the end would attempt to create invalid directories that resulted in crashes [#59, #58, #68].

### Misc
* Rolled back workflow Ubuntu version to 18.4 as the latest causes issues with OpenSSL.
* Documentation has been expanded and given more detail [#69 ... #91].
* Tons of code cleanup that are listed in the pull request (#65) below.
* Turned `Config` and `Login` into singletons for easier use and access.
* Imports are now organized across all files.
* `Grabber` now has all the code related to grabbing posts broken off into multiple functions, increasing readability greatly.
* Converted the programming workflow of the entire project to Gitflow for a more structured software development cycle (also reducing bugs from leaking into the `main` branch).

### Pull Requests
* Removed is_deleted from PoolEntry by @head-gardener in https://github.com/McSib/e621_downloader/pull/61
* Crate toml updates. by @McSib in https://github.com/McSib/e621_downloader/pull/63
* Update workflow for this branch and update crates. by @McSib in https://github.com/McSib/e621_downloader/pull/64
* Codebase cleanup by @McSib in https://github.com/McSib/e621_downloader/pull/65

## New Contributors
* @head-gardener made their first contribution in https://github.com/McSib/e621_downloader/pull/61

**Full Changelog**: https://github.com/McSib/e621_downloader/compare/1.7.1...1.7.2