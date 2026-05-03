# Tsui Dot

[日本語](README.md)

Tsui Dot is a Tsui-series tool that converts photos, illustrations, and the local camera feed into 8-bit-style 2D pixel art or a glass-window-style framed view, entirely inside the browser.

- No login
- No ads
- No install (the Cloudflare version is also installable as a PWA)
- No external modules / no CDN / JavaScript only
- No outbound traffic from the app itself (CSP `connect-src 'none'`)
- Full-image pixelization with `MODE full`
- Partial pixelization through a movable glass window with `MODE window`
- PNG export

---

## Web version (Cloudflare Pages, PWA-ready)

Available at:
[https://tsuidot.pages.dev/](https://tsuidot.pages.dev/)

## Download version

The latest build is distributed via GitHub Releases.

- **Repository**: [https://github.com/hajimetwi3/Tsui-dot](https://github.com/hajimetwi3/Tsui-dot)
- **Latest release**: [https://github.com/hajimetwi3/Tsui-dot/releases/latest](https://github.com/hajimetwi3/Tsui-dot/releases/latest)
- The artifact is a single file, `tsui-dot.html`. No installation step.

To verify the artifact, compare the SHA-256 hash listed on the Release page with the hash of your local file.

## Quick start

### Single-file HTML version

```
1. Open tsui-dot.html in your browser.
2. Click "Image" to load a photo or illustration.
3. Adjust MODE / DOT / SIZE / GLASS and other controls.
4. Click "PNG" to save the result.
```

### Camera

Choose `CAM back / front` to set rear- or front-preferred, then click `CAMERA` to start the local camera. Use `FIX` to freeze the current frame.
The browser will ask for camera permission. In some environments cameras are unavailable from `file://`, so HTTPS hosting (such as Cloudflare Pages) or `localhost` is recommended.


## PRIVACY

Images and camera frames are not sent outside this app.
`connect-src 'none'` blocks `fetch` and other network requests at the browser level.

Image data and camera frames are not stored in `localStorage` or `IndexedDB`.
Only UI preferences (such as DOT size and palette) are saved.


## Notes

- This software is provided as-is, with no guarantees about correctness or availability. Use at your own risk.
- You are responsible for saving and managing exported images.
- Camera support depends on your browser and on the security context of the host.
- This repository does not currently accept external pull requests.

## License

[MIT License](LICENSE)

© 2026 Hajime Tsui

## Third-party

None. No external modules.

## Announcements

- Announced on X:
[https://x.com/hajimetwi3/status/2050477785224036739](https://x.com/hajimetwi3/status/2050477785224036739)

---

## Author

[Hajime Tsui](https://hajimetwi3.github.io/hajimetwi3/)
