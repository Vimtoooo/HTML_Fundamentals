# HTML Fundamentals

HTML stands for **HyperText Markup Language**, which is the standard coding language used to create and structure content for the web (such as HTTP AND HTTPS), acting as a fundamental building block of all web pages by defining elements like headings, paragraphs, links and images using tags that web browsers interpret to display information. But it is key to remember, that HTML is **not a programming language, but a markup language**, meaning that it annotates text to define how it's structured and displayed.
HTML is also a **Static language**, where it does not inherently provide interactive features, but can be combined with `CSS` for styling and `JavaScript` for interactivity.

## HTML Basics and Structure:

### The Basic Structure of an HTML:

Every HTML document follows a simple structure:

#### <!DOCTYPE html>:

At the very top (line 1), it starts with `<!DOCTYPE html>`, telling us **which version of HTML** that we are using. This will be then, followed by the `<html>` tag, containing **all of the HTML content**.

#### <HTML>:

Inside the `<html>` tag, we add the `<body>` tag, which holds all of the visible content of the web page. Here is a simple example:

```html
<!DOCTYPE html>
<html>
    <body>
        This is some text.
    </body>
</html>
```

From the above example, you are given the base code of an HTML page, and inside the `<body>` tag, there is a text, which will be displayed on the webpage as content.

### Elements and Tags:

In HTML, the **tags** are represented as **keywords enclosed in angle brackets**, like the simple `<html>`. They tell the browser how to display the content. The **elements** are the **components of an HTML document**, consisting of a start tag, content and an end tag. Here's a simple breakdown:

#### Tags:

```html
<html> <!-- Singular tag for representation -->
```

This singular `<html>` tag is just a keyword within double angle brackets that define how content is displayed.

#### Elements:

```html
<html>
    <body>
        <!-- These would be considered as elements, with opening and closing tags! -->
    </body>
</html>
```

In the other hand, the elements are components made up of a start tag, content inside that block for that tag, and an end tag, which can be identified with the `</body>` syntax ("/").

```html
<p>This is a paragraph.</p>
```

For that example, the `<p>` is the start tag, "This is a paragraph." is the content, and the `</p>` is the end tag. Together, they form a paragraph element!
