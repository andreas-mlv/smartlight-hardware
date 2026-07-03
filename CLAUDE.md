# smartlight-hardware

**Created:** 03_07_2026

Append-only archive of compiled SmartLight firmware binaries. Source lives in
`github.com/andreas-mlv/smartlight` (`source/public.esp_firmware/`).

## Structure rules

- Layout: `<variant>/<chip>/<version>_<env>_<dd_mm_yyyy>.bin`
- `variant`: `prod` (IS_DEBUG off) / `dev` (IS_DEBUG serial console on)
- `chip`: `esp8266` / `esp32`; `env`: PlatformIO env (`nodemcuv2`, `d1_mini`, `esp32dev`)
- Version comes from the source repo's `VERSION_PROD.txt` / `VERSION_DEV.txt`,
  patch-bumped on every publish, so filenames are unique and increasing.
- **Never delete** existing binaries; only add.
- Binaries only — no source here.
