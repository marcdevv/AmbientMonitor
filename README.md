# Ambient Monitor

Ambient Monitor turns a secondary display into an ambient extension of games, films, and other screen content.

![Ambient Monitor Icon](Ambient_Monitor_Icon.png)

## Browser version

The browser version lives in [docs/index.html](docs/index.html) and is published through GitHub Pages.

**Features**
- Live settings GUI with brightness, contrast, blur, zoom, and flip controls.
- Adjustable source crop: full screen, left half, right half, or a custom region.
- Drag the crop selection and its corner handles in the Crop tab.
- Independent fade-to-black controls for the top, right, bottom, and left edges.
- Animated noise overlay with adjustable opacity, grain size, and refresh rate.
- Settings saved locally in the browser, plus JSON import/export.
- Named local profiles, fullscreen mode, and keyboard shortcuts.

### Run it

Open the hosted browser version using a modern browser that supports screen capture. Screen capture requires HTTPS (GitHub Pages qualifies) or localhost. Press **Choose screen to capture** and select the screen/window you want to sample. The browser controls the capture permission and may show a confirmation indicator.

For the best multi-monitor experience, open Ambient Monitor on the target secondary display, then select the screen you want to capture. Avoid selecting the Ambient Monitor output itself, which can create a feedback loop.

### Browser controls

| Key | Action |
|---|---|
| `Tab` | Toggle the settings panel |
| `F` or `Space` | Toggle fullscreen |
| `Enter` | Cycle full screen, left half, and right half (when the settings panel is not focused on an input) |
| `1` / `2` | Decrease / increase brightness |
| `3` / `4` | Decrease / increase contrast |
| `5` / `6` | Decrease / increase zoom |
| `7` / `8` | Decrease / increase blur |
| `9` | Export settings as JSON |
| `0` | Reset settings |

### Settings and compatibility

- Settings are stored in this browser's local storage. Clearing browser site data removes them.
- Export a JSON file to back up settings or transfer them to another browser.
- Saved profiles are local to the browser and device.
- Browser screen capture is controlled by the browser/operating system. Some browsers may limit which display surfaces can be selected.
- The browser version stretches the selected source region to fill the ambient output. Crop selection is expressed in percentages of the captured source.

## Python downloadable version

The original Python implementation is retained in the repository's previous revisions. Its legacy keyboard controls are documented in the corresponding historical scripts.
