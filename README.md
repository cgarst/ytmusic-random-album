# 🎲 Random Album for YouTube Music™
Can't decide which record to spin today? This browser extension plays a random album from your YouTube Music™ library.

## Chromium-based Browser Installation
 1. Browse to chrome://extensions
 2. Enable extension developer mode in the browser, if necessary, to allow loading unpacked extensions
 3. Select the "Load unpacked" extension option and navigate to the `src/chromium/` directory

## Firefox-based Browser Installation
The release version of Firefox does not allow users to permanently install unsigned extensions. This leaves two options.

Temporary installation in the Firefox release version:
 1. Run `cd bin/ && ./make_firefox_xpi.sh` to build the XPI extension file
 2. Browse to `about:debugging` and "This Firefox"
 3. Select "Load Temporary Add-On", "Install Add-on From File", and select `bin/random-album-for-youtube-music.xpi`

 Permanent installation in Firefox Developer Edition:
 1. Browse to `about:config` and set `xpinstall.signatures.required` to "false"
 2. Browse to `about:addons`, click the gear icon, and select "Install Add-on from File"
 3. Select `bin/random-album-for-youtube-music.xpi`

## Usage
While in YouTube Music, click the extension icon. This will navigate to your album library, open a random album, and play it.

## Troubleshooting
The album will not automatically play if the site is denied autoplay by the browser. A message may be logged to console like "Autoplay is only allowed when approved by the user, the site is activated by the user, or media is muted." This can be resolved by giving the site autoplay permission in the permissions icon near the address bar.

## Credits
Icon by [Icons8](https://icons8.com/)
