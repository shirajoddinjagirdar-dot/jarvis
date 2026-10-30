JARVIS Android project starter

This project wraps the supplied JARVIS HTML interface in a Capacitor Android app.
The HTML file is in www/index.html.

LOW-RAM BUILD METHOD (recommended for a 4 GB Windows PC):
Use GitHub Actions to build the APK in the cloud, rather than running Android Studio locally.

1. Create/sign in to a GitHub account.
2. Create a NEW private repository.
3. Upload the contents of this ZIP (not the ZIP itself) to the repository.
4. Open the repository's Actions tab.
5. Select "Build JARVIS Android APK" and click "Run workflow".
6. When it finishes, open the completed workflow run and download the
   "JARVIS-debug-APK" artifact. Extract it to get app-debug.apk.
7. Transfer app-debug.apk to your Android phone and install it. You may need
   to allow installation from that file manager/browser.

Important limitations:
- This first APK is a WebView wrapper for the current HTML interface.
- It does NOT yet implement native Android calling, WhatsApp sending,
  reliable always-on wake-word listening, or a connected AI brain.
- The current HTML uses browser SpeechRecognition and speechSynthesis;
  support varies by Android WebView/device. Microphone permission may be needed.
- Do not expect "Hey Jarvis" background listening to work reliably yet.
- Calls/messages and background services require additional native Android
  integration and explicit permissions/confirmation.
