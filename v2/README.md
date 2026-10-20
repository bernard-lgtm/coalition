# Who can build a coalition? Embeds, v2

Five interactive graphics for Daily Maverick articles, exported from the Metro Coalition Maths canvas:

| File | Graphic | Canvas artboard |
| --- | --- | --- |
| `all-metros.html` | All four metros, with a metro dropdown | All four metros embed v5 |
| `johannesburg.html` | Johannesburg | Johannesburg embed v25 |
| `cape-town.html` | Cape Town | Cape Town embed v5 |
| `tshwane.html` | Tshwane | Tshwane embed v5 |
| `ethekwini.html` | eThekwini | eThekwini embed v5 |
| `fonts/DMCustomMar2026-V2-Bold.woff2` | DM Custom, the headline font | |

Each page holds its graphic, its data and the code that runs it in the one HTML file, with no build step; the five share the DM Custom font file in `fonts/`. Every embed is **920px high** at every width and up to **659px** wide; on phones the layout rearranges inside the same height.

## Putting it on GitHub Pages

Copy this `v2` folder into the root of the `coalition` repository, commit and push. The pages are then served at `https://bernard-lgtm.github.io/coalition/v2/…`, alongside the first-round embeds, which stay where they are so articles already using them keep working. `index.html` is a preview page with all five graphics and their embed codes.

## Embed codes

### All four metros

```html
<iframe src="https://bernard-lgtm.github.io/coalition/v2/all-metros.html" title="Who can build a coalition? Johannesburg, Cape Town, Tshwane and eThekwini" width="100%" height="920" scrolling="no" loading="lazy" style="display:block;width:100%;max-width:659px;height:920px;border:0;"></iframe>
```

### Johannesburg

```html
<iframe src="https://bernard-lgtm.github.io/coalition/v2/johannesburg.html" title="Who can build a coalition in Johannesburg?" width="100%" height="920" scrolling="no" loading="lazy" style="display:block;width:100%;max-width:659px;height:920px;border:0;"></iframe>
```

### Cape Town

```html
<iframe src="https://bernard-lgtm.github.io/coalition/v2/cape-town.html" title="Who can build a coalition in Cape Town?" width="100%" height="920" scrolling="no" loading="lazy" style="display:block;width:100%;max-width:659px;height:920px;border:0;"></iframe>
```

### Tshwane

```html
<iframe src="https://bernard-lgtm.github.io/coalition/v2/tshwane.html" title="Who can build a coalition in Tshwane?" width="100%" height="920" scrolling="no" loading="lazy" style="display:block;width:100%;max-width:659px;height:920px;border:0;"></iframe>
```

### eThekwini

```html
<iframe src="https://bernard-lgtm.github.io/coalition/v2/ethekwini.html" title="Who can build a coalition in eThekwini?" width="100%" height="920" scrolling="no" loading="lazy" style="display:block;width:100%;max-width:659px;height:920px;border:0;"></iframe>
```

The height is set both as an attribute and in the inline style, so the article's CSS can't stretch or squash it.

## Fonts

DM Custom, the headline font, is bundled in `fonts/DMCustomMar2026-V2-Bold.woff2` and served from GitHub with the embeds, so keep the `fonts` folder next to the HTML files. Archivo and Geist load from Google Fonts.
