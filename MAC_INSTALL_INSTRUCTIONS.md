# macOS Installation Instructions

Due to Apple's security requirements, you may see a "damaged app" error when installing Everything Black Browser. This is because the app isn't notarized with an Apple Developer certificate. The app is safe to use.

## Installation Steps

### Method 1: Right-Click to Open (Recommended)
1. Download the DMG file
2. Open the DMG and drag Everything Black to Applications
3. **Important**: Don't double-click to open the app yet
4. Go to Applications folder
5. **Right-click** (or Control-click) on Everything Black
6. Select "Open" from the menu
7. Click "Open" in the dialog that appears
8. The app will now open and be saved as an exception

### Method 2: Terminal Command
If Method 1 doesn't work:
1. Open Terminal (Applications > Utilities > Terminal)
2. Run this command:
   ```
   xattr -cr "/Applications/Everything Black.app"
   ```
3. Now you can open the app normally

### Method 3: Security Settings
1. Try to open the app (it will show an error)
2. Go to System Settings > Privacy & Security
3. Look for a message about Everything Black being blocked
4. Click "Open Anyway"

## Why This Happens

macOS requires apps to be notarized by Apple, which requires:
- An Apple Developer account ($99/year)
- Code signing certificates
- Apple's approval process

As an independent open-source project, Everything Black Browser is not notarized, but it's completely safe to use.

## Future Releases

We're working on getting proper code signing certificates for future releases to eliminate this issue.