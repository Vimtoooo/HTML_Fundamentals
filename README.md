# HTML Fundamentals

HTML stands for **HyperText Markup Language**, which is the standard coding language used to create and structure content for the web (such as HTTP AND HTTPS), acting as a fundamental building block of all web pages by defining elements like headings, paragraphs, links and images using tags that web browsers interpret to display information. But it is key to remember, that HTML is **not a programming language, but a markup language**, meaning that it annotates text to define how it's structured and displayed.
HTML is also a **Static language**, where it does not inherently provide interactive features, but can be combined with `CSS` for styling and `JavaScript` for interactivity.

## HTML Basics and Structure:

### The Basic Structure of an HTML:

Every HTML document follows a simple structure:

#### The `<!DOCTYPE html>`:

At the very top (line 1), it starts with `<!DOCTYPE html>`, telling us **which version of HTML** that we are using. This will be then, followed by the `<html>` tag, containing **all of the HTML content**.

#### `<HTML>`:

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

#### Example of Usage:

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

### Line Breaks:

In HTML, the `<br>` tag is used to create a **line break**, which can be useful when you want to start text on a new line without having to start another paragraph. Unlike the `<p>` tag, which adds a blank line before and after the text, the `<br>` tag simply moves the text to the next line.
Here's how you can use the `<br>` tag in HTML:

#### Example of Usage:

```html
<p>This is a line.<br>This is another line.</p>
```

When using the `<br>` tag, you won't necessarily use the end tag for the `<br>` line breaker tag since we just want to move one part of the text to the next line...

On the example above, "This is a line." will be displayed above "This is another line.", successfully separating the text in half and displaying the text in separate lines. The `<br>` tag is an **empty element**, which means that it **doesn't have an end tag**. So you would just simply write the `<br>` tag where you want the line break to occur.

### Bold and Italic Text:

In HTML, you can style text easily!

* Make it bold with the `<strong>` tag;
* Make it italic with `<em>`.

These tags help emphasize important words and making them stand out!

#### Example of Usage:

```html
<p>This is normal text</p>
<p>This is <strong>bold</strong> text</p>
<p>This is <em>italic</em> text</p>
```

In the example above, the word "bold" will be displayed in bold, while the "italic" word will be displayed in italics.

#### Other Bold and Italic Tags:

There are another two different tags that can be used to make your text bold or in italics:

- `<b>`: Bold;
- `<i>`: Italic.

Here is an example:

```html
<p>This is normal text. <b>This is bold text</b>. <i>This is italic text</i>.</p>
```

### Recap - Text Formatting:

* **Headings**: Use `<h1>` up to `<h6>` tags to create headings with different levels (most to least important);
* **Paragraphs**: Use `<p>` and `</p>` to construct paragraphs, where browsers automatically generate a space above and below each paragraph;
* **Line Breakers**: Use `<br>` when needing to separate text into other sections;
* **Bold and Italic**: Use `<strong>` and `</strong>` (or `<b>`) for making text bold, and `<em>` or `<i>` for italics!

Here is an example that combines all of the mentioned tags:

```html
<h1>Main Heading</h1>
<p>This is a <strong>bold</strong> paragraph. Here is a line break:<br>This is <em>italic</em> text.</p>
```

In this example, we have a main heading, a paragraph with bold and italic text, and a line break within the paragraph. This demonstrates how to use different formatting tags together to create well-structured and styled content.

## Working with Lists:

### Unordered List:

In HTML, an **unordered list** is a list of items that are **not ordered by numbers or letters**. Instead, each item is marked with a **bullet point**. To create an unordered list, you would use the `<ul>` and the `</ul>` tags (marks the structure). Each item in the list is defined using the `<li>` and `</li>` tags (they would represent the bullet points).

> [!NOTE]
> Remember, `<ul>` stands for **Unordered List** and the `<li>` stands for a **list item**!
> If you don't remember what tags or elements to use, always be aware of the letters within the elements and tags.

#### Example of Usage:

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

In this example, the `<ul>` tag defines the unordered list, and each `<li>` tag represents a list item. When displayed in a browser, this code will create a list with bullet points:

```
* Item 1
* Item 2
* Item 3
```

#### Why use Unordered Lists?

Unordered lists are useful when presenting items that do not consist of **any order**, such as a list of ingredients or features.

### Ordered Lists:

Now an **ordered list** is a list of items that are ordered by numbers or letters. To create an ordered list, you would use the `<ol>` and `</ol>` tags, and each element in the list is defined using the `<li>` and `</li>` tags (similar to the unordered list).

The `<ol>` tag stands for **Ordered List**.

#### Example of Usage:

```html
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

In this example, the `<ol>` tag defines the ordered list, and each `<li>` tag represents a list item. When displayed in a browser, this code will create a numbered list:

```
1. First item
2. Second item
3. Third item
```

#### Why use Ordered Lists?

Ordered lists are useful for presenting items where the **order matters**, such as steps in a procedure or a list of ranked items.

### Nested Lists:

Did you know that you can place **one list inside another?** 
This feature is so called **nested lists**, this can be useful for creating hierarchical structures, such as outliers or multi-level menus. 

#### Creating a Nested List:

Now, to create a nested list, you simply add the `<ul>` or the `<ol>` element inside the outer `<i>`, `<li>` or `</i>` element of another list. Here's an example of a nested unordered list:

```html
<ul> <!-- This tag will be the outer list -->
  <li>Item 1</li>
  <li>Item 2
    <ul> <!-- This would be the inner list -->
      <li>Subitem 2.1</li>
      <li>Subitem 2.2</li>
    </ul>
  </li> <!-- When nesting, always have an end tag for legible and efficient nesting -->
  <li>Item 3</li>
</ul>
```

> [!NOTE]
> The second item `Item 2` contains a nested list of two subitems: `Subitem 2.1` and `Subitem 2.2`.

In the browser, it will look similar to this:

```html
* Item 1
* Item 2
    - Subitem 2.1
    - Subitem 2.2
* Item 3
```

You can also nest ordered lists or mix them up!

### Recap - Lists:

* **Unordered Lists `<ul>`:** Use `<ul>` and `</ul>` for creating an unordered list (with bullet points), each item is defined using the **item list tags `<li>` and `</li>`**;
* **Ordered Lists `<ol>`:** Use `<ol>` and `</ol>` for creating a numbered list, where each item is also defined with `<li>`;
* **Nested Lists:** Place one list inside another by putting either the `<ul>` or `<ol>` inside the inner `<li>` tag of another list, then use any of the lists as mentioned!

Here is an example of all of the lists being used in a webpage: A Todo List

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>My Todo List</h1>
    <ol>
      <li>Morning
        <ul>
          <li>Wake up at 5:00 AM</li>
          <li>Brush my teeth</li>
          <li>Read a book of choice</li>
        </ul>
      </li>
      <li>Afternoon
        <ul>
          <li>Touch some grass</li>
          <li>Do my homework</li>
          <li>Go to the gym</li>
        </ul>
      </li>
      <li>Evening
        <ul>
          <li>Stretch</li>
          <li>Play games</li>
          <li>Sleep</li>
        </ul>
      </li>
    </ol>
  </body>
</html>
```

## Adding Content:

### HTML Attributes:

In HTML, **attributes** provide additional information about elements. They are used to define properties of an element, such as its size, color or behavior. Attributes are always specified in the start tag and usually come in `name/value` pairs like `name=value`.

#### General Syntax:

Here is a general syntax for adding attributes into an HTML element:

```html
<tagname attribute1="value1" attribute2="value2">Content</tagname>
```

- `tagname`: Name of the HTML element, for example: (`<p>`, `<strong>`, `<h3>`);
- `attribute1` and `attribute2`: Names of the attributes;
- `value1` and `value2`: The values assigned to those attributes.

### Links:

In HTML, a **link** (or a hyperlink) is an element that connects **one webpage to another**. 

You can create links to other webpages, files, locations within the same page or any other URL. Links are create using the `<a>` tag. The `<a>` tag stands for **anchor**.

#### Basic Syntax:

Here is the basic syntax for making links in HTML:

```html
<a href="url">Link text</a>
```

- `<a>`: The opening anchor tag;
- `href`: The destination URL of the link;
- `Link text`: The visible text that users will see and click on;
- `</a>`: The closing anchor tag.

#### Link to Google's Homepage:

```html
<a href="https://www.google.com">Visit Google</a>
```

In this example, when a user clicks on the text "Visit Google", they will be taken to `https://www.google.com`.

#### Multiple Links:

##### Links Next to Each Other:

```html
<!DOCTYPE html>
<html>
  <body>
    <a href="https://coddy.tech">Visit Coddy </a>
    <a href="https://www.google.com">Visit Google</a>
  </body>
</html>
```

##### Separate Links:

```html
<!DOCTYPE html>
<html>
  <body>
    <p>
      <a href="https://coddy.tech">Visit Coddy </a>
    </p>
    <p>
      <a href="https://www.google.com">Visit Google</a>
    </p>
  </body>
</html>
```

### New Page Links:

You can also create links that open on a **new tab or window** by using the `target` attribute with the value `_blank`:

#### Basic Syntax:

```html
<a href="https://www.example.com" target="_blank">Visit Example</a>
```

> [!NOTE]
> This will open the link in a new tab or window, but this will depend on the user's browser settings!

### Images:

Images can make your webpages more engaging, and adding them into HTML is simple! Use the `<img>` tag for inserting images with ease. The `<img>` tag is self-closing, so it does not require an end tag.

#### How to Insert an Image:

To insert an image, use the `src` attribute to specify the image's location (can be made by either referring the URL or file path location). Here's an example:

##### Insertion Via URL:

```html
<img src="https://coddy.tech/images/bit.svg" />
```

In this example, the browser will load up and display the image from the URL `https://coddy.tech/images/bit.svg`.

##### Insertion Via File Path:

```html
<img src="C:\Users\leone\OneDrive\Imagens\Screenshots£>" />
```

Or if the image is in the same folder as your HTML file:

```html
<img src="myImage.jpg" alt="A description of my image">
```

### Image Attributes:

Here are some additional image attributes to improve your image manipulation and exhibition:

#### `alt`:

The **`alt`** attribute provides alternative text if the image doesn't load, for example:

```html
<img src="img.jpg" alt="Message that pops if image has not loaded" />
```

#### `width` and `height`:

These two attributes control the size and height of an image in pixels.

```html
<img src="img.jpg" width="800" height="600" />
```

And if you combine these features, you should get something like this:

```html
<img src="img.jpg" alt="A scenic view of mountains" width="600" height="400" />
```

This would set the image source, provide a brief description, and sizes of 600x400 pixels. Always include an `alt` for accessibility and dimensions to maintain design consistency.

## Page Layout:

### Divisions:

Imagine that you would like to split you webpage into segmented blocks to organize your content. In HTML, you can use the `<div>` to group elements together. 
The `<div>` (division) tags are handy for creating layouts and separating sections. Here's the basic syntax:

#### Basic Syntax:

```html
<div>
    <!-- Content goes here -->
</div>
```

> [!NOTE]
> You can add other HTML elements inside a `<div>` tag, such as paragraphs, headings, images, and even nest other `<div>` elements!

#### Example of Usage:

Here, the `<div>` is being used to construct a simple layout with a header, main content area and a footer.

```html
<div>
    <h1>Header</h1>
</div>
<div>
    <p>Main content goes here.</p>
</div>
<div>
    <p>Footer</p>
</div>
```

### Inline Spans:

Imagine that you have a sentence and you wish to highlight one word or a small part of it, what would you do to handle this case? Use a `<span>` tag? Well the answer is crystal clear!

We can use the `<span>` tag to apply styles or make changes to only a specific part of a text without affecting the rest. 

#### Basic Syntax:

```html
<span>This is some text.</span>
```

#### Highlighting a Portion of Text:

```html
<p>
  This is a <span style="color:blue;">blue</span> word.
</p>
```

The `style` attribute within the `<span>` tag is applying a blue paint in the "blue" word, and the rest of the sentence remains the same color!
This is just an introduction to style attributes, we will learn them next lesson!

### Semantic Tags:

The **semantic tags** in HTML help define the meaning of content, making the code clearer for both developers and browsers. Unlike `<div>` and `<span>`, they give context to the enclosed content.

#### Common Semantic Tags:

* `<header>`: Introductory content, usually at the top;
* `<nav>`: Contains navigation links;
* `<main>`: Main content of the page;
* `<article>`: A self-contained piece like a blog post;
* `<section>`: Groups related content, often with a heading;
* `<footer>`: Bottom section with info like copyright or contact details.

#### Example of Usage:

```html
<header>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
</header>
<main>
    <article>
        <h2>Article Title</h2>
        <p>Article content goes here.</p>
    </article>
</main>
<footer>
    <p>Copyright 2023</p>
</footer>
```

This structure provides a clear and meaningful layout for the content.

### Sections and Articles:

The `<section>` and `<article>` tags are used to **organize content into logical parts**.

#### `<section>`: 

The `<section>` tag defines a section in a document, such as chapters, headers, footers and any other sections of the document. This can be seen as a way to group content together, for example, you might use `<section>` to divide a page into an introduction, content and contact information. Here is how to use `<section>`:

```html
<section>
    <h2>Section Heading</h2>
    <p>Section content goes here.</p>
</section>
```

#### `<article>`:

In the other hand, the `<article>` tag specifies independent, self-contained content. I should make sense on its own and also possible to read it independently from the rest of the website. Examples of where an `<article>` element should be used: In a forum post, a blog entry, a news story or a comment. Here you can see the `<article>` tag being utilized:

```html
<article>
    <h2>Article Title</h2>
    <p>Article content goes here.</p>
</article>
```

