# Profile assets

## Header

The header uses the waving shape from [capsule-render](https://github.com/kyechan99/capsule-render), adapted from the settings in the [GitHub Profile README Editor](https://github-profile-readme-editor.netlify.app/secondstep).

The generated wave geometry is retained. Motion uses CSS transforms and opacity; `prefers-reduced-motion` disables it. The README also selects a separate static SVG for reduced motion.

- `profile-header-wave.svg`: animated wave and entrance lettering.
- `profile-header-static.svg`: static version for reduced motion.
- `profile-header.svg`: static compatibility asset for earlier README links.

Source render request:

```text
https://capsule-render.vercel.app/api?type=waving&color=0:155E75,100:1F6C58&height=180&text=SUJIN%20LEE&animation=fadeIn&fontColor=F7FAFC&fontSize=60
```

The renderer source license is retained in `CAPSULE-RENDER-LICENSE.txt`.

## Type

The header lettering uses [Wanted Sans](https://github.com/wanteddev/wanted-sans), also listed on [Noonnu](https://noonnu.cc/en/font_page/1269).
The Bold Latin font is converted to vector outlines, so GitHub can display the intended lettering without loading a webfont.
GitHub controls the README body font; this asset does not replace it.

Font source: `packages/wanted-sans-std/fonts/ttf/WantedSansStd-Bold.ttf` in the official repository.
Copyright and SIL Open Font License 1.1 are retained in `WANTED-SANS-OFL.txt`.

## Badges

Technology and email badges are static [Shields.io](https://shields.io/) SVGs using the `for-the-badge` style. Colors are adjusted for a minimum 4.5:1 contrast with white text.
Technology icons are supplied by Shields from [Simple Icons](https://simpleicons.org/).

The selected editor's old Hits endpoint did not resolve. The live profile counter uses [GitHub Profile Views Counter](https://github.com/antonkomarev/github-profile-views-counter) without a fabricated base value. It counts image requests, not unique visitors.

## Languages

`README.md` is the English Overview. `README.ko.md` is the Korean version, and `README.en.md` preserves the earlier English file URL with the same English content.
