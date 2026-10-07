# May's Restaurant

A multi-page restaurant website built with plain HTML and CSS as a front-end practice project. It covers a home page, a menu with Naira (₦) prices, a photo gallery and a table reservation form.

> **Status:** Work in progress. The HTML structure is complete for all four pages. Styling, images and form handling are still being added (see [Roadmap](#roadmap)).

---

## Table of Contents

1. [Pages](#pages)
2. [Features](#features)
3. [Project Structure](#project-structure)
4. [Getting Started](#getting-started)
5. [Technologies Used](#technologies-used)
6. [What I Practised](#what-i-practised)
7. [Known Issues](#known-issues)
8. [Roadmap](#roadmap)
9. [Contact](#contact)

---

## Pages

| Page | File | What it contains |
|---|---|---|
| Home | `index.html` | Welcome banner, opening hours, today's special, FAQ and contact footer |
| Menu | `menu.html` | Menu items, drinks and beverages in tables, with prices in Naira |
| Reservation | `reservation.html` | Booking form (name, email, phone, date, time, guests, dietary needs, seating, occasion) |
| Gallery | `gallery.html` | Restaurant photos with captions and an embedded map |

---

## Features

- **Opening hours** shown with a description list (`<dl>`).
- **Today's special** with an image and a highlighted dish.
- **FAQ section** using expandable `<details>` and `<summary>` elements, grouped so only one answer opens at a time.
- **Menu tables** for main dishes, drinks and beverages, with prices written with the Naira sign (`&#8358;`).
- **Table of contents link** on the menu page that jumps to a section on the same page.
- **Reservation form** with:
  - required fields and built-in validation (`required`, `type="email"`, `type="tel"`, `type="date"`, `type="time"`)
  - guest limit from 1 to 20
  - dietary needs checkboxes, seating preference radio buttons and an occasion drop-down with grouped options (`<optgroup>`)
- **Photo gallery** using `<figure>` and `<figcaption>`.
- **Footer** with address, email link, phone link and copyright.
- **Responsive meta tag** (`viewport`) on every page.

---

## Project Structure

```
Restaurant-practice-Html-/
├── index.html          # Home page
├── menu.html           # Menu page
├── reservation.html    # Reservation form
├── gallery.html        # Photo gallery
├── style.css           # Shared stylesheet (to be completed)
├── .gitignore
└── README.md
```

Images and favicon files are referenced by the pages and should sit in the same folder as `index.html`:

```
Fine dining.jpg
Barbecue chicken and rice.jpg
fine dining 2.jpg ... fine dining 8.jpg
apple-touch-icon.png
favicon-32x32.png
favicon-16x16.png
site.webmanifest
```

---

## Getting Started

No installation or build step is needed.

### Run it locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Chekwube-devops/Restaurant-practice-Html-.git
   cd Restaurant-practice-Html-
   ```
2. **Open `index.html`** in your browser (double-click it), or
3. **Use Live Server in VS Code** so the page refreshes as you edit:
   - Install the **Live Server** extension.
   - Right-click `index.html` and choose **Open with Live Server**.

### Navigate

Use the links at the top of each page to move between Home, Menu, Reservation and Gallery.

---

## Technologies Used

- **HTML5**: semantic elements (`header`, `nav`, `main`, `section`, `footer`, `address`, `figure`)
- **CSS3**: single shared stylesheet (`style.css`)
- **Git and GitHub**: version control and hosting

---

## What I Practised

- Structuring a multi-page site with semantic HTML
- Building forms with labels, input types, validation, checkboxes, radio buttons and select menus
- Using tables, description lists and expandable details
- Linking pages together and linking to sections on the same page with `id` anchors
- Adding images with alt text and captions
- Using HTML entities such as `&#8358;` for the Naira sign and `&copy;` for the copyright sign

---

## Known Issues

- `style.css` is currently empty, so pages use the browser's default styling, and `gallery.html` does not yet link to it.
- The reservation form posts to `submit_reservation.php`, which does not exist, so submitting does nothing yet.
- Some form fields share the same `id`/`name` values and need to be made unique.
- Image and favicon files need to be added to the repository, and some image filenames contain spaces.
- The map on the gallery page uses a short share link that cannot be embedded; it needs a proper Google Maps embed URL.
- The navigation menu differs between pages.
- The phone link should use the international format (`tel:+2349067509444`).

---

## Roadmap

- [ ] Write `style.css`: colours, typography, spacing and layout
- [ ] Make the layout fully responsive for phones and tablets
- [ ] Add all images and favicons to the repository
- [ ] Fix form `id`/`name` attributes and group options with `<fieldset>`
- [ ] Connect the reservation form to a form service or backend
- [ ] Use one consistent navigation menu and footer on every page
- [ ] Embed a working Google Map
- [ ] Add a table of contents and "back to top" links on long pages
- [ ] Publish the site with GitHub Pages

---
---

## License

This is a learning project. Add a license here if you decide to share or reuse the code (for example, the [MIT License](https://choosealicense.com/licenses/mit/)).
