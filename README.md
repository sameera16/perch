# Perch 🪺

**A gentle, privacy-first desktop coach for your eyes and posture.**

Perch uses your Mac's camera **locally** (on-device AI) to watch your blink rate, screen distance, posture, and lighting — then gives small, well-timed nudges to look away, sit back, or fix your setup. **No video, images, audio, or face data ever leaves your Mac.**

This public repository is used for **release downloads only** — the app source code is not published here.

---

## Download

Grab the newest build from the [**latest release**](https://github.com/sameera16/perch/releases/latest):

- **Apple Silicon Mac** → `Perch-<version>-arm64.dmg`
- **Intel Mac** → `Perch-<version>.dmg`

> **Not sure which Mac you have?** Click the **Apple menu → About This Mac** and look at **Chip**: if it starts with **Apple** (M1, M2, M3, or M4), choose Apple Silicon; if it says **Intel**, choose Intel.

### Install

1. Open the DMG and drag **Perch** into **Applications**.
2. In Applications, **right-click Perch → Open**, then click **Open** again.
   *(Perch isn't notarized by Apple yet, so this one-time step is required — after that it opens normally.)*
3. When macOS asks, **Allow** camera access.

The first launch can take a little longer while macOS scans the app — that's normal and only happens once.

---

## Ask Claude about your own data (optional)

The latest release also includes **`Perch-<version>.dxt`** — a local [Claude Desktop](https://claude.ai/download) extension. Double-click it to install (no terminal, no setup), then ask Claude natural-language questions about your own trends:

- *"When during the day is my posture worst?"*
- *"Is my blink rate below my baseline in the afternoons?"*
- *"Which nudges do I dismiss most?"*

It's **read-only** and fully local: it reads only the small hourly aggregates Perch keeps on your machine — never video, images, or face landmarks — and nothing leaves your Mac except what you choose to send to Claude.

---

## Screenshots

### The dashboard

Live blink rate, screen distance, posture, lighting, and call-readiness — all computed on-device.

![Perch dashboard](docs/dashboard.png)

### Private by design

The camera preview is **off by default** — Perch runs without ever showing you. When you do turn it on, you see live tracking points overlaid on the feed, and processing stays entirely on-device: no frame is saved or sent.

![Detection view with tracking points overlaid](docs/detection.png)

> *The face in this screenshot is blurred by us for the README — it's a real camera frame we didn't want on a public page, not an in-app effect.*

### Ask Claude about your trends

With the `.dxt` extension installed, Claude reads your local aggregates and answers questions in plain language.

![Claude summarizing Perch data](docs/claude.png)

---

## Privacy

All processing happens **on-device**. Perch never uploads video, images, audio, face/pose landmarks, or screen contents. Optional anonymous analytics are **off by default**.

This is a behavior-coaching tool, not a medical device — it does not diagnose or detect any medical condition.
