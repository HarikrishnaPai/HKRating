# HKRating for iOS

A custom rating view for SwiftUI

A view of inline images that represents a rating.
Tapping on an image will change it from an unfilled to a filled version of the image. 
HKRating has a set of predefined images and also supports custom images for rating.

## Usage
The following example shows a HKRating view with a maximum rating of 5 red hearts, each with a width of 40, and an initial rating of 2:

```swift
struct ContentView: View {

    @State var currentRating = 2

    var body: some View {
        VStack {
            Text("My Rating")
            HKRating(maxRating: 5,
                     currentRating: $currentRating,
                     width: 40,
                     color: .red,
                     ratingImage: .heart)
        }
        .padding()
    }
}
```

Output:

<img width="396" alt="HKRating" src="https://github.com/user-attachments/assets/1d2d6e64-71dc-4e88-9d0c-971a6d91e748">


## Installing HKRating
HKRating supports installation via [Swift Package Manager](https://www.swift.org/package-manager/).

### Swift Package Manager

To install HKRating using [Swift Package Manager](https://github.com/swiftlang/swift-package-manager) you can follow the [tutorial published by Apple](https://developer.apple.com/documentation/xcode/adding_package_dependencies_to_your_app) using the URL for the HKRating repo with the current version:

1. In Xcode, select “File” → “Add Packages...”
1. Enter https://github.com/HarikrishnaPai/HKRating

or you can add the following dependency to your `Package.swift`:

```swift
.package(url: "https://github.com/HarikrishnaPai/HKRating", from: "1.0.0")
```

## Swift Version Support

HKRating uses Swift 5 and Xcode version 15.4
