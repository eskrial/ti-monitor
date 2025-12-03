
# TI-monitor

A lightweight web dashboard for monitoring the Telematics Infrastructure (TI) and internet quality in real time.
`TI-monitor` displays the current status of TI services using the official [Gematik Lagebild](https://fachportal.gematik.de/ti-status) API and measures [internet performance](https://speed.cloudflare.com/) (ping & jitter).  
It includes automatic refresh and WebPush notifications for TI service outages.

**Live Demo:** [yourproject.pages.dev](https://yourprojectare)

---

## Features
- **Real-time TI status** via Gematik API (`lageapi/v2/tilage`)
- **Internet quality measurement** (ping & jitter) using Cloudflare
- **Auto-refresh** every 60 seconds
- **WebPush notifications** for TI service issues (internet does not trigger alerts)
- Responsive HTML/CSS, no external frameworks

---

## Notifications
- On first load, the page requests permission for system notifications.
- If a TI service is **restricted** or **down**, a warning notification appears.
- Internet status does **not** trigger notifications.

---

