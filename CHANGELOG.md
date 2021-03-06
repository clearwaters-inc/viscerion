# Release Notes

### [5.2.11] - 2020-02-09
- Follow system theme on all API levels
- Update library dependencies
- Update native dependencies
- Improve user experience with QR code flow

### [5.2.10] - 2020-01-25
- Update library dependencies
- Add Android TV support
- Fix occasional crash with tunnel stats
- Properly ensure we're not treated as a metered network
- Resolve another attack vector for biometric auth
- Update native dependencies

### [5.2.9] - 2020-01-16
- Update Chinese Simplified and German translations
- Add a rudimentary widget to toggle last used tunnel
- Allow userspace backend to restore tunnels on reboot
- Fix cancelling biometric dialog allows auth bypass
- Upgrade library dependencies

### [5.2.8] - 2020-01-11
- Workaround background service restrictions on Android 10
- Fix occasional crash with search/detail view
- Update library dependencies
- Handle case when user removes all fingerprints with biometric authentication enabled
- Match some UI aspects to the Material Design specification
- Switch completely to the new icon and remove the toggle
- Update Polish translations
- Rewrite global exclusions implementation

### [5.2.7] - 2019-12-13
- Require unlocking for using Quick Settings tile.
- Show tunnel's data usage statistics in detail fragment
- Update library dependencies
- Update French, Russian, German and Portugese translations
- Update WireGuard tools to 0.0.20191127 snapshot
- Resolve some animation related issues
- Fix global exclusions not working properly

### [5.2.6] - 2019-11-27
- Update libwg-go and build with Go 1.13.4
- Add Tasker plugin support to simplify integration (by Rafhaan Shah)
- Allow using PIN/password/pattern as fallback authentication
- Fix file descriptor leaks
- Allow Android TV devices to use file picker
- Rewrite native library loading for enhanced robustness
- Update German and French translations

### [5.2.5] - 2019-10-20
- Resolve crashes with QR import dialog on release builds

### [5.2.4] - 2019-10-19
- Fix QR code import action not working

### [5.2.3] - 2019-10-16
- Make log exporter a top-level menu item and remove viewer activity
- Resolve wg-quick segfaults on some devices

### [5.2.2] - 2019-10-16
- Fix another crash in settings

### [5.2.1] - 2019-10-13
- Fix crash in tunnel detail view

### [5.2.0] - 2019-10-12
- Add timer to wg-quick notifications
- Defer tunnel state restoration to workaround AFWall+ startup block
- Add German translations
- Update library dependencies
- Update to Golang 1.12.9 for native library
- Add ability to restrict application access using biometric authentication
- Fix constant memory leaks on Q that Google deemed too low priority.
- Allow searching through tunnels in list view
- Support kernelspace mode on Android Q.

### [5.1.1] - 2019-07-21
- Revert back to non-service Tasker integration as many devices incessantly
  kill background services thus breaking the feature entirely.

### [5.1.0] - 2019-07-19
- Target Android Q and adapt APIs for it
- Ensure dark theme follows battery saver on Android P and below
- Improve memory usage
- Improve support for FireTV remote
- Refactor app theme and convert night theme to a dark grey background
- Update Russian translations
- Switch fully to Storage Access Framework and remove WRITE_EXTERNAL_STORAGE permission
- Fix theming related glitches
- Update library dependencies
- Use a background service to improve Tasker integration reliability

### [5.0.0] - 2019-05-08
- Add an adaptive icon and an alternative concept icon
- Add live log viewer
- Ensure global exclusions are not exported with configs to prevent import bugs
- Support Magisk 19.0 and above
- Improve and speed up exclusion picker
- Improve landscape layout (Fixes Android TV not seeing all create options)
- Fix bug which caused excluded applications count to be incorrect
- Fix bug which caused settings to crash on first run
- Make app theme follow system night mode

### [4.0.0] - 2019-03-21
- Add support for Magisk 18.2
- Fix lingering theming issue with bottom sheets
- Add support for Tasker
- Automatically export configurations to external storage when upgrading
- Use a Google Messages style FAB in tunnel list
- Tweak dialog UI
- Add translations for Portuguese Brazilian and Russian
- Move theme toggle to overflow menu for easier access
- Improved speeds for ARM devices on userspace backend

### [3.1.1] - 2019-02-17
- Update userspace backend to latest upstream, should bring significant
  speed improvements.
- Fix more theming related issues.


### [3.1.0] - 2019-02-16
- Rewrite theming options - Replace light/dark/black options
  with a choice between light and black.
- Redesign settings screen with categories
- Resolve issues with installation of Magisk module on rooted
  mode.
- Code improvements and dependency updates.


### [3.0.0] - 2019-01-30
- Initial release with Viscerion branding
- Allow switching between whitelist and blacklist for userspace backend (more below)
- Smaller install size
- Ensure notification reacts to tunnel changes from command line tools
- Disable sound and notification for wg-quick notification
- Fix some misleading error messages
- Ensure keyboard shows up for tunnel name when importing QR codes
- Faster layout load times
- Code cleanup across the board

When the whitelist option is enabled, all apps that are not in the exclusions
list are exempt from going through the tunnel, and the ones in the list are
the only ones which use the tunnel for networking.


### [2.0.0] - 2018-12-30
- Rewrite entire codebase based on upstream remodel
- Future-proof Magisk version detection
- Fix restorecon issues with Magisk
- Ensure command line tools know the correct paths to probe for config files
- Update userspace implementation to work with Android 9's bionic restrictions

[Unreleased]: https://github.com/msfjarvis/viscerion/compare/5.2.11...HEAD
[5.2.11]: https://github.com/msfjarvis/viscerion/releases/5.2.11
[5.2.10]: https://github.com/msfjarvis/viscerion/releases/5.2.10
[5.2.9]: https://github.com/msfjarvis/viscerion/releases/5.2.9
[5.2.8]: https://github.com/msfjarvis/viscerion/releases/5.2.8
[5.2.7]: https://github.com/msfjarvis/viscerion/releases/5.2.7
[5.2.6]: https://github.com/msfjarvis/viscerion/releases/5.2.6
[5.2.5]: https://github.com/msfjarvis/viscerion/releases/5.2.5
[5.2.4]: https://github.com/msfjarvis/viscerion/releases/5.2.4
[5.2.3]: https://github.com/msfjarvis/viscerion/releases/5.2.3
[5.2.2]: https://github.com/msfjarvis/viscerion/releases/5.2.2
[5.2.1]: https://github.com/msfjarvis/viscerion/releases/5.2.1
[5.2.0]: https://github.com/msfjarvis/viscerion/releases/5.2.0
[5.1.1]: https://github.com/msfjarvis/viscerion/releases/5.1.1
[5.1.0]: https://github.com/msfjarvis/viscerion/releases/5.1.0
[5.0.0]: https://github.com/msfjarvis/viscerion/releases/5.0.0
[4.0.0]: https://github.com/msfjarvis/viscerion/releases/4.0.0
[3.1.1]: https://github.com/msfjarvis/viscerion/releases/3.1.1
[3.1.0]: https://github.com/msfjarvis/viscerion/releases/3.1.0
[3.0.0]: https://github.com/msfjarvis/viscerion/releases/3.0.0
[2.0.0]: https://github.com/msfjarvis/viscerion/releases/2.0.0
