# YouTube Hidden Banner

A minimal Chrome extension (Manifest V3) that hides the big statement/promo banner ad (`#big-yoodle` / `ytd-statement-banner-renderer`) shown at the top of the YouTube home feed.

There is no on/off button by design — hiding is always on. To turn it off, disable the extension in `chrome://extensions`.

## Features

- Removes the full-width statement banner ad from the home feed (e.g. car-detailing, brand "showcase" placements)

## How it works

- `hide-banner.css` — injected at `document_start`, hides the banner via `display: none`. No JavaScript needed.

No data is collected and no extra permissions beyond `*.youtube.com` host access.

## Install (unpacked)

1. Open `chrome://extensions`
2. Enable **Developer mode** (top right)
3. Click **Load unpacked** and select this folder
4. Open YouTube — the banner is gone

## Maintenance

YouTube renames elements often. If a new banner variant slips through, add a selector to `hide-banner.css`.

## License

MIT
