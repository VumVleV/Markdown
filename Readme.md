<!DOCTYPE html>
<html>
<head>
    <style>
        r {
            color: red;
        }
        y {
            background-color: yellow;
        }
    </style>
</head>


# 1. <y>Header</y>
- <b>Number Signs</b>(<r>#</r>)
- More Signs, Smaller the Header.
  
|Markdown|HTML|Alternate Syntax|Output|
| --- | --- | --- | --- |
|# Heading level 1|\<h1>Heading level 1</h1>|Heading level 1<br>============|<h1>Heading level 1</h1>|
|## Heading level 2|\<h2>Heading level 1</h2>|Heading level 2<br>---------------------|<h2>Heading level 1</h2>|
|### Heading level 3|\<h3>Heading level 1</h3>||<h3>Heading level 1</h3>|
|#### Heading level 4|\<h4>Heading level 1</h4>||<h4>Heading level 1</h4>|
|##### Heading level 5|\<h5>Heading level 1</h5>||<h5>Heading level 1</h5>|

|✅ Do this|❌ Don't do this|
|---|---|
|# Here's a Heading|#Here's a Heading|
|Try to put a blank line before...<br><br># Heading<br><br>...and after a heading.|Without blank lines, this might not look right.<br># Heading<br>Don't do this!|

# 2. <y>Paragraphs</y>
To create paragraphs, use a blank line to separate one or more lines of text.

|Markdown|HTML|Output|
|---|---|---|
|I really like using Markdown.<br><br>I think I'll use it to format<br>all of my documents from now on.|\<p>I really like using Markdown.\</p>\<br><br>\<p>I think I'll use it to format all of my documents from now on.\</p>|I really like using Markdown.<br><br>I think I'll use it to format<br>all of my documents from now on.|

To create a line break or new line, end a line with two or more spaces, and then type return.


|✅ Do this|❌ Don't do this|
|---|---|
|Don't put tabs or spaces in front of your paragraphs.<br><br>Keep lines left-aligned like this.|&nbsp;&nbsp;&nbsp;&nbsp; This can result in unexpected formatting problems.<br><br>&nbsp;Don't add tabs or spaces in front of paragraphs.|

To create a line break or new line (\<br>), end a line with two or more spaces, and then type return.

|Markdown|HTML|Output|
|---|---|---|
|This is the first line.  <br>And this is the second line.|\<p>This is the first line.\<br><br>And this is the second line.\</p>|This is the first line.  <br>And this is the second line.|

You can use two or more spaces (commonly referred to as “trailing whitespace”) for line breaks in nearly every Markdown application, but it’s controversial.
There are two other options I don’t recommend using. CommonMark and a few other lightweight markup languages let you type a backslash (\) at the end of the line, but not all Markdown applications support this, so it isn’t a great option from a compatibility perspective. And at least a couple lightweight markup languages don’t require anything at the end of the line — just type return and they’ll create a line break.

|✅ Do this|❌ Don't do this|
|---|---|
|Trailing whitespace<br>\<br> HTML tag|backslash(\\)<br>just return|

# 3. <y>Empahsis</y>
To bold texts, add two asterisks or underscore before and after a word or phrase. To bold the middle of a word, add two asterisks without spaces around the letters.

|Markdown|HTML|Output|
|---|---|---|
|I just love \*\*bold text\*\*.|I just love \<strong>bold text\</strong>.|I just love <strong>bold text</strong>.|
|I just love \_\_bold text\_\_.|I just love \<strong>bold text\</strong>.|I just love <strong>bold text</strong>.|
|Love\*\*is\*\*bold|Love\<strong>is\</strong>bold|Love**is**bold|

|✅ Do this|❌ Don't do this|
|---|---|
|Love\*\*is\*\*bold|Love\_\_is\_\_bold|

To italicize text, add one asterisk or underscore before and after a word or phrase. To italicize the middle of a word, add one asterisk without space around the letters.

|Markdown|HTML|Output|
|---|---|---|
|Italicized text is the \*cat's meow\*.|Italicized text is the \<em>cat's meow\</em>.|Italicized text is the <em>cat's meow</em>.|
|Italicized text is the \_cat's meow\_.|Italicized text is the \<em>cat's meow\</em>.|Italicized text is the <em>cat's meow</em>.|
|A\*cat\*meow|A\<em>cat\</em>meow|A*cat*meow	|

|✅ Do this|❌ Don't do this|
|---|---|
|Love\*is\*bold|Love\_is\_bold|

To bold and italicize texts, add three asterisks or underscores before and after a word or phrase. To bold and italicize the middle of a word, add three asterisks without spaces around the letters.

|Markdown|HTML|Output|
|---|---|---|
|This text is \*\*\*really important\*\*\*.|This text is \<em>\<strong>really important\</strong>\</em>.|This text is <em><strong>really important</strong></em>.|
|This text is \_\_\_really important\_\_\_.|This text is \<em>\<strong>really important\</strong>\</em>.|This text is <em><strong>really important</strong></em>.|
|This text is \_\_\*really important\*\_\_.|This text is \<em>\<strong>really important\</strong>\</em>.|This text is <em><strong>really important</strong></em>.|
|This text is \_\*\*really important\*\*\_.|This text is \<em>\<strong>really important\</strong>\</em>.|This text is <em><strong>really important</strong></em>.|
|This text is really\*\*\*very\*\*\*important.|This text is really\<em>\<strong>very\</strong>\</em>important.|This text is really<em><strong>very</strong></em>important.|

# 4. <y>Blockquotes</y>
To create a blockquote, add a > in front of a paragraph.

\> Once when I was six years old I saw

> Once when I was six years old I saw

Blockquotes can contain multiple paragraphs.

\> Once when I was six years old I saw
\> 
\> a magnificent picture in a book.

> Once when I was six years old I saw
> 
> a magnificent picture in a book.

Blockquotes can be nested. Add a >> in front of the paragraph you want to nest.

\> Once when I was six years old I saw
\>
\>\> a magnificent picture in a book.

> Once when I was six years old I saw
>
>> a magnificent picture in a book.

Blockquots can contain other Markdown formatted elements. Not all elements can be used.

\> #### Welcome to \*\*\*Hogwarts\*\*\*!
\> 
\> - Harry potter
\> - Albert Dumbledore
\> 
\> \*Hogwarts\* is divided into \*\*four houses\*\*.

> #### Welcome to ***Hogwarts***!
> 
> - Harry potter
> - Albert Dumbledore
> 
> *Hogwarts* is divided into **four houses**.

|✅ Do this|❌ Don't do this|
|---|---|
|Try to put a blank line before...<br><br>\> This is a block quote<br><br>... and after a blockquote.|Without blank lines, this might not look right.<br>\>This is a blockquote<br>Don't do this!|

# 5. <y>Lists</y>
## Ordered Lists
To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

|Markdown|HTML|Output|
|---|---|---|
|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|\<ol><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ol>|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|
|1. First item<br>1. Second item<br>1. Third item<br>1. Fourth item|\<ol><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ol>|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|
|1. First item<br>8. Second item<br>3. Third item<br>5. Fourth item|\<ol><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ol>|1. First item<br>2. Second item<br>3. Third item<br>4. Fourth item|
|1. First item<br>2. Second item<br>3. Third item<br>&emsp;1. Indented item<br>&emsp;2. Indented item<br>4. Fourth item|\<ol><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;&emsp;\<ol><br>&emsp;&emsp;&emsp;\<li>Indented item\</li><br>&emsp;&emsp;&emsp;\<li>Indented item\</li><br>&emsp;&emsp;\</ol><br>&emsp;\<li>Fourth item\</li><br>\</ol>|1. First item<br>2. Second item<br>3. Third item<br>&emsp;1. Indented item<br>&emsp;2. Indented item<br>4. Fourth item|

|✅ Do this|❌ Don't do this|
|---|---|
|1. First item<br>2. Second item|1)First item<br>2)Second item|

> CommonMark and a few other lightweight markup languages support parenthesis as a delimiter but not recommended.
> List index and text needs to be delimited by a space.
## Unordered Lists
To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. Indent one or more items to create a nested list.

|Markdown|HTML|Output|
|---|---|---|
|- First item<br>- Second item<br>- Third item<br>- Fourth item|\<ul><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ul>|· First item<br>· Second item<br>· Third item<br>· Fourth item|
|* First item<br>* Second item<br>* Third item<br>* Fourth item|\<ul><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ul>|· First item<br>· Second item<br>· Third item<br>· Fourth item|
|+ First item<br>+ Second item<br>+ Third item<br>+ Fourth item|\<ul><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;\<li>Fourth item\</li><br>\</ul>|· First item<br>· Second item<br>· Third item<br>· Fourth item|
|- First item<br>- Second item<br>- Third item<br>&emsp;- Indented item<br>&emsp;- Indented item<br>- Fourth item|\<ul><br>&emsp;\<li>First item\</li><br>&emsp;\<li>Second item\</li><br>&emsp;\<li>Third item\</li><br>&emsp;&emsp;\<ul><br>&emsp;&emsp;&emsp;\<li>Indented item\</li><br>&emsp;&emsp;&emsp;\<li>Indented item\</li><br>&emsp;&emsp;\</ul><br>&emsp;\<li>Fourth item\</li><br>\</ul>|· First item<br>· Second item<br>· Third item<br>&emsp;○ Indented item<br>&emsp;○ Indented item<br>· Fourth item|

If you need to start an unordered list with a number follower by a period, you can use a backslash after the period for escaping.
|Markdown|HTML|Output|
|---|---|---|
|- 1968\. A great year!<br>- I think 1969 was second best.|\<ul><br>&emsp;\<li>1968. A great year!\</li><br>&emsp;\<li>I think 1969 was second best.\</li><br>\</ul>|· 1968. A great year!<br>· I think 1969 was second best.|

|✅ Do this|❌ Don't do this|
|---|---|
|- First item<br>- Second item<br>- Third item<br>- Fourth item|+ First item<br>* Second item<br>- Third item<br>+ Fourth item|

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

#### Paragraphs
```
* This is the first list item.
* Here's the second list item.
    I need to add another paragraph below the second list item.
* And here's the third list item.
```

* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third list item.

#### Blockquotes

```
* This is the first list item.
* Here's the second list item.
    > I need to add another quoteblock below the second list item.
* And here's the third list item.
```

* This is the first list item.
* Here's the second list item.

    > I need to add another quoteblock below the second list item.

* And here's the third list item.

#### Code Blocks
Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

```
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.
```

1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

#### Image

```
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.
```

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.

#### Lists
You can nest an unordered list in an ordered list, or vice versa.

```
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item
```

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

# 6. <y>Code</y>
To denote a word or phrase as code, enclose it in backticks (`).

|Markdown|HTML|Output|
|---|---|---|
|At the command prompt, type \`nano\`.|At the command prompt, type \<code>nano\</code>.|At the command prompt, type `nano`.|

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (``).

|Markdown|HTML|Output|
|---|---|---|
|\`\`Use \`code\` in your Markdown file.\`\`|\<code>Use \`code\` in your Markdown file.\</code>|Use \`code\` in your Markdown file.|

# 7. <y>Code Blocks</y>
To create code blocks, indent every line of the block by at least four spaces or one tab.
```
    <html>
      <head>
      </head>
    </html>
```

The rendered output looks like this:

    <html>
      <head>
      </head>
    </html>

# 8. <y>Horizontal Rules</y>

To create a horizontal rule, use three or more asterisks (***), dashes (---), or underscores (___) on a line by themselves.
For compatibility, put blank lines before and after horizontal rules.

|✅ Do this|❌ Don't do this|
|---|---|
|Try to put a blank line before...<br><br>---<br><br>...and after a horizontal rule.|Without blank lines, this would be a heading.<br>---<br>Don't do this!|

# 9. <y>Links</y>

To create a link, enclose the link text in brackets (e.g., [Duck Duck Go]) and then follow it immediately with the URL in parentheses (e.g., \(https://duckduckgo.com\)).

```
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
```

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in quotation marks after the URL.

```
My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
```

The rendered output looks like this:

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").

To quickly turn a URL or email address into a link, enclose it in angle brackets.

```
<https://www.markdownguide.org>
<fake@example.com>
```

The rendered output looks like this:
<https://www.markdownguide.org>
<fake@example.com>

To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.

```
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```

The rendered output looks like this:
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

Reference-style links are a special kind of link that make URLs easier to display and read in Markdown. Reference-style links are constructed in two parts: the part you keep inline with your text and the part you store somewhere else in the file to keep the text easy to read.

Formatting the First Part of the Link
The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

Although not required, you can include a space between the first and second set of brackets. The label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

This means the following example formats are roughly equivalent for the first part of the link:

The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

Although not required, you can include a space between the first and second set of brackets. The label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

This means the following example formats are roughly equivalent for the first part of the link:

- [hobbit-hole][1]
- [hobbit-hole] [1]

The second part of a reference-style link is formatted with the following attributes:

The label, in brackets, followed immediately by a colon and at least one space (e.g., [label]: ).
The URL for the link, which you can optionally enclose in angle brackets.
The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.
This means the following example formats are all roughly equivalent for the second part of the link:

- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
- \[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
- \[1]: \<https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
- \[1]: \<https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
- \[1]: \<https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)

You can place this second part of the link anywhere in your Markdown document. Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document (like endnotes or footnotes).

Markdown applications don’t agree on how to handle spaces in the middle of a URL. For compatibility, try to URL encode any spaces with %20. Alternatively, if your Markdown application supports HTML, you could use the a HTML tag.

|✅ Do this|❌ Don't do this|
|---|---|
|`[link](https://www.example.com/my%20great%20page)`<br><br>`<a href="https://www.example.com/my great page">link</a>`|\[link](https://www.example.com/my great page)|

Parentheses in the middle of a URL can also be problematic. For compatibility, try to URL encode the opening parenthesis (() with %28 and the closing parenthesis ()) with %29. Alternatively, if your Markdown application supports HTML, you could use the a HTML tag.

|✅ Do this|❌ Don't do this|
|---|---|
|`[a novel](https://en.wikipedia.org/wiki/The_Milagro_Beanfield_War_%28novel%29)`<br><br>\<a href="https://en.wikipedia.org/wiki/The_Milagro_Beanfield_War_(novel)">a novel\</a>|\[a novel](https://en.wikipedia.org/wiki/The_Milagro_Beanfield_War_(novel))|

# 10. <y>Images</y>

To add an image, add an exclamation mark (!), followed by alt text in brackets, and the path or URL to the image asset in parentheses. You can optionally add a title in quotation marks after the path or URL.

```
![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")
```

To resize an image, see the section on image size. To add a caption, see the section on image captions.

To add a link to an image, enclose the Markdown for the image in brackets, and then add the link in parentheses.

```
[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)
```

# 11. <y>Escaping Characters</y>

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (\) in front of the character.

```
\* Without the backslash, this would be a bullet in an unordered list.
```

The rendered output looks like this:

\* Without the backslash, this would be a bullet in an unordered list.

|Character|Name|
|---|---|
|\\ |backslash|
|`|backtick|
|*|asterisk|
|_|underscore|
|{}|curly brackets|
|[]|square brackets|
|<>|angle brackets|
|()|parentheses|
|#|pound sign|
|+|plus sign|
|-|minus sign(hyphen)|
|.|dot|
|!|exclamation mark|
|\||pipe|

# 12. <y>HTML</y>

Many Markdown applications allow you to use HTML tags in Markdown-formatted text. This is helpful if you prefer certain HTML tags to Markdown syntax. For example, some people find it easier to use HTML tags for images. Using HTML is also helpful when you need to change the attributes of an element, like specifying the color of text or changing the width of an image.

To use HTML, place the tags in the text of your Markdown-formatted file.

```
This **word** is bold. This <em>word</em> is italic.
```

The rendered output looks like this:

This **word** is bold. This <em>word</em> is italic.

For security reasons, not all Markdown applications support HTML in Markdown documents. When in doubt, check your Markdown application’s documentation. Some applications support only a subset of HTML tags.

Use blank lines to separate block-level HTML elements like \<div>, \<table>, \<pre>, and \<p> from the surrounding content. Try not to indent the tags with tabs or spaces — that can interfere with the formatting.

You can’t use Markdown syntax inside block-level HTML tags. For example, \<p>italic and \*\*bold\*\*\</p> won’t work.

# 13. <y>Lightweight Markup Languages</y>
Not all Markdown applications support extended syntax elements. You’ll need to check whether or not the lightweight markup language your application is using supports the extended syntax elements you want to use. If it doesn’t, it may still be possible to enable extensions in your Markdown processor.

Lightweight Markup Languages
There are several lightweight markup languages that are supersets of Markdown. They include basic syntax and build upon it by adding additional elements like tables, code blocks, syntax highlighting, URL auto-linking, and footnotes. Many of the most popular Markdown applications use one of the following lightweight markup languages:

- CommonMark
- GitHub Flavored Markdown (GFM)
- Markdown Extra
- MultiMarkdown
- R Markdown

There are dozens of Markdown processors available. Many of them allow you to add extensions that enable extended syntax elements. Check your processor’s documentation for more information.

# 13. <y>Table</y>
- <b>Header and Content</b> delimited by <b><r>-</r></b>
- <b>Columns</b> delimited by <b><r>|</r></b>
  
```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

The rendered output looks like this:

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

Cell widths can vary, as shown below. The rendered output will look the same.

- <b>Alignment</b>
You can align text in the columns to the left, right, or center by adding a colon to the left, right, or on both side of the hyphens within the header row.

```Markdown
| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
```

You can format the text within tables. For example, you can add links, code (words or phrases in backticks (`) only, not code blocks), and emphasis.
You can’t use headings, blockquotes, lists, horizontal rules, images, or most HTML tags.

You can display a pipe (|) character in a table by using its HTML character code (\&#124;).

You can separate paragraphs within a table cell by using one or more <br> HTML tags.

```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title |
| Paragraph   | First paragraph. <br><br> Second paragraph. |
```

The rendered output looks like this:

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title |
| Paragraph   | First paragraph. <br><br> Second 

You can add a list within a table cell by using HTML tags.

```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title |
| List        | Here's a list! <ul><li>Item one.</li><li>Item two.</li></ul> |
``` 

The rendered output looks like this:

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title |
| List        | Here's a list! <ul><li>Item one.</li><li>Item two.</li></ul> |

# 14. <y>Fenced Code Block</y>
The basic Markdown syntax allows you to create code blocks by indenting lines by four spaces or one tab. If you find that inconvenient, try using fenced code blocks. Depending on your Markdown processor or editor, you’ll use three backticks (```) or three tildes (~~~) on the lines before and after the code block. The best part? You don’t have to indent any lines!

\`\`\`
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
\`\`\`

The rendered output looks like this:

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Many Markdown processors support syntax highlighting for fenced code blocks. This feature allows you to add color highlighting for whatever language your code was written in. To add syntax highlighting, specify a language next to the backticks before the fenced code block.

# 15. Footnotes
Footnotes allow you to add notes and references without cluttering the body of the document. When you create a footnote, a superscript number with a link appears where you added the footnote reference. Readers can click the link to jump to the content of the footnote at the bottom of the page.

To create a footnote reference, add a caret and an identifier inside brackets (\[^1]). Identifiers can be numbers or words, but they can’t contain spaces or tabs. Identifiers only correlate the footnote reference with the footnote itself — in the output, footnotes are numbered sequentially.

Add the footnote using another caret and number inside brackets with a colon and text (\[^1]: My footnote.). You don’t have to put footnotes at the end of the document. You can put them anywhere except inside other elements like lists, block quotes, and tables.

```
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```

The rendered output looks like this:

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.

# 16. <y>Heading IDs</y>

Many Markdown processors support custom IDs for headings — some Markdown processors automatically add them. Adding custom IDs allows you to link directly to headings and modify them with CSS. To add a custom heading ID, enclose the custom ID in curly braces on the same line as the heading.

```
### My Great Heading {#custom-id}
```

```
The HTML looks like this:
<h3 id="custom-id">My Great Heading</h3>
```

You can link to headings with custom IDs in the file by creating a standard link with a number sign (#) followed by the custom heading ID. These are commonly referred to as **anchor links**.
Other websites can link to the heading by adding the custom heading ID to the full URL of the webpage (e.g, \[Heading IDs](https://www.markdownguide.org/extended-syntax#heading-ids)).


|Markdown|HTML|Output|
|---|---|---|
|\[Heading IDs](#heading-ids)|\<a href="#heading-ids">Heading IDs</a>|[Heading IDs](#heading-ids)|

# 17. <y>Definition Lists</y>
Some Markdown processors allow you to create definition lists of terms and their corresponding definitions. To create a definition list, type the term on the first line. On the next line, type a colon followed by a space and the definition.

```
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```

```
The HTML looks like this:

<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term. </dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```
The rendered output looks like this:

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

# 18. <y>Strikethrough</y>
You can strikethrough words by putting a horizontal line through the center of them. The result looks like this. This feature allows you to indicate that certain words are a mistake not meant for inclusion in the document. To strikethrough words, use two tilde symbols (~~) before and after the words.

```
~~The world is flat.~~ We now know that the world is round.
```
~~The world is flat.~~ We now know that the world is round.

# 19. <y>Task Lists</y>
Task lists (also referred to as checklists and todo lists) allow you to create a list of items with checkboxes. In Markdown applications that support task lists, checkboxes will be displayed next to the content. To create a task list, add dashes (-) and brackets with a space ([ ]) in front of task list items. To select a checkbox, add an x in between the brackets ([x]).

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

# 20. <y>Emoji</y>
There are two ways to add emoji to Markdown files: copy and paste the emoji into your Markdown-formatted text, or type emoji shortcodes.

In most cases, you can simply copy an emoji from a source like Emojipedia and paste it into your document. Many Markdown applications will automatically display the emoji in the Markdown-formatted text. The HTML and PDF files you export from your Markdown application should display the emoji.
 > Tip: If you're using a static site generator, make sure you encode HTML pages as UTF-8.
Some Markdown applications allow you to insert emoji by typing emoji shortcodes. These begin and end with a colon and include the name of an emoji.

```
Gone camping! :tent: Be back soon.

That is so funny! :joy:
```

The rendered output looks like this:

Gone camping! ⛺ Be back soon.

That is so funny! 😂

# 21. <y>Highlight</y>
This isn’t common, but some Markdown processors allow you to highlight text. The result looks like this. To highlight words, use two equal signs (==) before and after the words.

```
I need to highlight these ==very important words==.
```
I need to highlight these ==very important words==.

Alternatively, if your Markdown application supports HTML, you can use the mark HTML tag.

```
I need to highlight these <mark>very important words</mark>.
```

# 22. <y>Subscript</y>
This isn’t common, but some Markdown processors allow you to use subscript to position one or more characters slightly below the normal line of type. To create a subscript, use one tilde symbol (~) before and after the characters.

```
H~2~O
```

H~2~O

> Tip: Be sure to test this in your Markdown application before using it. Some Markdown applications use one tilde symbol before and after words not for subscript, but for strikethrough.

Alternatively, if your Markdown application supports HTML, you can use the sub HTML tag.

```
H<sub>2</sub>O
```

# 23. <y>Superscript</y>
This isn’t common, but some Markdown processors allow you to use superscript to position one or more characters slightly above the normal line of type. To create a superscript, use one caret symbol (^) before and after the characters.

```
X^2^
```

The rendered output looks like this:

X^2^

Alternatively, if your Markdown application supports HTML, you can use the sup HTML tag.

```
X<sup>2</sup>
```

# 24. <y>Automatic URL linking</y>
Many Markdown processors automatically turn URLs into links. That means if you type http://www.example.com, your Markdown processor will automatically turn it into a link even though you haven’t used brackets.
```
http://www.example.com
```

The rendered output looks like this:

http://www.example.com

If you don’t want a URL to be automatically linked, you can remove the link by denoting the URL as code with backticks.

```
`http://www.example.com`
```

The rendered output looks like this:

`http://www.example.com`

# 25. <y>Underline</y>
Underlined text is not something you typically see in web writing, probably because underlined text is nearly synonymous with links. However, if you’re writing a paper or a report, you may need the ability to underline words and phrases. A couple of applications like Bear and Simplenote provide support for underlining text, but Markdown doesn’t natively support underlining. If your Markdown processor supports HTML, you can use the \<ins> HTML tag to underline text in your document.

```
Some of these words <ins>will be underlined</ins>.
```

The rendered output looks like this:

Some of these words <ins>will be underlined</ins>.

# 26. <y>Indent(Tab)</y>
Tabs and whitespace have a special meaning in Markdown. You can use trailing whitespace to create line breaks, and you can use tabs to create code blocks. But what if you need to indent a paragraph the old-fashioned way, using the tab key? Markdown doesn’t provide an easy way of doing that.

Your best bet might be to use a Markdown editor that supports indentation. This is common in applications that are more oriented towards desktop publishing. For example, iA Writer allows you to customize indentation settings for the editor in the application preferences. It also provides template customization options so that you can make the rendered document look the way you expect it to, indentation and all.

Another option, if your Markdown processor supports HTML, is to use the HTML entity for non-breaking space (\&nbsp;). This should probably be your option of last resort as it can get awkward. Basically, every \&nbsp; in your Markdown source will be replaced with a space in the rendered output. So if you stick four instances of \&nbsp; before a paragraph, the paragraph will look like it’s indented four spaces.

```
&nbsp;&nbsp;&nbsp;&nbsp;This is the first sentence of my indented paragraph.
```

The rendered output looks like this:

&nbsp;&nbsp;&nbsp;&nbsp;This is the first sentence of my indented paragraph.

# 27. <y>Center</y>
Having the ability to center text is a necessity when writing a paper or a report. Unfortunately, Markdown doesn’t have any concept of text alignment (one possible exception is when using tables). The good news is that there’s an HTML tag you can use: \<center>. If your Markdown processor supports HTML, you can place these tags around whatever text you want to center align.

```
<center>This text is centered.</center>
```

The rendered output looks like this:

<center>This text is centered.</center>

The \<center> HTML tag is technically supported but officially deprecated, which means it works for now but you’re not supposed to be using it. Unfortunately, there’s not another pure HTML alternative. You could try using one of the CSS alternatives. Not all Markdown applications provide CSS support, but if the one you’re using does, here’s an alternative to the \<center> tag:

```
<p style="text-align:center">Center this text</p>
```

If this is supported by your Markdown application, the output looks like this:

<p style="text-align:center">Center this text</p>

# 28. <y>Color</y>
Markdown doesn’t allow you to change the color of text, but if your Markdown processor supports HTML, you can use the \<font> HTML tag. The color attribute allows you to specify the font color using a color’s name or the hexadecimal #RRGGBB code.

```
<font color="red">This text is red!</font>
```

The rendered output looks like this:

<font color="red">This text is red!</font>

The \<font> HTML tag is technically supported but officially deprecated, which means it works for now but you’re not supposed to be using it. Unfortunately, there’s not another pure HTML alternative. You could try using one of the CSS alternatives. Not all Markdown applications provide CSS support, but if the one you’re using does, here’s an alternative to the \<font> tag:

```
<p style="color:blue">Make this text blue.</p>
```

If this is supported by your Markdown application, the output looks like this:

<p style="color:blue">Make this text blue.</p>

# 29. <y>Comments</y>
Some people need the ability to write sentences in their Markdown files that will not appear in the rendered output. These comments are essentially hidden text. The text is viewable by the author of the document, but it’s not printed on the webpage or PDF. Markdown doesn’t natively support comments, but several enterprising individuals have devised a solution.
To add a comment, place text inside brackets followed by a colon, a space, and a pound sign (e.g., \[comment]: #). You should put blank lines before and after a comment.

```
Here's a paragraph that will be visible.

[This is a comment that will be hidden.]: # 

And here's another paragraph that's visible
```

The rendered output looks like this:

Here's a paragraph that will be visible.

[This is a comment that will be hidden.]: # 

And here's another paragraph that's visible

> This tip comes from Stack Overflow. It's been peer-reviewed and used by thousands of people!

# 30. <y>Admonition</y>
Admonitions are frequently used in documentation to call attention to warnings, notes, and tips. Markdown doesn’t provide special syntax for admonitions, and most Markdown applications don’t provide support for admonitions (one exception is MkDocs).

```
> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.
```

The rendered output looks like this:

> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.

# 31. <y>Image Size</y>
The Markdown syntax for images doesn’t allow you to specify the width and height of images. If you need to resize an image and your Markdown processor supports HTML, you can use the img HTML tag with the width and height attributes to set the dimensions of an image in pixels.

```HTML
<img src="image.png" width="200" height="100">
```

The rendered output will contain the image resized to the dimensions you specified.

# 32. <y>Image Captions</y>
Markdown doesn’t natively support image captions, but there are two possible workarounds. If your Markdown application supports HTML, you can use the figure and figcaption HTML tags to add a caption for your image.

```HTML
<figure>
    <img src="/assets/images/albuquerque.jpg"
         alt="Albuquerque, New Mexico">
    <figcaption>A single track trail outside of Albuquerque, New Mexico.</figcaption>
</figure>
```

> Tip: If your Markdown application supports CSS, you can use CSS to style the appearance of the caption.

If your Markdown application doesn’t support HTML, you could try placing the caption directly below the image and using emphasis.

```
![Albuquerque, New Mexico](/assets/images/albuquerque.jpg)
*A single track trail outside of Albuquerque, New Mexico.*
```

# 32. <y>Link Targets</y>
Some people like creating links that open in new tabs or windows. The Markdown syntax for links doesn’t allow you to specify the target attribute, but if your Markdown processor supports HTML, you can use HTML to create these links.

```HTML
<a href="https://www.markdownguide.org" target="_blank">Learn Markdown!</a>
```

The rendered output looks like this:

<a href="https://www.markdownguide.org" target="_blank">Learn Markdown!</a>

# 32. <y>Symbols</y>
Markdown doesn’t provide special syntax for symbols. However, in most cases, you can copy and paste whatever symbol you want to use into your Markdown document. For example, if you need to display Pi (π), just find the symbol on a webpage and copy and paste it into your document. The symbol should appear as expected in the rendered output.
Alternatively, if your Markdown application supports HTML, you can use the HTML entity for whatever symbol you want to use. For example, if you want to display the copyright sign (©), you can copy and paste the HTML entity for copyright (&copy;) into your Markdown document

Here’s a partial list of HTML entities for symbols:
- Copyright (©) — &copy;
- Registered trademark (®) — &reg;
- Trademark (™) — &trade;
- Euro (€) — &euro;
- Left arrow (←) — &larr;
- Up arrow (↑) — &uarr;
- Right arrow (→) — &rarr;
- Down arrow (↓) — &darr;
- Degree (°) — &#176;
- Pi (π) — &#960;

For a complete list of available HTML entities, refer to Wikipedia’s page on HTML entities.

# 33. <y>Table of Contents</y>
Some Markdown applications like Markdeep can automatically generate a table of contents (also referred to as a toc) from your headings, but this isn’t a feature provided by all Markdown applications. However, if your Markdown application supports heading IDs, you can create a table of contents for your Markdown file using a list and some links.

```
#### Table of Contents

- [Underline](#underline)
- [Indent](#indent)
- [Center](#center)
- [Color](#color)
```

The rendered output looks like this:

#### Table of Contents

- [Underline](#underline)
- [Indent](#indent)
- [Center](#center)
- [Color](#color)

# 34. <y>Videos</y>
If your Markdown application supports HTML, you should be able to embed a video in your Markdown file by copying and pasting the HTML code provided by a video website like YouTube or Vimeo. If your Markdown application doesn’t support HTML, you can’t embed a video, but you can come close by adding an image and a link to the video. You could do this with practically any video on any video service.

Since YouTube makes this easy, we’ll use them as an example. Take this video, for instance: \https://www.youtube.com/watch?v=8q2IjQOzVpE. The last part of the URL (8q2IjQOzVpE) is the ID of the video. We can take that ID and put it in the following template:

```
[![Image alt text](https://img.youtube.com/vi/YOUTUBE-ID/0.jpg)](https://www.youtube.com/watch?v=YOUTUBE-ID)
```

YouTube automatically generates an image for every video (https://img.youtube.com/vi/YOUTUBE-ID/0.jpg), so we can use that and link the image to the video on YouTube. After we replace the image alt text and add the ID of the video, our example looks like this:

```
[![Less Than Jake — Scott Farcas Takes It On The Chin](https://img.youtube.com/vi/PYCxct2e0zI/0.jpg)](https://www.youtube.com/watch?v=PYCxct2e0zI)
```

The rendered output looks like this:

[![Less Than Jake — Scott Farcas Takes It On The Chin](https://img.youtube.com/vi/PYCxct2e0zI/0.jpg)](https://www.youtube.com/watch?v=PYCxct2e0zI)
