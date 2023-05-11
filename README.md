# Juno-prep

- Going through the Juno web-development bootcamp prep.

## Intro to the Internet

### What is a website?

- Website is a collection files and folders that live on a server.
- Visitors can view these files on an internet browser by entering the associated URL (website address) where the files are stored.
- Requested files are pulled through the network and displayed on the browser window.

- Websites are built on three primary languages: HTML, CSS, and JavaScript.
  - HTML (Hyper Text Markup Language): The content (words, images, etc.)
  - CSS (Cascading StyleSheets): Design, color, size, position, layout, etc.
  - JavaScript (JS): User interaction, functional aspect.

### What happens when you visit a webpage?

- URL is typed into the search input field.
- Browser checks history if the site has been visited in the past.
- Once received, the browser pulls up the files for display on the browser window.

### What is the Internet?

- "Physical infrastructure of connected devices that deliver information from one device to another using wires (electricity), cables (light with fiber optics), and/or radio transmitters (sound waves - WiFi)."

- Each device has an IP (internet protocol) address (like a phone number, or street address).
- One device asks for some information from another device by visiting a website.
  - The requesting device lets the providing device know where to send the requested information.

- IP addresses are difficult to remember.
- So we use DNS (Domain Name System) to match URL (Uniform Resource Location) with the specific IP address.

### What is a web browser?

- "An application where users can see and interact with a web resource."
- Best to choose evergreen browsers, which means that the browser is updated frequently, and automatically in the background, without any user action required.

### The Role of a Web Developer

- Front end web developers write code for web browsers to read.
- It is crucial to learn how to communicate with browsers.
  - Since browsers are subject to change frequently, it is the web developer's responsibility to respond to those changes.

---

## Keeping Organized as a Developer

### Naming Files and Project Folders

- Developers deal with many projects, and each project has many files and folders, of which many have the same name (ex. index.html).
- It is crucial to maintain an organized file system since these files and folders will be shared with other developers as well.

#### No Spaces

- Folder names shall not have spaces. It'll only cause problems down the line.
- Use `camelCase`, `kebab-case`, or `underscore_case`
- Whatever you use, consistency is key.
- It is important to communicate with other developers to maintain consistency.

### Development Workspace

- Working on multiple projects can get out of control without proper management.
- Each project will have `index.html` (note that there should be only one of these for every project), and folders named `styles` and `scripts`.

- Create `sites` or `websites` at the root user folder of your computer.
- Organize the folders for projects of different categories.
- Apply a numbering system that represent project ID or dates.
- Organize in a manner that is scalable and makes sense to you

- DO NOT save your folders on a cloud drive. Make sure it is saved on the local drive.

- Lastly, close the files that you are not working on.
- Practice `tab minimalism` across text editors and browsers.

---

## Intro to HTML

- Hyper Text Markup Language
- Standard language used to create web pages.
- When HTML file is opened in a browser, the code is interpreted visually or audibly.

- Think of HTML as the framework of a building.
- It creates the structure of the content.
- The design aspect is a whole other game (CSS).

### Base HTML Structure

- All websites require a base structure, or a 'skeleton'.

- Current standard is shown below.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equv="X_US_Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title> Title will not show on the browser page, but on the tab </title>
  <link rel="stylesheet" href="styles.css"> 
  <!-- This hasn't been covered yet, but it is a link to a separate CSS file -->
</head>
<body>
  <h1> The Content </h1>
  <p> May include images, text, forms for submission, etc.</p>
</body>
</html>
```

- The base structure, or `boilerplate` can be added in code editors, such as vscode, by entering `!` and `tab` on an `html` template.
- It is an easy shortcut, but all developers should be familiar with the base structure.

  - `<!DOCTYPE html>`: Indicates to the browser that the file is written in HTML5 (latest version). Must be included at the very head of every HTML document.
  - `<html lang="en"></html>`: All contents of the html code are 'nested' in the `<html>` element. It also specifies the language with the `lang` attribute.
  - `<head></head>`: The `head` element does not appear on the browser. It specifies the site information to the browser.
  - `<meta>`: These tags provide specific information about the website. Notice that it is a `self-closing` tag.
  - `<title></title>`: Short title of the website that will appear on the tab of the browser page.
  - `<body></body>`: Everything visible on the website will be 'nested' in the body element.

### HTML Syntax

- Set of rules that make up a language.
- The rules must be followed in order for the language to make sense for interaction.

- HTML is made up of `elements` that describe content.
- Elements are created by wrapping the contents in `tags`.
- Elements typically have an opening and a closing tag.
- The content wrapped inside the tags will be displayed on the browser page.
- There are also `self-closing` tags that do not require a closing tag.

### Creating Elements

`<h1>Hello World!</h1>`

- Opening tag contains the name (or type) of the element.
- Anything that comes after the opening tag is the content.
- The closing tag must correspond with the type of the opening tag with an added 'forward slash'.

- Element: Structural component of a website that describes and contains content
- Tag: The opening and closing portion of element that wraps the content

### Separation of Content and Style

Very Important!

- When elements are added to the page and the code is rendered on the browser page, there is basic default styling that is applied by the browser itself.
- Marking up content with proper elements help describe the content for the browser and assistive technologies (AT).
- Without proper markup, the page may have visual styling effect, but it would have no meaning for Assistive Technologies and Search Engine Optimization (SEO).
- We use HTML tags to provide further description of the content for assistive technologies.
- Visual stylization in general is done through CSS.

### Nesting Elements

- Nesting is an important concept in coding because it represents a parent-child relationship between elements.
- When nesting elements, it must always be closed in reverse order that was opened. Otherwise, the page may not load properly.

### Indentation

- When nesting, it is best practice to apply proper indentation to show structure and improve readability.
- Some exceptions apply to `inline` elements, such as `<span>`, `<em>`, etc.

### HTML Comments

- Commenting is a handy tool to stay organized while coding.
- It is also used to make notes, either for personal use, or to provide instructions or information for other developers viewing the code.
- Remember, comments will not be rendered on the browser page.

- `<!-- comment here -->` is the commenting syntax for HTML.
- Use `command` + `/` for shortcut

### Attributes

- Add attributes to HTML elements for more robust and dynamic use.
- Attributes are added to the opening tag of an element to define class, id, type, value, etc.

---

## HTML Elements

### Typographic Elements

#### Headings

- Use `heading` as the main title of a page.
- Headings have opening and closing tags
- `<h1></h1> ... <h6></h6>`
- There may only be one `<h1>` element per HTML page.
- Sub-headings may use `<h2>` and so forth for content division.
- Appearance and styling can be changed with CSS
- Note that Assistive Technologies highly depend on hierarchy. Skipping headings can cause problems.
- You may not skip heading sequence (ex. <h1>...<h3>).

#### Paragraphs

- use `<p></p>` to define a paragraph of text.
- `Paragraphs` have opening and closing tags.
- `inline` elements, such as `<span>`, `<em>`, `<strong>` may be used in the `paragraph` element.

#### Anchor Elements

- `Anchor` elements are used to create `links` to other web pages or specific places within the same website.
- It is an inline element and requires opening and closing tags.
- Anchor elements require an `href` attribute that tells the link where to go when clicked.
- The text wrapped with the `<a></a>` tags will serve as the link on the webpage.
  
##### Linking Externally

```html
<div>
  <p>For more information, contact us at <a href="https://www.junocollege.com/contact">Juno College</a>.</p>
</div>
```

- The above code will provide a hypertext link to the external website specified in the `href`, where the text 'Juno College' will serve as the link.

##### Linking Internally

- You may have a multi-page website.
- A link to an internal page is called a relative link.
- Ensure that all html files are saved in the same folder. (ex. index.html and about.html in a folder called 'myWebsite')

```html
<a href="about.html">About</a>
```

- The above code may be used for a link to a separate personal bio page.
- This code would be written in the `index.html` file.

- It is best practice to name the main html file `index.html`.
- It is the industry standard, and it is also the name that servers will look for by default.

##### Opening Links in a New Window

- Without specifying, the links above will open in the current window.
- In order to open the link in a new tab or a new window automatically, use the `target` attribute and set its value to `_blank`.

```html
<a href="https://www.google.com" target="_blank">Google.com</a>
```



