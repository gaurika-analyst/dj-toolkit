# Brand kit

The mark, a wordmark, and how to use them. Take them for a poster, a slide, a sticker or a post about DJ Toolkit, so
nobody has to guess. The files are in [`design/brand/`](../../design/brand/) and are free to share under the project's
[MIT licence](../../LICENSE).

![The mark and the wordmark on a Daylight background (left) and a Booth background (right). The dashed square around the
first mark is its clear space.](../../design/brand/overview.svg)

## The mark

A tile with five waveform bars. Use the files as they are: redrawing it, changing its proportions or its colours, or
adding shadows and effects needs its own issue.

The same mark lives in four places, and they change together: `website/public/favicon.svg`,
`website/src/components/BrandMark.astro`, `BrandMark` in `djtoolkit/ui/widgets.py`, and the files here. The app icon is
drawn from the favicon by `tools/make_icon.py`. Inside the app the tile takes the accent colour a DJ has chosen. The
files here are the neutral mark: the one in the favicon and the app icon.

## Which version goes where

Each version is made for one kind of background. The numbers are contrast ratios, measured the way `theme.py` measures
them (3:1 is the least a shape needs to be seen), against the background of Daylight (`#ebe7de`) and of Booth
(`#0e0d0c`).

| File | Use it on | On Daylight | On Booth |
|---|---|---|---|
| [`mark-color.svg`](../../design/brand/mark-color.svg) | light backgrounds, white paper | 14.1:1 | 1.1:1, don't |
| [`mark-black.svg`](../../design/brand/mark-black.svg) | one-colour printing in black: stamps, stickers, newsprint | 17.0:1 | 1.1:1, don't |
| [`mark-white.svg`](../../design/brand/mark-white.svg) | dark backgrounds | 1.2:1, don't | 19.4:1 |
| [`wordmark.svg`](../../design/brand/wordmark.svg) | light backgrounds | 14.1:1 | 1.1:1, don't |
| [`wordmark-light.svg`](../../design/brand/wordmark-light.svg) | dark backgrounds | 1.1:1, don't | 17.5:1 |

On a photo or a busy background, put the mark on a plain area, or on a plain tile of Daylight or Booth.

## The wordmark

"DJ Toolkit" in Inter Bold, 24 px with the letters pulled in by 0.5 px, converted to outlines. It looks the same on every
computer, without Inter installed, so use the file and don't retype the name in another font. The file has no padding:
the clear space below is yours to add.

Inter is under the SIL Open Font License 1.1 (Copyright (c) 2016 The Inter Project Authors,
<https://github.com/rsms/inter>), which allows using its letters in artwork like this. The outlines were drawn from
Inter 4.1, and no font file is in this repository.

## Minimum size

| | On screen | In print |
|---|---|---|
| Mark | 16 px, the size of the favicon | 6 mm |
| Wordmark | 64 px wide | 20 mm |

At 16 px the gaps between the bars of the mark are already under one pixel (about 0.9 px), so that is the smallest it
can go: below it the bars run together. At 64 px wide the capital letters of the wordmark are about 10 px tall.

## Clear space

Keep a quarter of the item's height free on every side: 7 units around the 28-unit mark (14 px around a mark that is
56 px tall, the dashed square in the picture), and a quarter of its height around the wordmark. No other text, edge or
picture goes into that space.

## Don't

- Don't recolour the mark outside the app. The accent colours belong to the app's own interface.
- Don't stretch, rotate or crop it, and don't round the tile differently.
- Don't put the colour or black version on Booth, or the white version on Daylight: the tile disappears.
- Don't set the name in another font.
