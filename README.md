<p align="center">
  <a href="https://www.cloudflare.com/">
    <img src="https://cf-assets.www.cloudflare.com/slt3lc6tev37/6EYsdkdfBcHtgPmgp3YtkD/0b203affd2053988264b9253b13de6b3/logo-thumbnail.png" alt="Cloudflare" width="200" />
  </a>
  <h2 align="center">RealtimeKit Core SDK for iOS</h2>
</p>

Swift Package Manager distribution package for the **RealtimeKit Core** iOS SDK. This package provides low-level APIs for building live video and audio experiences on iOS.

## Installation

### Xcode

1. In Xcode, go to **File > Add Package Dependencies...**
2. Enter the repository URL:
   ```
   https://github.com/cloudflare/realtimekit-ios-core.git
   ```
3. Select the version rule you prefer (e.g., **Up to Next Major Version**) and add the package.

### Package.swift

Add the dependency to your `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/cloudflare/realtimekit-ios-core.git", from: "<version>")
]
```

Then add the products you need to your target:

```swift
.target(
    name: "YourApp",
    dependencies: [
        .product(name: "RealtimeKit", package: "realtimekit-ios-core"),
        .product(name: "RTKWebRTC", package: "realtimekit-ios-core"),
    ]
)
```

## Products

| Product | Description |
|---------|-------------|
| `RealtimeKit` | Core SDK — includes the RealtimeKit binary XCFramework and RTKWebRTC |
| `RTKWebRTC` | WebRTC binary XCFramework (standalone) |

## Requirements

- iOS 13+
- Swift 5.5+

## Documentation

Full documentation is available at **[developers.cloudflare.com/realtime/realtimekit/core](https://developers.cloudflare.com/realtime/realtimekit/core/)**.
