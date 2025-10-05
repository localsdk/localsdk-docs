# LocalSDK Android Integration Guide

This repository contains the official integration documentation for LocalSDK Android Core, hosted on GitHub Pages.

## 🌐 Live Site

Visit the integration guide at: `https://localsdk.github.io/localsdk-docs/`

## 📚 Contents

- **Integration Guide** (`index.html`) - Complete step-by-step integration instructions for LocalSDK Android

## 🚀 LocalSDK Features

LocalSDK is an enterprise-grade location tracking SDK for Android with:

- ✅ High accuracy location tracking with multiple providers
- ✅ Battery-optimized background tracking
- ✅ Real-time AWS IoT integration
- ✅ Comprehensive permission handling
- ✅ Foreground service support
- ✅ Battery optimization bypass utilities

## 📦 Installation

Add to your `build.gradle.kts`:

```kotlin
dependencies {
    implementation("com.localsdk:core:0.0.1-alpha")
}
```

## 🔧 Quick Start

**Note:** You need an SDK key to use LocalSDK. Contact your LocalSDK representative to obtain one.

```kotlin
// Initialize SDK with key
LocalSDK.initialize(context, "YOUR_SDK_KEY_HERE")

val config = Config.Builder()
    .setTrackingMode(TrackingMode.STANDARD)
    .setForegroundServiceEnabled(true)
    .build()

LocalSDK.setConfig(config)

LocalSDK.onLocation { location ->
    // Handle location updates
}

LocalSDK.startTracking()
```

## 🔧 Development

This is a static HTML site using Bootstrap 5 for styling. To modify:

1. Edit `index.html` directly
2. Test locally by opening `index.html` in a browser
3. Push changes to deploy via GitHub Pages

## 📄 License

© 2025 LocalSDK. All rights reserved.

## 🔗 Links

- [Main SDK Repository](https://github.com/localsdk/localsdk-android-core)
- [GitHub Organization](https://github.com/localsdk)
- [Maven Central](https://central.sonatype.com/artifact/com.localsdk/core)