# zmk-sofle

ZMK config for an Eyelash Sofle with **nice!view** displays and a nice!nano v2.

- Upstream: https://github.com/a741725193/zmk-sofle (branch `main`). Add it as the `upstream` remote.
- Never merge from `a741725193/zmk-sofle-oled` — same author, but it drives an SSD1306 OLED on the nice!view header pins. Merging it blanks both screens.
- `boards/shields/eyelash_sofle/` should stay identical to upstream; only `config/` and `build.yaml` are ours.
- Firmware is built by GitHub Actions; artifacts are `eyelash_sofle_{left,right} nice_view-nice_nano_v2-zmk.uf2`. `settings_reset` is a pre-flash step, never the final flash.
