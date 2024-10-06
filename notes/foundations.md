# HTML

### Lesson 1:
- HTML Hypertext Markup Language will allow you to add different elements to the webpage and strucutre them.
- CSS  Cascading Style Sheet will allow you to improve the structure and elements look that were added with HTML
- JS Javascript will allow you to manipulate the webpage, including its HTML and CSS and add interactivity to it.
> 10/10 no reviews needed; no additional resources needed



### Lesson 2:
We will learn the difference between HTML tags and elements and how each work:
- **Tags:** each HTML element has an opening tag `<>` and a closing tag `</>` seperated by a keyword signifying the nature of the element: paragraph, heading, etc. 
- **Elements:** Using the right tags which would translate into the right elements by the browser is crucial vis a vis Search Engine Optimization and Accessibility and Looks.
Some elements don't wrap any content in between them so they don't have a closing tag: `<br>`, `<img>` 
<br>Historically, they self closed and still but don't need to as per newer HTML version, like this: `<img />` and `<br />` are discouraged.
> 9/10 look at: 
[Mozilla HTML elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)



### Lesson 3:
We will learn the HTML boilerplate that is needed to get started and what each line means:
- `<!DOCTYPE html>` is a declaration that this document is an HTML in version 5; other version have compicated declarations.
- `<html> </html>` is an HTML tag that goes in every HTML document and will be important when we are manipulating HTML with JS. It has many associated *__attributes__* like: `lang = "en"` that go like this `<html lang = "en">CONTENT</html>` this lang tag helps Accessibility. This will be the root of the document and any other element will descend from it.
- `<head> </head>` is an important HTML element that tells the browser how to treat the document. `<meta charset="UTF-8">` is part of the head and `<title> TITLE </title>` were it not included the browser would default to file name as title for the tab.  You should NOT and NEVER put any content or elements that appear inside the head element.
- `<body> </body>` this is the final boiler plate HTML element to complete the file. 
- **Full HTML Boilderplate Code:** 
```html
<DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title> TITLE </title>
    </head>
    <body>
        <h1>FIRST HEADING</h1>
    </body>
</html>
```
- This folowing meta is concerned with responsive design that we'll be covered in advanced curriculum
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
>9/10 needs more boilerplate practice


### Lesson 4:
- **Paragraphs and Headings and Emphasis and Bold:** A chunck of text followed by a line and another chunck will be treated as a single space between them that 's why we need a paragraph element to wrap our paragraphs within. `<strong> to make text strong </strong>` makes it have an importance to Accesibility tools. `<em> Emphasis of text</em>` which acts same as strong for Accessibilty. `<i></i>` and `<b></b>` are also for bold and italics: they do as intended but don't give any significance to Accessibility.
```html
<body>
    <p>This a test paragraph and will be used to check what's going to be check. And having done what's been done is what is going to occur. The termination of the hermination of the Klausian integration.</p>
    <p>Another paragprah that discusses how the Klausian Integration is achieved. Not only achiving this is what being striven but also it's efficiency.</p>
</body>
```
- **Nesting; Parents and Childrens:** All html elements are children or nested from `html` and the hierarchy continues like this; this is significant when manipulating these elements with CSS. This also gives a visual aid to know which element stems from which when editing the code. Elements at same level in hierarchy are siblings. 
```html
<body>
    <p>
        <strong>
                <!-- HTML and Markdown comments can be enclosed between this tiring thing to write; can be written with shortcut on VSCODE.-->
        </strong>
    </p>
</body>
```
>10/10

### Lesson 5
- **Unordered and Ordered Lists:**
```html
<!DOCTYPE html>
<html lang = "en">
    <head>
        <meta charset = "utf-8">
        <meta name = "viewport" content = "width = device-width, initial-scale = 1.0">
        <title>Title of the Page</title>
    </head>
    <body>
        <h2>Unordered List</h2>
        <ul>
            <li>Apple</li>
            <li>Orange</li>
            <li>Mango</li>
        </ul>
        <h2>Ordered List</h2>
        <ol>
            <li>finish HTML unit in TOP</li>
            <li>do undone exercises of 42 pool</li>
            <li>read and implement some DSA</li>
        </ol>
    </body>
</html>
```
> 10/10



### Lesson 6
- **Links: Absolute and Relative:** Absolute links are made of a protocol and a domain and a path; relative links are made of a path(directory) to a page in your website. To link to a page as well as other things, we use an anchor tag, which has many attributes such as href, target, rel etc.
```html
<a href="https://www.absolute.com/link">Name Given to Link</a>
<a href="./pages/about.html">Relative Link</a>
<a href="https://website.com/page" target="_blan" rel="noopener noreferrer">Safe Links that reveal no oepner and phising proof</a>
``` 
- **Images:** Images can be added to html page with nearly same syntax as links with minor difference in that `<img>` is a void tag that self closes, and the source image is linked to with `src="absolute link or directory relative link"`
- It is always advised to have a height and width *__attributes:have three parts a name and a value that give more information about the html element, goes always with the openeing tag__* of the image added in the html even if they are handled with CSS.
```html
<img src="relative or absolute links" alt="alt text" height="100" width="100">
```
- Types of Images: Working with multiple pages linked together and containing multiple images each requires high orgnization. 
- JPG: handle large color palettes and lots of gradients while taking smaller sizes than their counterparts PNG, but don't allow for transparent pixels.  Good for photos.
- PNG: As good as JPG in handling colors but takes more size for similar quality image with a JPG. Good for Diagrams and Icons. 
- GIF: Good for animations and are never used for photos as they are color-lacking. 
- SVG: Fancy and awesome; vector-based graphics?! Should be used whenever you can.
> 7/10 need more practice and learn more abotu security: [Privacy](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a#security_and_privacy) and [Phishing](https://www.ibm.com/topics/phishing) and [Tabnabbing](https://owasp.org/www-community/attacks/Reverse_Tabnabbing) ; [Good blog for more info](https://internetingishard.netlify.app/html-and-css/links-and-images/#image-formats)

### Lesson 7
*__Git Commit Messages__*
- Commits come with a subject and description that should be written explaining the reason for the commit clearly; allowing others working on large project to understand. 
- Commits serve also as memories for future selves to remind us of things we are destined to forget as time passes working on large projects.
- Commits should happen at milestones in the project progress and will allow for backtracking as needed when things break down.