<p align="center">
  <img src="skydog-logo.png" alt="SkyDog AI" width="140">
</p>

<h1 align="center">🏁 SkyDog DragCam</h1>
<p align="center"><b>Powered by SkyDog AI</b> — the camera that knows how fast you're going.</p>

---

## What it does

Point your phone at the road, the trail, the water — hit record. Your live telemetry is **burned right into the video** (and photos), so it's part of the footage forever, on any player, no editing:

- 🚀 **Speed** — big live MPH (or km/h) readout with session max
- ⛰️ **Elevation** — live altitude in feet or meters
- 🧭 **Compass** — scrolling heading tape with degrees & cardinal direction
- 🕐 **Timestamp** — date & time on every frame
- ⏱ **Drag timing** — arm it, launch, and get 0–30, 0–60, 60 ft, 330 ft, 1/8 mile, 1000 ft and **1/4 mile ET with trap speed**, drawn onto your video as they happen
- 📷 **Photos too** — one tap grabs a still with the full HUD baked in
- 💾 **Save & share** — everything lands in the built-in gallery; share straight to Messages/Instagram or save to your camera roll
- 🏁 **Run history** — every quarter-mile pass is logged and shareable as text
- ▶ **Demo mode** — try the whole thing from your couch with a simulated pull
- 📴 **No accounts, no uploads, no tracking.** One file. Your footage stays on your phone.

## Put it on your phone

1. Open the app URL in Safari (iPhone) or Chrome (Android)
2. Tap **Share → Add to Home Screen**
3. It installs with the SkyDog AI logo and runs full-screen like a real app
4. First launch will ask for **camera, microphone & location** — that's the whole trick

## Notes

- GPS speed/timing accuracy depends on your phone's GPS (typically ±1 mph and a tenth or two on ETs). It's for fun and practice, not sanctioned racing.
- Recording format is MP4 on iPhones and WebM on most Androids — both share fine.
- Drag timing: come to a **full stop**, tap ⏱ → **ARM**, then launch whenever. The clock starts the instant you move.

## Tech

Single-file HTML/JS. Live camera frames + telemetry HUD are composited on a canvas at up to 1080p/30fps and encoded on-device with MediaRecorder; GPS via the Geolocation API with speed smoothing and interpolated split timing; compass via device orientation with GPS-course fallback; captures persist in IndexedDB. Verified by an automated browser test suite (simulated GPS runs, capture pipeline, timing math).

---

<p align="center"><img src="icon-192.png" width="48" alt="SkyDog AI"><br><sub>© 2026 SkyDog AI</sub></p>
