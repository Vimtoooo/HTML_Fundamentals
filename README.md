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

## Text and Formatting:

### Headings:

You are probably not going to use only plain text into your website, right? 
If you would like to add a title or a section name, the best way is to utilize **headings**. Note that there are **six levels of headings**, from `<h1>` (the most important) to `<h6>` (the least important). Here is an example of usage:

```html
<h1>This is a main heading</h1>
<h2>This is a subheading</h2>
<h3>This is a sub-subheading</h3>
```

#### Purpose of Headings:

Headings help **organize your content** and make it easier for people or users to **search engines to understand your page**.

* `<h1>`: Represents the main title of the webpage (the most important);
* `<h2>`: Subheading;
* `<h3>`: Sub-subheading;
* `<h4>` and `<h5>`: Other sub-sub-headings;
* `<h6>`: The least important heading.

With all these headings, you can construct something that looks similar to this:

```html
<h1>Welcome to My Website</h1>
<h2>About Me</h2>
<h3>My Hobbies</h3>
<h4>Reading</h4>
<h5>Fiction</h5>
<h6>Favorite Authors</h6>
```

#### How to use Headings Well:

- Use only **one `<h1>` per page** for the main title;
- Use headings to create a **logical structure**, you can think of them as an outline;
- **Never skip heading levels**, for example: Don't jump from `<h1>` to `<h4>`;
- Use headings for structure, not for styling, because **CSS** will take over that part and will prioritize for appearance;
- Headings help with accessibility and SEO (Search Engine Optimization), they make your content easier to navigate for users and search engines.

##### Example of Good Heading Structure:

```html
<h1>HTML Fundamentals</h1>
<h2>Introduction</h2>
<h2>HTML Basics</h2>
  <h3>Elements and Tags</h3>
  <h3>Nesting</h3>
<h2>Formatting Text</h2>
```

#### Summary:

Use headings to organize your content clearly, making it easy for both people and search engines to **understand your page's structure**. Always start with `<h1>` (once per page!), then use `<h2>`, `<h3>` and etc... as needed for subsections.

### Paragraphs:

In HTML, paragraphs are used to **show blocks of text**, where you would define them inside the `<p>` and `</p>` tags. Note that when you put text between the `<p>` and `</p>` tags, the browser will display it as a separate paragraph with some space above and below it. Here is how you can add a paragraph in HTML:

```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

> [!NOTE]
> If you are creating an article, the **title** would be a heading `<h1>`, and the **actual text** would be the paragraph `<p>`.

#### Example of a Paragraph:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>Welcome to our pizza restaurant!</p>
        <p>Explore our menu today.</p>
    </body>
</html>
```

#### Combining Headings with Paragraphs:

```html
<!DOCTYPE html>
<html>
    <body>
        <p>
            <h1>Welcome to My Website</h1>
            <h2>About Me</h2>
            <p>My name is Vimto, and I code for living</p>
        </p>
    </body>
</html>
```

