# Source Evidence Manifest

- File: theme-436950476820499404 (3).xml
- Size: 355,162 bytes
- Lines: 2,861
- SHA-256: 5e52f84ec39a50072d47b0ac3d06603b905c0c160141ce86bace446a4ea1144
- Handling: inspected as untrusted text; no theme JavaScript was executed.
- Publication: source XML intentionally not committed to this public repository.

## Static inventory

| Item | Count / observation |
|---|---|
| Script tags / script-like blocks | 15 detected by lexical scan |
| Image tags | 11 |
| Iframe tags | 2 |
| Anchor tags | 92 |
| H1 / H2 / H3 tags | 4 / 10 / 11 in source |
| Meta tags | 31 |
| Link tags | 53 |
| Buttons | 16 |
| Tables | 0 explicit table tags in source |

## XML validation

A standard XML parser fails at line 988, column 110 with an unbound xlink prefix. The root element does not declare xmlns:xlink, while the source uses xlink:href. This result applies to the supplied file as parsed; it is not proof that Blogger currently rejects the theme.

## Known third-party endpoints in source

- Google Tag Manager / gtag.js
- Google AdSense
- Google Charts loader
- Google Fonts
- Blogger-hosted image assets
- WhatsApp, Telegram, Facebook, Instagram, X/Twitter, YouTube links

Endpoint presence is not itself a security defect. Each endpoint and its role should be confirmed against the intended site configuration.

## Limitations

This manifest is a source-level inventory, not a browser crawl. It does not establish live HTTP status, runtime network requests, Core Web Vitals, search indexing, or the validity of Blogger-rendered metadata.