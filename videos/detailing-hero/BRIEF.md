---
workflow: general-video
flow: automation
storyboard: yes
message: "Showroom-level paint correction, done by hand, brought to you"
destination: website-hero
aspect: 1920x1080 + 1080x1920
language: en
length: ~10s seamless loop
---

## Intent

A muted, looping background hero video for a mobile car detailing business's website.
Clean footage only: no text baked in, because the site's own HTML headline and CTA sit on top.
Dark premium grade so the paint and polisher stand out and the garage background recedes.

## Assets

- media/source-IMG_4558.mov — the user's own 12s vertical iPhone clip (HEVC 1080x1920 @ 60fps): a gloved hand running a dual-action polisher over a dark metallic car's rear quarter panel and roof edge, windows masked with green tape. This is the only footage.

## Customizations

- Two deliverables: 16:9 desktop hero and 9:16 mobile hero.
- Dark premium grade (moody contrast, deeper blacks, light slow-motion feel).

## Notes

- Silent: website hero videos autoplay muted, so audio is stripped.
- Avoid ~3.6–5.0s of the source: the operator's bare arm sweeps across and blocks the camera.
- The background has a white wall sign and cleaning supplies; the grade/vignette should push them back.
- Source is iPhone HLG HDR; it is tonemapped to SDR Rec.709 (assets/polish-sdr.mp4, regenerable, not committed).
- The dark grade is baked with ffmpeg into assets/polish-graded.mp4 (sharp layer) and assets/polish-bg.mp4 (blurred fill), because the realtime WebGL grade renders minutes-per-frame in this GPU-less container.
- GSAP is vendored at assets/vendor/gsap.min.js because the render browser cannot reach cdn.jsdelivr.net here.
