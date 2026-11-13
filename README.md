# My Video Suite

A comprehensive collection of video editing, clipping, and sharing tools brought together into a single repository (`https://github.com/heyaniket065/my-video-suite`).

## Included Modules

| Folder | Tool | Tech Stack | Purpose |
| :--- | :--- | :--- | :--- |
| `supoclip-main/` | **SupoClip** | Next.js (`3107`), FastAPI (`8000`), PostgreSQL, Redis, Whisper | Fast long-video to short-clip generation with AI captions |
| `openshorts-main/` | **OpenShorts** | Vite + React (`5175`), FastAPI (`8000`), Remotion (`3100`), YOLO, MediaPipe | 9:16 vertical Shorts/Reels with active speaker tracking & burned subtitles |
| `openreel-video-main/` | **OpenReel Video** | Turborepo, React/Vite, Electron, Cloudflare Workers | Open-source browser and desktop timeline video editing suite |
| `autoclip_mvp-main/` | **AutoClip MVP** | Vite + React (Ant Design), FastAPI (`8000`), FFmpeg, `yt-dlp` | Automated video/subtitle downloading and AI clip & collection recommendations |
| `PHPVibe-Video-Sharing-CMS-master/` | **PHPVibe CMS** | PHP, MySQL | Complete legacy video, image, and music sharing CMS platform |

## Getting Started

1. Clone this repository:
```bash
git clone [https://github.com/heyaniket065/my-video-suite.git](https://github.com/heyaniket065/my-video-suite.git)
cd my-video-suite
```

2. Run any module individually (note that `supoclip-main`, `openshorts-main`, and `autoclip_mvp-main` all default to port `8000`, so assign separate ports if running multiple backends together):

* **SupoClip:**
```bash
cd supoclip-main && docker compose up --build
```

* **OpenShorts:**
```bash
cd openshorts-main && docker compose up --build
```

* **OpenReel Video:**
```bash
cd openreel-video-main && pnpm install && pnpm dev
```

* **AutoClip MVP:**
```bash
cd autoclip_mvp-main && docker compose up --build
```

* **PHPVibe CMS:**
Configure your database credentials in `PHPVibe-Video-Sharing-CMS-master/vibe_config.php` and serve via a PHP + MySQL stack.

## Planned Unified Integration

* **Unified Portal UI:** Single sidebar-driven dashboard with dedicated sections for SupoClip, OpenShorts, OpenReel, AutoClip, and PHPVibe.
* **Reverse Proxy Routing:** Nginx path routing (`/supoclip`, `/openshorts`, `/openreel`, `/autoclip`, `/phpvibe`) over Docker Compose.
* **Shared Media Volume:** Common `input/` and `output/` folders so clips generated in SupoClip or OpenShorts open directly in OpenReel.

## Author

* **Aniket Bhalerao** ([@heyaniket065](https://github.com/heyaniket065))
* 
