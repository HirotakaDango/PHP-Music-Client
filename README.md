# PHPMusic Player

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/50bc78b1-09e3-4c5e-9429-5e7df281d336" />

A lightweight, modern, client-side web application interface for streaming music from a custom PHP backend API.

## Features

- **Modern UI & Responsive Design:** Built using Material Design 3 guidelines with light/dark adaptive layout and full responsiveness across mobile and desktop viewports.
- **Audio Controls & Playback:** Real-time seeking, visualizer, volume control, mute, shuffle, and repeat modes.
- **Search & Filtering:** Dynamic client-side track searching by title, artist, or album.
- **Mobile & Desktop Modes:** Fullscreen audio modal with floating mini-player on mobile devices, alongside a dedicated desktop media panel.
- **Media Session Integration:** Native media key support (`Space`, `ArrowLeft`, `ArrowRight`, `M`) and OS lock screen/notification bar media metadata controls.
- **Demo Mode:** Built-in offline demo mode for quick testing without requiring an active backend connection.

## Requirements

- **Client:** Any modern browser supporting HTML5 Audio, ES6+, and CSS CSS Variables / Grid / Flexbox.
- **Backend API:** A PHP server exposing endpoints for track listing (`action=get_songs`), audio streaming (`action=get_stream`), and image retrieval (`action=get_image` or `action=thumb`).
  - **CORS Notice:** Ensure your PHP backend headers permit Cross-Origin Request Sharing:
    ```php
    header('Access-Control-Allow-Origin: *');
    ```

## Quick Start

1. Open `index.html` in your web browser.
2. Click the **Settings** icon (tune icon in the top right header).
3. Provide your backend details:
   - **API Endpoint URL:** e.g., `https://example.com/index.php`
   - **API Key:** Secret API token
   - **Source Type & Feed ID:** Choose between *All Tracks*, *Playlist*, or *Artist* filtering.
4. Click **Save & Connect** or select **Try Demo Tracks** to test immediately.
