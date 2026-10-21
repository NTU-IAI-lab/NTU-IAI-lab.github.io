# Industrial AI Lab website

Source for the Industrial AI Lab website at Nanyang Technological University Singapore, led by Asst. Prof. Marvin Carl May.

## Run locally

Install dependencies once:

```bash
bundle install
```

Start the local preview:

```bash
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Build

```bash
bundle exec jekyll build
```

The built static site is generated in `_site`.

## Team profiles and local images

Edit `group.md` for the team roster. Research Fellows, PhD Students, and Visiting
Scholars and Students use the existing member cards with 110 × 110 px images and
`object-fit: cover`. Master's Students retain the original compact name list,
including the four newly added names. No new master's profile links are added.

Store approved headshots in `assets/img/members/` using lowercase, hyphenated
full names. Use square, optimized JPEGs, normally 200–320 px wide; avoid enlarging
a small source image and remove EXIF metadata. Use the shared local default
`/assets/img/member-placeholder.svg` when a headshot is unavailable or deferred.

### Profile review — 21 October 2026

Kevin Gleich and Sophia Hartmann appear only in Alumni, retaining their existing
LinkedIn links. All eight new members retain the lab-supplied full-name spelling.
The research fellow's portrait was recovered from the current LinkedIn image URL
on [his professional homepage](https://oliverfanhl.github.io/). The remaining six
portraits below were retrieved from the corresponding LinkedIn profile through
the browser's existing session after the old signed image URLs had expired.
All seven headshots are stored locally, without expiring URLs in the website.

| Member | Verified profile / source | Local headshot |
| --- | --- | --- |
| Haolin Fan | [Professional homepage](https://oliverfanhl.github.io/) with his LinkedIn-hosted portrait and NTU identity. | `assets/img/members/haolin-fan.jpg` (200 × 200 px) |
| Muyang Lyu | [LinkedIn](https://www.linkedin.com/in/muyang-lv/), NTU mechanical engineering PhD. | `assets/img/members/muyang-lyu.jpg` (320 × 320 px) |
| Zibo Meng | [LinkedIn](https://www.linkedin.com/in/zibo-meng-875631331/), NTU Research Associate. | `assets/img/members/zibo-meng.jpg` (320 × 320 px) |
| Dave Christopher Hong | [LinkedIn](https://www.linkedin.com/in/davechristopherh/), Industrial AI PhD at NTU. | `assets/img/members/dave-christopher-hong.jpg` (320 × 320 px) |
| Maurus Keeve | [User-confirmed LinkedIn](https://www.linkedin.com/in/maurus-keeve/), NTU and KIT industrial engineering. | `assets/img/members/maurus-keeve.jpg` (320 × 320 px) |
| Valentin Weiss | [User-confirmed LinkedIn](https://www.linkedin.com/in/valentin-weiss-7b7578249/), NTU and KIT industrial engineering. | `assets/img/members/valentin-weiss.jpg` (320 × 320 px) |
| Jennifer Mona Liesen | [User-confirmed LinkedIn](https://www.linkedin.com/in/jennifer-liesen/); profile display name Jennifer Liesen, full name supplied by the lab. | `assets/img/members/jennifer-mona-liesen.jpg` (320 × 320 px) |

Per the lab's follow-up instruction, headshots and profile links for **Raphaël
Etienne, Robin Schumacher, and Christian Stricker** are deferred. They retain
the local default placeholder and plain-text names. Master's Students have no
headshots; no further professional-profile research is required for that section.
No additional home affiliations or more specific visiting appointments were
inferred. These photographs remain subject to their owners' rights; no broader
license is asserted for third-party photographs.

The principal investigator and other categories remain outside this image
migration. Existing styles, scripts, bachelor's roster, and Other Members are
unchanged. The master's list keeps the existing Wentian Xiao profile link.

Validation: `bundle exec jekyll build --trace` passed. All 48 members are unique;
all ten scoped image assets exist and load (seven portraits, three placeholders).
Desktop (1440 px) and mobile (375 px) checks confirmed 110 × 110 px image content
areas, no horizontal overflow, and the master's list in two columns on desktop
and one column on mobile, with no master's headshots.

## Template

This site is adapted from the Minimal Light academic website template.
