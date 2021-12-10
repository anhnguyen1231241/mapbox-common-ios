# mapbox-common-ios

### Prerequisites

Before you can download the Mapbox Common SDK, you need to create a token with `DOWNLOAD:READ` scope.
Go to https://account.mapbox.com and click "Create token"

##### SPM, CocoaPods and Carthage
Insert or append the following to `~/.netrc`

```bash
machine api.mapbox.com
  login mapbox
  password <TOKEN WITH DOWNLOAD:READ SCOPE>
```

## Integration

##### Swift Package Manager

###### Using Xcode

<details><summary>Detailed Flow</summary>
<img src=".img/spmx-1.png">
<img src=".img/spmx-2.png">
<img src=".img/spmx-3.png">
<img src=".img/spmx-4.png">
</details>

###### Using SPM Package 📱🖥💻

```swift
.package(url: "https://github.com/mapbox/mapbox-common-ios.git", from: "20.1.2"),
```

##### CocoaPods 📱🖥💻

```ruby
pod 'MapboxCommon', '20.1.2'
```

##### Carthage 📱

Add the following code to your Cartfile.

```bash
binary "https://api.mapbox.com/downloads/v2/carthage/mapbox-common/MapboxCommon-ios.json" == 20.1.2
```

Then run the following command in the Terminal.
```bash
carthage update --platform ios --use-netrc
```
