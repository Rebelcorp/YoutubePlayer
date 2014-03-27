# Android YouTube Player Module

## Description

Android module that plays videos from YouTube. This module creates an Android activity that allows developers to play videos that are hosted on YouTube. It uses the native Android Youtube SDK to play videos use the player provided by the native Youtube app. If the Youtube app is not installed it falls back to the Android YouTube Player (http://code.google.com/p/android-youtube-player/) library.

## Referencing the module in your Titanium Mobile application ##

Simply add the following lines to your `tiapp.xml` file:

```xml    
    <modules>
        <module platform="iphone">titutorial.youtubeplayer</module> 
        <module platform="android">titutorial.youtubeplayer</module> 
    </modules>
```

## Example

Put the following code in your app.js (or alloy.js if you are using Alloy) to use the module.

```javascript
var youtubePlayer = require("titutorial.youtubeplayer");
youtubePlayer.developerKey = 'abcdefghijklmnopq';

youtubePlayer.playVideo('kh29_SERH0Y');
```

Information on how to obtain a  developer key can be found on: https://developers.google.com/youtube/android/player/register

## Methods

### playVideo(videoId)

Takes video id as input parameter and plays video automatcally. 

### playPlayListVideo(playListId)

Takes playlist id as input parameter then it will play the latest video added to a YouTube playlist


## Author

Timan Rebel
based on the work of Karthi Ponnusamy - karthi.nkl@gmail.com

## License

Copyright (c) 2013 Karthi Ponnusamy

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
