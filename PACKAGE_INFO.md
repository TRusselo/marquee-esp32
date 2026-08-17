# Version information

- Version: `2.2.1-esp32-enhanced.4`
- Upstream base: [`Jamisonfitz/marquee`](https://github.com/Jamisonfitz/marquee) v2.2.1
- ESP32/ESPHome fork: this repo ([`TRusselo/marquee-esp32`](https://github.com/TRusselo/marquee-esp32))
- Enhanced Designer edition: contributed by [`pqpxo`](https://github.com/pqpxo/marquee-esp32)

## What the enhanced edition adds

- Viewer, Device, Stream, Active streams, and Audio & subtitles Designer blocks
- A common Plex, Emby, and Jellyfin session/playback payload
- Eligible-session rotation position and count
- Metadata-change capture in `marquee-shot` (session/stream/tracks/design), so the
  ESP32 panel refreshes on more than just title changes
- Equal-height session cards with independent background and border switches
- An 800 × 480 default Design viewport plus Nest Hub, 16:9, 4:3, and custom sizes
- Optional Local/Remote label on the Device block
- Server-wide Active streams block
- A separate Street rain-animation switch
- A removable/addable Credits Badge block
- Independently movable Street poster-light frame and NOW PLAYING sign
- Centered, bounded title-logo fitting with transparent-padding trim,
  contain/width/natural modes, and 50–200% zoom
- Separate Category and Title blocks
- Fifteen named per-block fonts plus the theme default
- Persistent custom-backdrop upload with image-adjustment controls
- The Home-Assistant-controlled `esphome/marquee-elecrow-7.yaml` panel config
- Backward-compatible settings and presets

See [ENHANCEMENTS.md](ENHANCEMENTS.md) for feature details and
[CHANGELOG.md](CHANGELOG.md) for the per-version history.

## Validation

- `python3 cast/cast.py --selftest`
- `python3 sidecar/shot.py --selftest`
- `docker compose config`
- Inline JavaScript syntax check of `cast/settings.html` and `output/index.html`
- Enhanced panel config `esphome/marquee-elecrow-7.yaml` verified on hardware
  (Elecrow CrowPanel 7") with the Home Assistant controls
