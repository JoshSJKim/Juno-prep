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

