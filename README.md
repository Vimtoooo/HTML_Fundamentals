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

### Nesting and Closing Tags:

In HTML, nesting means placing an element inside another. For example, you can put the `<strong>` tag inside the `<p>` tag to make the text bald within a paragraph.
Here is how it looks:

```html
<p>This is <strong>bold</strong> text.</p>
```

**Closing tags are crucial**, it is mandatory that every start tag must implement an end tag, rementioning that the end tag has a **/** bar at the beginning of a keyword (left-side). This can be seen in the above code, the `<p>` is the start, we have the content inside between the start and end tags, and the `</p>` represents the end tag.

#### Issues with Incorrect Nesting:

Incorrect nesting can lead to rendering issues, so make sure to always close tags in the correct order. The inner tag should be closed before the outer tag.

##### Correct Nesting:

```html
<p>This is <strong>bold</strong> text.</p>
```

##### Incorrect Nesting:

```html
<p>This is <strong>bold text.</p></strong>
```

### Comments:

Comments are a feature used commonly for documenting parts in your code, but they are mainly known as **notes that don't appear in your program or web page**. They are useful for:

- Explaining complex code;
- Leaving notes for other or yourself;
- Temporarily disabling code.

#### Syntax:

In HTML, comments are written between `<!--` and `-->`.

```html
<!-- This is a comment -->
<p>This is a paragraph.</p>
```

#### Disabling Content:

You can also use comments to not exhibit content or disable functioning code in your html document.

```html
<!DOCTYPE html>
<html>
    <body>
        <p>
            <!--Hello <strong>boys</strong>!-->
        </p>
    </body>
</html>
```