# Admin Dashboard

A static admin dashboard layout built as part of [The Odin Project](https://www.theodinproject.com/) HTML & CSS curriculum. It practices CSS Grid and Flexbox by recreating a typical dashboard: a fixed sidebar, a top navigation bar, a profile header, a grid of project cards, and a right-hand column for announcements and trending topics.

> This is a front-end layout exercise only. All content is placeholder text and there is no backend or JavaScript.

## Features

- **Sidebar navigation** with a logo and two groups of links (Home, Profile, Messages, History, Tasks, Communities, plus Settings, Help, Privacy)
- **Top nav bar** with a rounded search field, notification icon, and profile picture with username
- **Profile header** with avatar, tagline, handle, and pill-shaped action buttons (New, Upload, Share)
- **Projects grid**: six cards in a two-column grid, each with a title, description, and icon actions (favorite, preview, fork)
- **Announcements panel** with a list of notices
- **Trending panel** with icons and short posts
- **Inline SVG icons** (Material Design Icons paths) colored via CSS `fill`, so they need no external files or icon fonts
- **Montserrat** loaded from Google Fonts, with a `sans-serif` fallback
- **Theme color as a CSS variable** (`--blueBackground`) used for the sidebar, buttons, and accents
- **`rem` sizing** using the `62.5%` root font-size technique (1rem = 10px)

## Project Structure

```
admin-dashboard/
├── index.html
├── styles.css
└── media/
    └── output.jpg      # profile picture
```


## Layout Overview

| Area | Technique |
| --- | --- |
| Page shell (sidebar + main) | CSS Grid, `grid-template-columns: 1fr 4.5fr` |
| Main section rows (nav bar, header, content) | CSS Grid, `grid-template-rows: 0.5fr 0.5fr 5fr` |
| Content area (projects + highlights) | CSS Grid, `3fr 1fr` columns |
| Project cards | Nested CSS Grid, 2 columns x 3 rows |
| Nav items, icon rows, header buttons | Flexbox |
| Section titles ("Your Projects", "Announcements", "Trending") | `::before` pseudo-elements with absolute positioning |

## Technologies

- HTML5 (semantic grouping with `div`s, inline SVG)
- CSS3 (Grid, Flexbox, custom properties, pseudo-elements, `box-shadow`, `object-fit`)
- Google Fonts (Montserrat)

## What I Practiced

- Composing complex layouts from nested Grid and Flexbox containers
- Sizing and coloring inline SVG icons with CSS
- Using CSS variables for a consistent theme color
- Positioning decorative headings with `::before`
- Cropping images into circles with `border-radius` and `object-fit` / `object-position`


## Credits

- Layout project brief from [The Odin Project](https://www.theodinproject.com/)
- Icons: [Material Design Icons](https://pictogrammers.com/library/mdi/)
- Font: [Montserrat](https://fonts.google.com/specimen/Montserrat) via Google Fonts

## Author

**Z-K11** — [GitHub](https://github.com/Z-K11)
