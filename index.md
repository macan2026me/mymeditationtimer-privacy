# My Meditation Timer

A simple meditation timer for iPhone (iOS 17.6 and later), written in SwiftUI.

## Features

- Timer with ready presets (1, 3, 5, 10, 15, 20, 60 minutes) or open-ended count-up
- Breathing guide with adjustable speed and optional voice guidance
- End sounds: wood block, singing bowl, birds, or vibration
- Background sounds: ocean, forest and birds, brown noise (started by hand each time)
- Paste in your own Spotify or Apple Music playlist link
- Daily streak (Swedish time, a new day starts 00:01) and a star counting all days you have meditated
- Four colour themes with a birch-bark background
- Free version plus a one-time in-app purchase for the full version

## Build

Open `MY MEDITAITON TIMER.xcodeproj` in Xcode 26 and run on a simulator or device.
The folder name contains the spelling `MEDITAITON`; that is intentional and must not be "fixed".

Run the unit tests with Cmd+U, or from a terminal:

```bash
xcodebuild test -project "MY MEDITAITON TIMER.xcodeproj" -scheme "MY MEDITAITON TIMER" \
  -destination "platform=iOS Simulator,name=iPhone 17" -only-testing:"MY MEDITAITON TIMERTests"
```

To try the full version without buying, launch from Xcode with the argument `-forcePremium YES` (debug builds only).
A local StoreKit test product is in `MY MEDITAITON TIMER.storekit`.

## In-app purchase

Product ID: `com.marcus.mymeditationtimer.premium` (non-consumable, USD 2.99). It must exist with exactly this ID in App Store Connect.

## Privacy

See [PRIVACY.md](PRIVACY.md). The app has no network code, no accounts and no analytics.

## Sound licences

See `background_SOURCE.txt` and `nature_loop_SOURCE.txt`.
