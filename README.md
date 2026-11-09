# AutoEditor (Windows v2)

Sync timestamp-named images and video clips to a voiceover narration and export an MP4, completely offline on your computer.

---

## ⚡ What it Does
* **Automatic Voiceover Sync:** Name images or video clips with the second they should appear (e.g., `0-03.png` or `0-03.mp4` cuts in at 0:03).
* **Local Rendering:** Video processing runs directly on your machine using FFmpeg with hardware acceleration (NVIDIA NVENC, Intel QSV, AMD AMF) or CPU fallback. No files are uploaded to any external server.
* **Audio & Video Editing:** Supports trimming, zooming, mixing clip audio under narration, and adding customized captions.

---

## 🚀 How to Run
1. Open the **`AutoEditor`** directory.
2. Double-click **`AutoEditor.exe`**.
3. A console window will launch, detecting your hardware encoder and starting the server at:
   ```
   http://localhost:4000
   ```
4. Your default browser will open automatically. Keep the console window open while working.
5. Finished renders are saved directly to:
   ```
   C:\Users\<YourUsername>\Downloads\AutoEditor
   ```

---

## 📁 Repository Structure
```
AutoEditor/
  ├── AutoEditor.exe      # Main application engine (Node.js runtime bundled)
  ├── ffmpeg.exe          # FFmpeg video encoder binary with GPU acceleration
  ├── caption.ttf         # Font file used for video subtitles and captions
  ├── READ ME FIRST.txt   # Original usage instructions
  └── out/                # Web frontend assets (HTML, JS chunks, CSS, icons)
```

---

## 💻 Requirements
* Windows 10 / Windows 11 (64-bit)
* No additional dependencies required (FFmpeg and app engine are pre-bundled).
