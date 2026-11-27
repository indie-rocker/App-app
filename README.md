# Presence — Daily Check-in (iPhone-ready web app)

## Included
- One prompt per screen, clean white, phone-friendly interface
- **Core ratings:** presence, dissociation/detachment, memory/recall, focus, mental clarity, stress, emotional state
- **Context:** sleep, caffeine, environment, social interaction quality, connection, meaningful conversations, relationship tone, other influences
- **Behaviors:** hygiene/personal maintenance, physical activity, time outside, water intake, food intake, meal regularity, nutrition quality, whether you ate enough, general self-care
- Daily entries saved locally on this device, with history, edit/delete, trend summaries, CSV export, and JSON backup/restore
- Installable PWA with offline cache

## Update an existing GitHub Pages repository
1. Download/extract this folder.
2. In your `presence-checkin` GitHub repository, open the existing app files.
3. Upload and replace the six files in the repository root: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`, and `README.md`.
4. Commit the changes to the `main` branch. GitHub Pages will redeploy automatically.
5. On your iPhone, open the site in Safari and refresh. If the old version remains, fully close and reopen the Home Screen app; the service-worker cache version has been updated.

## Existing entries and data safety
This version deliberately keeps the original local-storage key, `presence_checkins_v1`, and preserves existing field names. Your old entries should remain readable and the new fields will be added as you complete them. The app stores data in the browser on your device; it does not upload your check-ins. **Before updating, export a JSON backup from History** as a precaution.

## 9 PM reminder on iPhone
GitHub Pages is static hosting, so the website cannot independently schedule reliable background push notifications. Keep or create your existing 9:00 PM iPhone Shortcuts automation with a **Show Notification** action as the reminder, then open Presence from your Home Screen to complete the check-in. The reminder is an iOS Shortcut, not a push notification sent by this website.

## Install on iPhone (if needed)
1. Open the GitHub Pages URL in Safari.
2. Tap Share → **Add to Home Screen** → Add.
3. Launch Presence from the Home Screen.

## Privacy note
This is a local-first personal journal, not a diagnostic or emergency tool. Entries remain in this browser's local storage. Clearing website data or deleting the app can erase them, so export JSON backups periodically.
