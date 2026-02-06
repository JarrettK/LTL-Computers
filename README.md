# HTML Basics

## Welcome to HTML

Today you're learning the basics of HTML (HyperText Markup Language), which is the foundation of every website on the internet. We'll be building a simple fan page about The Lord of the Rings.

---

## Key Concepts

### What is HTML?

HTML is a **markup language** that tells web browsers how to display content. It uses **tags** to structure text, images, links, and other elements on a webpage.

### What are Tags?

Tags are keywords surrounded by angle brackets, like `<tagname>`. Most tags come in pairs:

- **Opening tag**: `<tagname>`
- **Closing tag**: `</tagname>`

The content goes between these tags: `<tagname>content</tagname>`

---

## Breaking Down HTML Pages

### 1. The Document Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    ...
</head>
<body>
    ...
</body>
</html>
```

**Every HTML page needs these parts:**

- `<!DOCTYPE html>` - Tells the browser this is an HTML5 document
- `<html>` - The root element that contains all other elements
- `<head>` - Contains information ABOUT the page (not displayed on the page itself)
- `<body>` - Contains everything that WILL be displayed on the page

### 2. The Head Section

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Lord of the Rings - Fan Page</title>
</head>
```

- `<meta charset="UTF-8">` - Tells the browser how to read characters (supports emojis, special characters, etc.)
- `<meta name="viewport"...>` - Makes the page display properly on different screen sizes
- `<title>` - Text that appears in the browser tab (not on the page itself)

### 3. The Body Section

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Lord of the Rings - Fan Page</title>
</head>
```

- `<meta charset="UTF-8">` - Tells the browser how to read characters (supports emojis, special characters, etc.)
- `<meta name="viewport"...>` - Makes the page display properly on different screen sizes
- `<title>` - Text that appears in the browser tab (not on the page itself)

#### 4. Headings

```html
<h1>The Lord of the Rings</h1>
<h2>About the Series</h2>
<h3>Interesting Facts</h3>
```

**Headings organize your content:**

- `<h1>` - Main title (most important, largest) - use only ONE per page
- `<h2>` - Major sections
- `<h3>` - Subsections
- Goes down to `<h6>` (smallest)

Think of them like an outline - `H1` is your title, `H2` is your main points, `H3` is your sub-points.

#### 5. Paragraphs

```html
<p>The Lord of the Rings is an epic fantasy adventure...</p>
```

The `<p>` tag creates a paragraph of text. Browsers automatically add spacing above and below paragraphs.

#### 6. Lists

**Unordered Lists** *(bullet points)*:

```html
<ul>
    <li>The Fellowship of the Ring</li>
    <li>The Two Towers</li>
    <li>The Return of the King</li>
</ul>
```

- `<ul>` = **U**nordered **L**ist *(creates bullets)*
- `<li>` = **L**ist **I**tem *(each bullet point)*

<!-- cSpell: disable-next-line -->
**Note:** There's also `<ol>` for **O**rdered **L**ists *(numbered lists)*. Same structure, just starts with `<ol>` instead of `<ul>`.

```html
<ol>
    <li>The Fellowship of the Ring</li>
    <li>The Two Towers</li>
    <li>The Return of the King</li>
</ol>
```

#### 7. Images

```html
<img>The Lord of the Rings is an epic fantasy adventure...</p>
```

The `<img>` tag is used for adding an image to a page. For accessibility, you should always add `alt` tags to your images, which provide spoken context to users utilizing screen readers. Browsers automatically ...

#### 8. Links

- **Links** (`<a>` tags) to connect pages

#### 9. Tables

- **Tables** to organize data

#### 10. Forms

- **Forms** for user input

---

## Important HTML Rules

1. **Tags Must Be Properly Nested**
   - Tags need to be properly nested, meaning that an opening tag should usually... need a short sentence or two description explaining how to know the scoping.
   - ✅ Correct: `<p>This is <strong>bold</strong> text.</p>`
   - ❌ Wrong: `<p>This is <strong>bold</p></strong> text.`

2. **Most `tags` Need Accompanying Closing `tags`**
   - Opening: `<p>`
   - Closing: `</p>`
     - Notice the `/` in the closing tag

3. **Indentation Matters for Readability**
   - Child elements should be indented inside parent elements
     - *(e.g., `td` inside `tr` and `tr` inside `table`)*
   - This doesn't affect how the page looks, but makes code easier to read

4. **Case Doesn't Matter for `tags` *(but lowercase is standard)***
   - `<P>` and `<p>` both work
   - As a best practice, always use lowercase for `tag text`

5. **Always Follow *(at least)* WCAG AA Accessibility Standards** <!-- cSpell: disable-line -->
   - This is important to ...
   - Stuff here...

---

## How to View Your HTML

1. Save your file with a `.html` extension *(like `index.html`)*
2. Open the file with a web browser *(double-click it, or right-click → Open With → Browser)*
   - You can also [click the `Show Preview` button](https://raw.githubusercontent.com/microsoft/vscode-livepreview/main/img/open-preview-btn.gif) in VS Code *(if you have the [`Live Preview` extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.live-server) installed)*.
3. The browser *(or extension)* will render your HTML into a formatted webpage!

---

## What's Next?

Later on, you'll learn:

- **CSS** to make your page look beautiful (colors, fonts, layouts)
- ***(OUTSIDE SCOPE OF THIS COURSE)*** - **JavaScript/TypeScript** to make your page interactive *(buttons that do things, animations, etc.)*

---

## Practice Challenge

Create your own HTML page to:

1. Display the title to your favorite book, movie, game, or band
2. Add a new `<h2>` section
3. Create a list of your favorite characters, albums, or facts
4. Add a paragraph explaining why you like it

Remember: Save the file and refresh your browser to see changes!

---

## Common Questions

**Q: What if I forget to close a tag?**
A: The browser will try to guess what you meant, but it might look wrong or not render at all. Always close your tags!

**Q: Do spaces in my HTML matter?**
A: Browsers usually ignore extra spaces and line breaks in your HTML unless in a text-specific tag, like `<p>` or `<span>`. The tags control spacing, not the spaces you type.

**Q: Can I have multiple `<h1>` tags?**
A: Technically yes, but best practice is to use **only one `<h1>` per page** as your main title.

**Q: How do I add comments in HTML?**
A: Use `<!-- comment here -->` - the browser will ignore anything between `<!--` and `-->`.

---
