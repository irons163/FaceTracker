# Face Tracker

This project is a copy and adjustment one from [FaceTracker] (https://github.com/anuragajwani/FaceTracker)

About original author:
```
This repository contains the source code for my blog post: [Live Face Tracking on iOS using Vision Framework](https://medium.com/@anuragajwani/live-face-tracking-on-ios-using-vision-framework-adf8a1799233). Each step from the post is a commit on the master branch.
```

The codes and the introductions are good, however, there are some codes are strange and the author didn't metion that.  Like this part:
```swift
let eyePathPoints = eye.normalizedPoints
            .map({ eyePoint in
                CGPoint(
                    x: eyePoint.y * screenBoundingBox.height + screenBoundingBox.origin.x,
                    y: eyePoint.x * screenBoundingBox.width + screenBoundingBox.origin.y)
            })
```

What is `eyePoint.y * screenBoundingBox.height + screenBoundingBox.origin.x`?

Looks weird, doesn't it?

So, I adjusted some parts of the codes to make it more understandable.




