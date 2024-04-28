# Prompt

To give to an LLM like GPT-4.

GPT-4 had trouble creating an SVG icon, so I'm using one from Gemini instead.

---

Create a web page by creating files "index.html", "styles.css", "script.js" as described below. Create the files individually in your temporary storage. Afterwards, zip the created files and let me download them. I will supply a site icon named "siteicon.svg". Do not create "siteicon.svg".

## Sticky Header

There is a sticky header containing the site icon, the site name, and four <a> elements style with CSS to make them look like buttons: Home, All Pages, Random Page, Search.

Create a generic site icon using SVG.

Use Headroom.js to hide the sticky header after the user scrolls down a bit, and make it reappear with the user scrolls up.

## Page

The page has two flexbox columns, "side-column" and "main-column". "side-column" is on the left and is 25em wide. "side-column" is an <aside>, and "main-column" is a <main>. Inside the main, we might want <article>.

```css
  .container {
    display: flex;
  }
  .side-column {
    width: 25em;
    background-color: #e0e0e0; /* Slightly darker grey background */
  }
  .main-column {
    flex-grow: 1;
    background-color: #f4f4f4; /* Light grey background */
  }
```

## Collapsible Sections

There are two collapsible sections which each appear twice in the page: "mainmenu" and "contents".

The collapsible sections are either displayed in the "side-column", or as a floating pane, but never both at the same time. When they're a floating pane, they have padding of 2em, and are sized to fit their content. Their top left corners are approximately in the location of their corresponding hamburger menu icon. The floating panes are displayed when the user clicks the corresponding hamburger menu icon. They hide if the user clicks somewhere else on the page.

    <aside id="sidebar" class="sidebar">
        <div class="collapsible" id="mainmenu">
            <h2>Main Menu</h2>
            <ul>
              <li><a href="#">Home</a></li>
              <li><a href="#">All Pages</a></li>
              <li><a href="#">Random Page</a></li>
              <li><a href="#">Search</a></li>
            </ul>
        </div>
        <div class="collapsible" id="contents">
            <h2>Contents</h2>
            <p>Topic 1</p>
            <p>Topic 2</p>
            <p>Topic 3</p>
            <p>Topic 4</p>
            </div>
    </aside>

## Hamburger Menus

The hamburger menu icon for "mainmenu" is displayed to the left of the site icon in the header.

The hamburger menu icon for "contents" is displayed at the top left corner of the main column.

"side-column" hides when the width breakpoint is less than 768px. The hamburger icons are shown if "side-column" is hidden. The hamburger icons are hidden if "side-column" is shown.

"side-column" unhides with the width breakpoint is greate than 768px.

Use some lorem ipsum for "main" content.
