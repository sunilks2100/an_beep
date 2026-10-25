Double Beep Timer PWA

Files:
- index.html: app interface
- double-beep-loop.wav: 60-second audio loop with two short beeps at the start
- manifest.webmanifest: installable web app metadata
- sw.js: offline caching service worker

Install on Android:
1. Upload the contents of this folder to an HTTPS static host (for example, GitHub Pages or Netlify).
2. Open the hosted URL in Chrome on your Android phone.
3. Use Chrome's menu and choose "Install app" or "Add to Home screen".
4. Open the installed app and tap "Start beeping".
5. Lock the phone to test. Use the app's Stop button before closing it.

Important limitation:
The app uses continuous looping media rather than a JavaScript timer, which is more likely to continue while the screen is locked. However, a PWA cannot guarantee background playback on every Android device. Battery optimization, force-stopping Chrome, or OS/browser policies may stop it. For guaranteed alarm-like behavior, a native Android app using an appropriate foreground service/alarm mechanism is more reliable.
