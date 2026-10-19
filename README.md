Simple QR-Code creator. Hosted on Github Pages at https://horaciosalles.github.io/qr-code/.

Everything runs in the browser: no external references, no network requests, nothing you type is uploaded.

## Features

- Generates the code as you type, choosing the smallest QR version that fits.
- Error correction level L, M (default), Q or H.
- Full UTF-8 support, including accented characters and emoji.
- Multi-line text (vCards, Wi-Fi strings, etc.).
- Sharp rendering on any screen size and pixel density, with the standard 4-module quiet zone.
- Download as PNG or SVG, or copy the image to the clipboard.

## Capacity

The largest QR code (version 40) holds, depending on the error correction level:

| Content                              | L    | M    | Q    | H    |
| ------------------------------------ | ---- | ---- | ---- | ---- |
| Digits only                          | 7089 | 5596 | 3993 | 3057 |
| Uppercase A–Z, digits, ` $%*+-./:`   | 4296 | 3391 | 2420 | 1852 |
| Anything else (UTF-8 bytes)          | 2953 | 2331 | 1663 | 1273 |

Accented letters take 2 bytes each and most emoji take 4. Very long codes are dense and harder to scan from a screen; use a lower error correction level to keep them smaller.

## Credits

Uses a local copy of [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) 2.0.4 by Kazuhiko Arase, MIT license.

"QR Code" is a registered trademark of DENSO WAVE INCORPORATED.
