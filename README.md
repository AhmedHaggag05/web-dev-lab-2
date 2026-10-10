# Lab 2: Simple Personal Portfolio

Open `index.html` in a browser. No installation or server is needed.

This is a simple HTML and CSS portfolio for CSE343 Lab 2: a header, About Me section, three project cards, contact links, and a footer. The personal information and project descriptions come from Ahmed's CV, with the year of study updated to third year.

## What each file does

- `index.html` contains the content and structure of the page.
- `styles.css` controls the colors, spacing, fonts, and layout.
- `README.md` explains the work; it is not part of the webpage.

## Understanding the HTML

1. `<!DOCTYPE html>` tells the browser to use modern HTML.
2. `<head>` contains the browser tab title, character encoding, viewport setting, and the link to the CSS file. The viewport setting helps the page fit mobile screens.
3. `<body>` contains the visible page. `<header>`, `<main>`, `<section>`, and `<footer>` give the content a meaningful structure.
4. `<h1>` is the main heading. `<h2>` is used for section headings, and `<h3>` for project titles. `<p>` contains paragraphs.
5. Navigation links such as `href="#about"` jump to the section with `id="about"`. Each ID is unique.
6. All project cards share `class="project-card"`, so one CSS rule can style them all. Their surrounding `<div>` groups them together.
7. `mailto:` opens the user's configured email application. The GitHub and LinkedIn links lead to the profiles listed in the CV.

## Understanding the CSS

- `body` is an element selector: it styles the whole page's default font, text color, and background.
- `header, footer` is a group selector: both get the same dark background and centered text.
- `.project-card` is a class selector: it styles every project card.
- `nav a` selects links inside the navigation, so they can be white while other links are blue.
- `margin` is space outside an element; `padding` is space inside it. `border` surrounds it. These are parts of the box model.
- `box-sizing: border-box` makes a declared width include padding and borders.
- `max-width` limits how wide the main content can become. `margin: 0 auto` centers the main content horizontally.
- `display: flex` places the project cards in a row. `gap` adds space between them, and `flex-wrap: wrap` allows extra rows on smaller screens.
- `flex: 1 1 240px` means each card can grow, shrink, and starts with a preferred width of 240 pixels.
- `border-radius` rounds corners, and `box-shadow` adds a small shadow to the cards.

## A short explanation for the TA

“I made a static personal portfolio using HTML and an external CSS file. It has a header, About section, three projects, contact links, and footer. The navigation links jump to sections using IDs. I used a shared class to style all project cards and Flexbox to arrange them. I used margin and padding for spacing, blue for the header, footer, and headings, and a light background. The information comes from my CV.”

The colors are simple hexadecimal values in CSS. `color` changes text color, `background-color` changes the background, and `border-top` gives the project cards a blue line at the top. For example, `#214e78` is the dark blue used on the page.

## Contact links

The final page uses an email link and GitHub/LinkedIn profile links instead of a contact form. There is no JavaScript, backend, or database.
