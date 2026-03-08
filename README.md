# Table Row Generator

A simple browser-based tool for generating Markdown table rows in the format used for visual novel music tracklists.
https://serecola.github.io/ensonglog-editor/

## Output format

```
| 月 | 作品 | ブランド | 曲名 | 種別 | ボーカル | 作詞 | 作曲 | 編曲 | 音源 | その他 | 試聴 |
```

Dates are formatted as `01<!--/30-->` (month/day). Empty fields output as `||` with no spaces.

## Features

- **Import** — paste an existing row to auto-fill all fields for editing
- **Date** — separate month and day inputs, zero-padded automatically
- **Preview links** — pick a platform and paste a URL; formats the markdown link automatically

| Platform | Output |
|---|---|
| YouTube | `[:fontawesome-brands-youtube:](url)` |
| chobit.cc | `[:rabbit:](url)` |
| emdb | `[:octicons-video-16:](url)` |
| Twitter / X | `[:fontawesome-brands-twitter:](url)` |
| HP | `[HP](url)` |
| Bilibili | `[B站](url)` |

- **Accumulate** — add multiple rows and copy the full table at once
- **Dark mode** — toggle in the top right; respects system preference and persists across sessions

## Usage

Open `index.html` in any browser. No install or build step required.

Fill in the fields and click **Generate** (or press `Enter` in any input field). Copy the row directly, or use **+ Add to Table** to build up multiple rows before copying.
