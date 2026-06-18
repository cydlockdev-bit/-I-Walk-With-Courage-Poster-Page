# I Walk With Courage Poster Page

A responsive motivational poster-style webpage built with **HTML** and **CSS**.
This project displays a full visual poster card with an image background, glowing text, decorative dividers, and a custom footer for **SJ TECH**.

## Live Demo

[View Live Project](https://cydlockdev-bit.github.io/-I-Walk-With-Courage-Poster-Page/)

```

## Screenshot

![I Walk With Courage Poster Screenshot](./assets/iimages/screenshot_I_walk_with_courage.png)
```

## About This Project

This project was created as a front-end practice page to improve my skills with:

- Mobile-first responsive design
- Image overlays
- Absolute positioning
- CSS `clamp()` for responsive text
- Flexbox layout
- CSS animations
- Custom footer design
- Accessibility-friendly HTML structure

The main message of the page is:

> I walk with courage into what I do not yet see.

The design is meant to feel like a digital motivational poster with warm glowing orange text placed over a background image.

## Features

- Responsive poster-card layout
- Mobile-first CSS
- Text overlay positioned on top of an image
- Glowing animated heading
- Decorative icon dividers
- Footer with logo, title, email link, and copyright
- Uses `object-fit: cover` for responsive image handling
- Uses `clamp()` for flexible text sizing
- Uses semantic HTML elements such as `main`, `section`, and `footer`

## Technologies Used

- HTML5
- CSS3
- Flexbox
- CSS Media Queries
- CSS Animations
- Tabler Icons
- Google Fonts / Cinzel font style

## What I Practiced

This project helped me practice how to build a visual webpage that works across different screen sizes.

Some of the main CSS concepts I worked with include:

```css
position: absolute;
object-fit: cover;
clamp();
@media queries;
text-shadow;
animation;
flexbox;
```

## Responsive Design

The page was designed mobile-first and then adjusted for larger screens using media queries.

Main breakpoints used:

```css
@media (min-width: 480px) {
}
@media (min-width: 768px) {
}
@media (min-width: 1024px) {
}
```

The layout is tested for common mobile widths such as:

- 380px
- 390px
- 430px
- 480px

## Accessibility Notes

This project keeps the main quote as real HTML text instead of baking the words directly into the image. This helps with:

- Screen readers
- Browser zoom
- Text scaling
- Better readability
- Better search engine understanding

Decorative dividers are marked with:

```html
aria-hidden="true"
```

This helps screen readers skip visual-only decoration.

## Project Structure

Example file structure:

```text
project-folder/
│
├── index.html
├── style.css
│
└── assets/
    └── iimages/
        ├── walk_with_courage.png
        └── SJ Tech logo with eye design.png
```

## Important Code Highlight

The poster image fills the card without stretching:

```css
.image {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  object-position: center;
}
```

The message is placed over the image:

```css
.message {
  position: absolute;
  top: 8%;
  left: 0.6rem;
  z-index: 2;
}
```

The heading uses a glowing pulse animation:

```css
@keyframes pulse {
  0% {
    transform: scale(1);
  }

  50% {
    transform: scale(1.12);
  }

  100% {
    transform: scale(1);
  }
}
```

## Future Improvements

Possible improvements for this project:

- Add a stronger dark overlay behind the text for better contrast
- Add a desktop layout with different text placement
- Add a reduced-motion option for accessibility
- Improve image file naming by removing spaces from filenames
- Add a favicon
- Add a project screenshot to the README
- Add a live GitHub Pages demo link

## Author

**John Syders**
SJ TECH
Email: [cydlock.dev@gmail.com](mailto:cydlock.dev@gmail.com)

## License

This project is for personal learning and portfolio development.
