# LaunchDeck

LaunchDeck is a lightweight, fullscreen application launcher for macOS that turns a computer into a simple, mode-based appliance.

It provides a clean, controller-friendly home screen for launching selected apps—such as media players, emulators, or tools—without exposing the desktop. LaunchDeck is designed to run at startup, stay idle in the background, and return automatically when a launched app exits.

LaunchDeck is ideal for couch setups, projectors, kiosks, dedicated media systems, and any environment where reliability and simplicity matter more than traditional desktop workflows.

---

## Features

- Fullscreen, distraction-free launcher UI
- Launches user-defined applications (by bundle ID)
- Automatically returns to the menu when an app exits
- Supports mouse, keyboard, and gamepad input
- Minimal CPU and memory usage when idle
- Runs at login for appliance-style setups
- macOS-native (Swift + SwiftUI)

---

## Typical Use Cases

- Home theater or projector setups
- Retro gaming systems (RetroArch, emulators)
- Media appliances (Plex, HDHomeRun, Kodi)
- Museum or exhibit kiosks
- Classroom or presentation stations
- Single-purpose or shared Macs

LaunchDeck does not attempt to replace the launched applications—it simply provides a stable, predictable way to select and switch between them.

---

## How It Works

1. LaunchDeck starts automatically and displays a fullscreen menu.
2. The user selects an app using a mouse, keyboard, or gamepad.
3. LaunchDeck launches the selected app and hides itself.
4. When the app exits (or when a defined “home” action is triggered), LaunchDeck returns to the foreground.

The launcher itself remains idle while another app is running and does not interfere with input, audio, or graphics.

---

## Input Support

LaunchDeck supports:
- Mouse and trackpad
- Keyboard navigation
- Game controllers via macOS GameController framework

Controllers can be used to:
- Navigate the menu
- Launch applications
- Return to the launcher (optional binding)

Applications such as RetroArch handle gamepad input directly once launched.

---

## Installation (Development)

LaunchDeck is currently built as a native macOS application.

### Requirements
- macOS Monterey (12.x) or newer
- Xcode
- Swift / SwiftUI

### Build Steps
1. Clone the repository
2. Open `LaunchDeck.xcodeproj` in Xcode
3. Build and run the app
4. Configure login/startup behavior as desired

Prebuilt binaries may be provided in the future.

---

## Configuration

Applications are defined internally by:
- Display name
- Bundle identifier
- Optional icon

Future versions may expose configuration via a file or UI, but the current design prioritizes simplicity and stability.

---

## License

LaunchDeck is licensed under the **Polyform Noncommercial License 1.0.0**.

You may use, modify, and distribute this software for **personal and non-commercial purposes only**.

**Commercial use**—including use by businesses, venues, kiosks, paid installations, or revenue-generating environments—**requires a separate commercial license**.

See the `LICENSE` file for full terms.

---

## Commercial Licensing

If you wish to use LaunchDeck in a commercial environment, please contact the author to discuss licensing options.

---

## Project Status

LaunchDeck is under active development and currently focused on:
- Stability
- Minimal resource usage
- Appliance-style workflows

The project intentionally avoids unnecessary features that would compromise reliability.

---

## Philosophy

LaunchDeck is designed around the idea that some computers should behave like appliances, not desktops.

It provides a predictable entry point, clear modes of operation, and a simple way to switch tasks—without locking users into a specific ecosystem or workflow.

---

## Contributing

Contributions, bug reports, and suggestions are welcome for non-commercial use cases.

Please note that any contributions must be compatible with the project’s licensing model.

---

## Disclaimer

LaunchDeck is provided “as is,” without warranty of any kind. Use at your own risk.
