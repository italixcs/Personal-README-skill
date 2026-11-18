# GitHub rendering

## Design for the profile surface

GitHub displays a nonempty root `README.md` from a public repository named for the account. Preserve repository-relative asset paths and filename case. See [GitHub's profile README guide](https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme) and [formatting reference](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

Use GitHub-flavored Markdown for essential content. Keep columns and fixed widths out of the main reading flow when they risk overflow. Use only necessary supported HTML. GitHub performs sanitization, so browser-only layout, JavaScript, embeds, inline SVG markup and CSS-based effects are poor dependencies. Serve simple standalone SVG via an image reference. Audit scripts, external references, embedded HTML and unsafe SVG features before reusing third-party files. Prefer a PNG fallback for an uncertain renderer.

A single asset with its own legible palette can work in both themes. If variants are warranted, use GitHub's [documented picture pattern](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github). Specify dark and light sources with an accessible `img` fallback, and verify each path. Limit GIFs to meaningful accents. Provide text or a static visual for information carried by animation. Avoid depending on an externally refreshed image for core content. If one is requested, document the source and how the profile reads during an outage.

## Check the actual draft

- Check every target and image path, including nested README paths, theme variants, image links and fragments. Spot-check external destinations directly where access allows. Distinguish a verified destination from an unreachable one.
- Check titles, logo usage and every factual claim against the evidence. Review screenshot metadata, image contents and public links for accidental disclosure before handoff.
- Check the small-screen wrapping of icon rows and buttons, the destination of each action, and any cutoff date shown in a stats snapshot.
- Inspect a narrow and a wide layout in light and dark. Check heading order, overflow, contrast, link labels and text alternatives. Give informative images useful alt text. Use empty alt text only for a truly decorative image whose information is available in adjacent text.
- Check real file sizes. Aim for a banner below about 500 KB where quality allows. Keep assets individually meaningful and improve compression without making type or fine details unclear.
- Prefer an authorized GitHub render where available. A local GFM/browser preview supports visual and responsive checks. It cannot establish GitHub.com sanitization, image proxies, GitHub theme overrides, or profile placement. State the preview method and any unverified behavior.
