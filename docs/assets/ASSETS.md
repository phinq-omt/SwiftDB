# Replacing placeholders

The homepage reserves two frames. Neither file is loaded until you add it.

| Frame | Ratio | Suggested size | Replace with |
| --- | --- | --- | --- |
| Screenshot | 16:10 | 1440 × 900 | Compressed WebP or PNG |
| Video | 16:9 | 1280 × 720 | MP4, `preload="none"`, with a poster image |

Set `width` and `height` to the file’s pixel size so the layout does not jump. Write alt text that describes the interface shown. Remove `role="img"` from the frame and the “Placeholder — replace later” caption.

Keep credentials and private records out of screenshots and video.

Serve the site locally with:

```sh
python3 -m http.server 8000 --directory docs
```
