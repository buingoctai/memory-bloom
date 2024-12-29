# FunLifeCare Mobile App

## Structure 

## Prerequisites

1. Node.js (>=18)
2. pnpm (>=9.0.0)
3. Expo Go app on your mobile device
   - [iOS App Store](https://apps.apple.com/app/apple-store/id982107779)
   - [Android Play Store](https://play.google.com/store/apps/details?id=host.exp.exponent)
4. For iOS development:
   - Mac computer
   - Xcode (latest version)
   - iOS Simulator
5. For Android development:
   - Android Studio
   - Android Emulator

## Getting Started

1. Install dependencies: 

This will start the Expo development server and show a QR code in your terminal.

```bash
pnpm install
```

2. Run the app:

```bash
cd apps/mobile
pnpm start
```

## Development Options

- **Physical Device**: 
  - Install Expo Go app on your phone
  - Scan the QR code with:
    - iOS: Use the Camera app
    - Android: Use the Expo Go app
  - Make sure your phone and computer are on the same network

- **iOS Simulator**:
  - Press `i` in the terminal to open iOS simulator
  - Or run `pnpm ios`

- **Android Emulator**:
  - Press `a` in the terminal to open Android emulator
  - Or run `pnpm android`

## Troubleshooting

1. If QR code doesn't work:
   - Ensure your phone and computer are on the same network
   - Try using a tunnel connection: `pnpm start --tunnel`

2. For "Unable to find expo" errors:
   ```bash
   pnpm install -g expo-cli
   ```

3. For Metro bundler issues:
   ```bash
   # Clear Metro bundler cache
   pnpm start --clear
   ``` 


The development server provides a menu in the terminal with these options, and you can use the keyboard shortcuts to launch your preferred environment.
Remember that:
- For iOS development, you need a Mac with Xcode installed
- For Android development, you need Android Studio with an emulator set up
- For physical device testing, your phone needs to be on the same network as your computer
