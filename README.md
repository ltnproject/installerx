# IPA Installer X

A modern web-based **iOS OTA (Over-The-Air) installer generator** that creates a direct install link for `.ipa` applications using the `itms-services://` protocol.

Users can paste an IPA download URL, enter basic app information, and instantly generate a **direct install link** that opens the iOS installation prompt.

---

## Features

- Clean modern UI
- Generates OTA install manifests
- Supports automatic install prompt
- Copy-to-clipboard install link
- Input validation for HTTPS IPA URLs
- Mobile-friendly design
- Works directly on iPhone and iPad browsers

---

## How It Works

1. User enters the **IPA download URL**
2. App metadata is filled:
   - App Name
   - Version
   - Bundle Identifier
3. The page generates a **manifest.plist**
4. The installer creates an `itms-services://` install link
5. When opened on iOS, the system prompts the user to **install the app**

---

## Requirements

For OTA installation to work correctly:

- The `.ipa` file must be **hosted over HTTPS**
- The IPA must be **signed with a valid Apple certificate**
- The device must **trust the developer certificate**
- Installation must be opened from **Safari on iOS**

---

## Installation

Simply host the HTML file on any web server.

Then open the page in a browser and generate install links.

---

## Usage

1. Open the installer page
2. Paste the direct download link to the `.ipa`
3. Enter:
   - App Name
   - Version
   - Bundle ID
4. Click **Generate Install Link**
5. Tap the generated link on an iOS device

The device will show the **Install App prompt**.

---

## Trusting the Developer

If the app does not open after installing:
Settings → General → VPN & Device Management

Find the developer certificate and tap **Trust**.

---

## Security Notice

Only install IPA files from trusted sources.  
Unsigned or revoked certificates will prevent installation.

---

## License

MIT License
