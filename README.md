# Cordova / Meteor icons and splash screens generator (including 9 patch png for Android splash screens)
# with ImageMagick native dependancy

## Prerequisites

This project requires `imagemagick`.

### Linux

```
sudo apt-get install imagemagick imagemagick-doc
```

### macOS

Install [homebrew](http://brew.sh/) and then:

```
brew install imagemagick
```

### Windows

http://www.imagemagick.org/script/binary-releases.php#windows

## Install

```
npm install -g assets9-im
```

## Usage

1. Create an icon at 1024x1024 and name it `icon.png`.

2. Create a splash screen at 2208x2208 and name it `splash.png`. Place your logo / brand in a 1200x1200 square centered in that splash screen.

3. Run `assets9-im` where these two files are.

4. (Meteor) Add the console output to your `mobile-config.js`

Sizes thanks to https://github.com/meteor/meteor/blob/release-1.4/tools/cordova/builder.js

## Notes

- For Meteor >= 1.3 and Cordova
- This will crop splash screen horizontally centered and vertically centered.
- This generates [9 patch](https://developer.android.com/guide/topics/graphics/2d-graphics.html#nine-patch) splash screens for Android.

## Credits

- Thanks to [Ipender](https://github.com/lpender/meteor-assets) for the inspiration
- Thanks to [aheckmann](https://github.com/aheckmann/gm) for the image manipulation library (ImageMagick) wrapper

## License

MIT