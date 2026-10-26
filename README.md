# castesan.github.io

Personal site of Raúl Castellanos Sánchez, served by GitHub Pages at https://castesan.github.io. Static HTML and CSS, no build step. Built on the free [Strata](https://html5up.net/strata) template by HTML5 UP (CC BY 3.0, see `LICENSE-strata.txt`; the credit in the footer must stay).

## Layout

| Path | What it is |
|---|---|
| `index.html` | The whole page: header (photo, name, headline, CV buttons, about), tabbed sections, footer. Edit this to change any text. |
| `assets/css/main.css` | Strata's own stylesheet. Do not edit. |
| `assets/css/custom.css` | Our overrides: fonts (Inter, Playfair Display), colours, header tint, tabs and cards. Colours are the variables at the top of the file. |
| `assets/js/` | Strata's scripts (jQuery, parallax, responsive footer). Unchanged. The tab script is inline at the end of `index.html`. |
| `images/avatar.jpg` | The round photo in the header. |
| `images/bg.jpg` | The header background, shown through a violet tint. |
| `files/` | The downloadable CVs, `CV_Raul_Castellanos_EN.pdf` and `CV_Raul_Castellanos_ES.pdf`. |
| `privacidad.html` | Privacy policy of the Gmail classifier. Kept as is; not part of this template. |

## Changing the photo and the background

Replace the two files, keep the names, do not touch the HTML:

- **`images/avatar.jpg`** — square, at least **600 × 600 px** (1:1). It is shown as a circle 100 px wide, so centre the face: anything near the corners is cut. JPEG, under 150 KB. A non-square photo also works (the CSS crops it to a centred square), but crop it yourself to control what shows.
- **`images/bg.jpg`** — on desktop it fills a tall left column (about 35 % of the window width, full height); on phones it fills a wide band at the top. It is cropped to cover both, centred, and tinted with the violet gradient. Use a **vertical or square** image, **1200 × 1600 px** (3:4) or **1600 × 1600 px**, with the interesting part in the middle. JPEG, under 300 KB. A plain dark image is also fine: the tint does the rest.

To make the tint lighter or remove it, edit the two `linear-gradient(...)` lines under `#header` and `#footer` in `custom.css` (lower the `0.88` alpha, or delete the gradient line to show the photo as is).

## Changing texts

Everything is in `index.html`. The header texts are in `<header id="header">`; each tab is a `<section class="tab-content">` whose `id` matches a `data-tab` button in `.tab-nav`. A job, degree or course is a `<div class="card">` (add `compact` for one without bullet points). The source of truth for the content is the CV (`cv-en.md` in the radar-ofertas project): change it there first.

## Updating the CVs

Copy the regenerated PDFs over `files/CV_Raul_Castellanos_EN.pdf` and `files/CV_Raul_Castellanos_ES.pdf`.
