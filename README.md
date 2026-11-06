# Very CocoaPods Specs

CocoaPods spec repository for Very's iOS SDKs. CocoaPods trunk stopped
accepting new podspecs on 2026-12-02, so new versions are published here.

## Usage

Add a `:source` to the pod line in your `Podfile`:

```ruby
pod 'VeryAILiveness', '~> 1.1', :source => 'https://github.com/veroslabs/very-cocoapods-specs.git'
```

The `:source` applies to that pod only; your other pods keep resolving from
their usual sources. Then run `pod install` (or `pod install --repo-update`
after a new release).

## Pods

| Pod | Versions |
|---|---|
| `VeryAILiveness` | 1.0.40 and later |

Binaries are not stored here: each podspec points at a tag of the SDK's
release repository (for `VeryAILiveness`,
[veroslabs/very-ai-liveness-ios](https://github.com/veroslabs/very-ai-liveness-ios)).
Swift Package Manager users depend on that repository directly.

Specs are added by the SDK release pipelines. Do not edit or remove a
published version.
