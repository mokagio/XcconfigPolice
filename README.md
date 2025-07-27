The Xcode GUI is _not_ a good place to manage build settings.

A better approach is to move all build settings to `xcconfig` files, making the setup easier to diff, modify, and understand.

---

## Usage

- Install [`swift-sh`] (`brew install swift-sh`)
- Checkout this repo
- Run `./police <path/to/xcodeproj>` to validate

At this time, this is just a proof of concept but the intention is to make it into a tool you can run as a build phase.

## Credits

- The heavy lifting of parsing the Xcode project file is done by [XcodeProj]https://github.com/tuist/XcodeProj).
- [Gio Lodi](https://giolodi.com) ([@mokagio](https://github.com/mokagio))
