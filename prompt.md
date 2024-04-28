# Prompt

To give to an LLM like GPT-4. GPT-4 had trouble creating an SVG icon, so I'm using one from Gemini instead.

---

Create a web page by creating files "index.html", "styles.css", "script.js" as described below. Create the files individually in your temporary storage. Afterwards, zip the created files and let me download them. I will supply a site icon named "siteicon.svg".

## Sticky Header

There is a sticky header containing the site icon, the site name, and four <a> elements style with CSS to make them look like buttons: Home, All Pages, Random Page, Search.

Create a generic site icon using SVG.

Use Headroom.js to hide the sticky header after the user scrolls down a bit, and make it reappear with the user scrolls up.

## Page

The page has two flexbox columns, "sidebar" and "main". "sidebar" is on the left and is 30em wide. "sidebar" is an <aside>, and "main" is a <main>.

## Collapsible Sections

There are two collapsible sections which each appear twice in the page: "mainmenu" and "contents".

The collapsible sections are either displayed in the sidebar, or as a fixed pane, but never both at the same time. The fixed panes are displayed when the user clicks the corresponding hamburger menu. They hide if the user clicks somewhere else on the page.

## Hamburger Menus

The hamburger menu for "mainmenu" is displayed to the left of the site icon in the header.

The hamburger menu for "contents" is displayed at the top left corner of the main column.

"sidebar" hides when the width breakpoint is less than 768px. The hamburger icons are shown if the sidebar is hidden. The hamburger icons are hidden if the sidebar is shown.

Use some lorem ipsum for "main" content.

Use a short list of topics for "sidebar" content.

