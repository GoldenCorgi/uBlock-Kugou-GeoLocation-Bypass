<h1 align="center">
  Kugou Music Global
</h1>

<div align="center">
  <b>
    Additional filters for
    <a href="https://adguard.com/">
      AdGuard
    </a>
    and
    <a href="https://github.com/gorhill/uBlock">
      uBlock Origin
    </a>
  </b>
  <br>
  <br>
  <a href="#description">
    Description
  </a>
  •
  <a href="#getting-started">
    Getting Started
  </a>
  •
  <a href="#available-filter-lists">
    Available Filter Lists
  </a>
  •
  <a href="#special-thanks">
    Special Thanks
  </a>
  •
  <a href="#license">
    License
  </a>
  <br>
  <br>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">
    <img src="https://img.shields.io/badge/Language-JavaScript-F7DF1E?style=for-the-badge&logo=javascript">
  </a>
  <a href="https://github.com/GoldenCorgi/uBlock-Kugou-GeoLocation-Bypass/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-181717?style=for-the-badge&logo=github">
  </a>
  <a href="https://kb.adguard.com/en/general/how-to-create-your-own-ad-filters">
    <img src="https://img.shields.io/badge/Syntax-AdGuard-68BC71?style=for-the-badge&logo=adguard">
  </a>
  <a href="https://github.com/gorhill/uBlock/wiki/Static-filter-syntax">
    <img src="https://img.shields.io/badge/Syntax-uBlock%20Origin-800000?style=for-the-badge&logo=ublock-origin">
  </a>
</div>

## Description
This repository contains filter lists that can be added to content blockers, such as [AdGuard][AdGuard Website Link] and [uBlock Origin][uBlock Origin GitHub Link]. 

#### Have this ever happen to you?


damn i really want to listen to Super Idol 的笑容 for hours on repeat 
by the original singer and support him on china's version of spotify 
called Kugou music, but this dummy thicc geolocation restriction is stopping me


yes, i did all this to hear the full 3 minutes of Super Idol 的笑容 cover by tian yi ming on kugou music





## Getting Started
### Installation
#### AdGuard on Safari (Mobile - iOS 15 or Above)
1. Download and install AdGuard from the App Store (Make sure to pay for a subscription or purchase the Pro version)
    - [AdGuard][AdGuard App Store Link] - Free With Optional Paid Subscription
    - [AdGuard Pro][AdGuard Pro App Store Link] - One-Time Purchase
2. Open the AdGuard application and go to the Protection section
    <br>
    2a. Turn on "Safari Protection" by tapping the toggle button
    <br>
    2b. Turn on "Advanced Protection" by tapping the toggle button
3. Close the AdGuard application and open the Settings application
4. Click on the following options in the Settings application: `Safari > Extensions`
    <br>
    4a. "Allow These Content Blockers" Section: Turn on all the AdGuard options to allow "Safari Protection" to work in Safari ([Guide][Content Blockers Guide])
    <br>
    4b. "Allow These Extensions" Section: Turn on AdGuard and click on the "Allow" option in the permission area to allow "Advanced Protection" to work in Safari ([Guide][Safari Web Extensions Guide])
5. Close the Settings application and open the AdGuard application
6. Click on the following options in the AdGuard application: `Protection > Safari protection > Filters > Custom`
    <br>
    6a. Turn on the use of "Custom" filters by tapping the toggle button
    <br>
    6b. Add a filter list from this repository to AdGuard by clicking on the "Add a filter" button, pasting the raw GitHub link from this repository into the "Filter URL" field, clicking on the "Next" button, and clicking on the "Add" button after reviewing the prompt to confirm that it is the correct filter list
#### uBlock Origin on Google Chrome (Desktop)
1. Add the uBlock Origin extension by downloading it from the [Chrome Web Store][uBlock Origin Chrome Web Store Link] or [GitHub][uBlock Origin GitHub Link]
2. After adding the extension, follow this [guide][uBlock Origin Filter Guide] to manually import a filter list from this repository to uBlock Origin or left-click on any of the **"Subscribe"** buttons below to automatically add a filter list to uBlock Origin
### Usage
No further actions are necessary. After adding a filter list from this repository to a content blocker, that filter list will work and remove annoyances without any user input.

## Available Filter Lists
| **Filter Lists** | **Links** | **Information** |
|:-----------------|:----------|:----------------|
| **[Base][Base Filter]** | <br> **Subscribe:** <br> [Click Here][Base Subscription] | **Description:** <br> This filter list allows you to listen to Kugou Music anywhere in the world, pretty cool. Just click subscribe on the left, then head over to any kugou links, [i highly recommend this one](https://www.kugou.com/mixsong/5veozf13.html)



## License
[MIT](https://github.com/uBlock-Kugou-GeoLocation-Bypass/filter-lists/blob/main/LICENSE)

<!-- Application Links -->
[AdGuard App Store Link]: https://apps.apple.com/app/id1047223162
[AdGuard Pro App Store Link]: https://apps.apple.com/app/id1126386264
[AdGuard Website Link]: https://adguard.com/
[uBlock Origin Chrome Web Store Link]: https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm
[uBlock Origin GitHub Link]: https://github.com/gorhill/uBlock

<!-- Filter Lists -->
[Base Filter]: https://github.com/GoldenCorgi/uBlock-Kugou-GeoLocation-Bypass/blob/main/kugou.txt

<!-- Information Links -->
[Safari Web Extensions Guide]: https://adguard.com/en/blog/adguard-4-3-for-ios.html
[uBlock Origin Filter Guide]: https://github.com/gorhill/uBlock/wiki/Filter-lists-from-around-the-web
[uBlock Origin Scriptlet Guide]: https://github.com/gorhill/uBlock/wiki/Advanced-settings#userresourceslocation

<!-- Subscription Lists -->
[Base Subscription]: https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/GoldenCorgi/uBlock-Kugou-GeoLocation-Bypass/main/kugou.txt&title=super%20idol%20moment

# disclaimer
pls dun sue me 


# how did i do this? for my future self

Go into Devtools Sources tab, find the Javascript that includes the phrases used in the geolocation block (or go into Network tab, search for any JSON response which includes that).

Find the javascript file that invokes the phrase, then check the network tab for the request that is initiated by the same javascript file

Deny that request and here we are


This means that Kugou Music actually sent over the mp3 files BEFORE checking for geolocation restrictions

# Translation

- [简体中文](README.zh-CN.md)

