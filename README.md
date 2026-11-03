# AvatarKit CocoaPods Specs

CocoaPods spec repository for the AvatarKit iOS SDKs:

| Pod | Module | Description |
|-----|--------|-------------|
| `SpatiusAvatarKit` | `AvatarKit` | AvatarKit — real-time, audio-driven avatar rendering SDK for iOS |
| `AvatarKitRTC` | `AvatarKitRTC` | RTC adapter for AvatarKit |
| `AvatarKitAgoraBridge` | `AvatarKitAgoraBridge` | ObjC++ bridge exposing Agora's encoded-frame observer to Swift |

The public CocoaPods trunk stops accepting new versions on December 2, 2026, so new
versions of these pods are published here. Earlier versions are mirrored here too.

## Usage

Add this repository as a source at the top of your `Podfile`, and keep the CocoaPods CDN
for third-party dependencies such as `AgoraRtcEngine_iOS` and `SwiftProtobuf`:

```ruby
source 'https://github.com/spatius-ai/avatarkit-specs.git'
source 'https://cdn.cocoapods.org/'

platform :ios, '16.0'

target 'YourApp' do
  use_frameworks!
  pod 'SpatiusAvatarKit', '1.3.7'
end
```

Then run `pod install --repo-update`.

Swift Package Manager users do not need this repository; see
https://github.com/spatius-ai/avatarkit-ios-release.

Documentation: https://docs.spatius.ai
