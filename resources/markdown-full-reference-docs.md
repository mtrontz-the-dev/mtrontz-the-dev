# markdown-full-reference-docs

## Markdown Project Page

## Markdown Document

### Introduction

Markdown is a plain text formatting syntax.

Paragraphs are separated by empty lines.

## Heading 1

### Heading 2

#### Heading 3

**Heading 4**

**Heading 5**

**Heading 6**

### Character Styles

These spans result in 'em' tags:

* _single asterisks_
* _single underscores_

These spans result in 'strong' tags:

* **double asterisks**
* **double underscores**

These spans result in 'del' tags:

* ~~double tildes~~

### Links and Images

This is an [example inline link](https://www.actiprosoftware.com) with tooltip text specified. [This link](https://www.actiprosoftware.com) has no tooltip text specified.

URLs and e-mail addresses can be turned into links by enclosing them in angle braces:

* [https://www.actiprosoftware.com](https://www.actiprosoftware.com)  
* [support@microsoft.com](mailto:support@microsoft.com)

[This link](markdown-full-reference-docs.md#markdown-project-page) links to the first heading in this document via custom ID.

### Images

This is an example of an image:

![Image](https://www.microsoft.com/favicon.ico)

This is an example of an image with a link:

[![Image](https://www.google.com/favicon.ico)](https://www.google.com)

### Blockquotes

Markdown said:

> This is the first level of quoting.
>
> > This is a nested blockquote.
>
> Back to the first level.

### Lists

Unordered list using minus signs \(-\):

* Step 1
* Step 2
* Step 3
  * Step 3a
  * Step 3b
  * Step 3c

Unordered list using plus signs \(+\):

* Step 1
* Step 2
* Step 3
  * Step 3a
  * Step 3b
  * Step 3c

Unordered list using asterisks \(\*\):

* Step 1
* Step 2
* Step 3
  * Step 3a
  * Step 3b
  * Step 3c

Ordered list:

1. Step 1
2. Step 2
3. Step 3
   1. Step 3a
   2. Step 3b
   3. Step 3c

Nested \(unordered within ordered\) list:

1. Step 1
2. Step 2
3. Step 3
   * Step 3a
   * Step 3b
   * Step 3c

Definition list:

Term \#1 : This is the definition of term \#1.

Term \#2 : This is the definition of term \#2.

### Code Blocks

Inline `code` can be delimited with characters.

This code block is fenced with three backticks and has its language specified:

```javascript
var oldUnload = window.onbeforeunload;
window.onbeforeunload = function() {
    saveCoverage();
    if (oldUnload) {
        return oldUnload.apply(this, arguments);
    }
};
```

This code block is fenced with three tildes and has its language specified:

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```

This code block is created by indenting the code, but no language can be specified:

```text
var foo = 1;
```

### Tables

| Fruit | Color |
| :--- | :--- |
| Apples | Red |
| Grapes | Purple |
| Lemons | Yellow |

### Horizontal Rules

Horizontal rules are formed by placing three or more hyphens, asterisks, or underscores on a line by themselves.

### HTML Tags

**HTML tags** can optionally be used in _Markdown_.

### Special Characters

Unescaped:  \` \* \_ { } \[ \] \( \) \# + - . !

Backslash-Escaped: \ \` \* \_ { } \[ \] \( \) \# + - . !

## Markdown: Basics

* [Main](https://daringfireball.net/projects/markdown/)
* [Basics](markdown-full-reference-docs.md)
* [Syntax](https://daringfireball.net/projects/markdown/basics)
* [License](https://daringfireball.net/projects/markdown/license)
* [Dingus](https://daringfireball.net/projects/markdown/dingus)

 \#\#\# Credit to \[The Daring Fireball Company LLC\]\(https://daringfireball.net/projects/markdown/\) Getting the Gist of Markdown's Formatting Syntax ------------------------------------------------ This page offers a brief overview of what it's like to use Markdown. The \[syntax page\] \[s\] provides complete, detailed documentation for every feature, but Markdown should be very easy to pick up simply by looking at a few examples of it in action. The examples on this page are written in a before/after style, showing example syntax and the HTML output produced by Markdown. It's also helpful to simply try Markdown out; the \[Dingus\] \[d\] is a web application that allows you type your own Markdown-formatted text and translate it to XHTML. \*\*Note:\*\* This document is itself written using Markdown; you can \[see the source for it by adding '.text' to the URL\] \[src\]. \#\# Paragraphs, Headers, Blockquotes \#\# A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. \(A blank line is any line that looks like a blank line -- a line containing nothing but spaces or tabs is considered blank.\) Normal paragraphs should not be indented with spaces or tabs. Markdown offers two styles of headers: \*Setext\* and \*atx\*. Setext-style headers for \`

## \` and \`\` are created by "underlining" with equal signs \(\`=\`\) and hyphens \(\`-\`\), respectively. To create an atx-style header, you put 1-6 hash marks \(\`\#\`\) at the beginning of the line -- the number of hashes equals the resulting HTML header level. Blockquotes are indicated using email-style '\`&gt;\`' angle brackets. Markdown: A First Level Header ==================== A Second Level Header --------------------- Now is the time for all good men to come to the aid of their country. This is just a regular paragraph. The quick brown fox jumped over the lazy dog's back. \#\#\# Header 3 &gt; This is a blockquote. &gt; &gt; This is the second paragraph in the blockquote. &gt; &gt; \#\# This is an H2 in a blockquote Output:A First Level HeaderA Second Level HeaderNow is the time for all good men to come to the aid of their country. This is just a regular paragraph.The quick brown fox jumped over the lazy dog's back.Header 3This is a blockquote.This is the second paragraph in the blockquote.This is an H2 in a blockquote \#\#\# Phrase Emphasis \#\#\# Markdown uses asterisks and underscores to indicate spans of emphasis. Markdown: Some of these words \*are emphasized\*. Some of these words \_are emphasized also\_. Use two asterisks for \*\*strong emphasis\*\*. Or, if you prefer, \_\_use two underscores instead\_\_. Output:Some of these words _are emphasized_. Some of these words _are emphasized also_.Use two asterisks for **strong emphasis**. Or, if you prefer, **use two underscores instead**. \#\# Lists \#\# Unordered \(bulleted\) lists use asterisks, pluses, and hyphens \(\`\*\`, \`+\`, and \`-\`\) as list markers. These three markers are interchangable; this: \* Candy. \* Gum. \* Booze. this: + Candy. + Gum. + Booze. and this: - Candy. - Gum. - Booze. all produce the same output:Candy.Gum.Booze.

Ordered \(numbered\) lists use regular numbers, followed by periods, as list markers:

1. Red
2. Green
3. Blue

Output:

1. Red
2. Green
3. Blue

If you put blank lines between items, you'll get `<p>` tags for the list item text. You can create multi-paragraph list items by indenting the paragraphs by 4 spaces or 1 tab:

* A list item.

  With multiple paragraphs.

* Another item in the list.

Output:

* A list item.

  With multiple paragraphs.

* Another item in the list.

#### Links \#\#\#

Markdown supports two styles for creating links: _inline_ and _reference_. With both styles, you use square brackets to delimit the text you want to turn into a link.

Inline-style links use parentheses immediately after the link text. For example:

```text
This is an [example link](http://example.com/).
```

Output:

This is an [example link](http://example.com/).

Optionally, you may include a title attribute in the parentheses:

```text
This is an [example link](http://example.com/ "With a Title").
```

Output:

This is an [example link](http://example.com/).

Reference-style links allow you to refer to your links by names, which you define elsewhere in your document:

```text
I get 10 times more traffic from [Google][1] than from
[Yahoo][2] or [MSN][3].

[1]: http://google.com/        "Google"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/    "MSN Search"
```

Output:

I get 10 times more traffic from [Google](http://google.com/) than from [Yahoo](http://search.yahoo.com/) or [MSN](http://search.msn.com/).

The title attribute is optional. Link names may contain letters, numbers and spaces, but are _not_ case sensitive:

```text
I start my morning with a cup of coffee and
[The New York Times][NY Times].

[ny times]: http://www.nytimes.com/
```

Output:

I start my morning with a cup of coffee and [The New York Times](http://www.nytimes.com/).

#### Images \#\#\#

Image syntax is very much like link syntax.

Inline \(titles are optional\):

```text
![alt text](/path/to/img.jpg "Title")
```

Reference-style:

```text
![alt text][id]

[id]: /path/to/img.jpg "Title"
```

Both of the above examples produce the same output:

```text
<img src="/path/to/img.jpg" alt="alt text" title="Title" />
```

#### Code \#\#\#

In a regular paragraph, you can create code span by wrapping text in backtick quotes. Any ampersands \(`&`\) and angle brackets \(`<` or `>`\) will automatically be translated into HTML entities. This makes it easy to use Markdown to write about HTML example code:

```text
I strongly recommend against using any `<blink>` tags.

I wish SmartyPants used named entities like `&mdash;`
instead of decimal-encoded entites like `&#8212;`.
```

Output:

I strongly recommend against using any `<blink>` tags.

I wish SmartyPants used named entities like `&mdash;` instead of decimal-encoded entites like `&#8212;`.

To specify an entire block of pre-formatted code, indent every line of the block by 4 spaces or 1 tab. Just like with code spans, `&`, `<`, and `>` characters will be escaped automatically.

Markdown:

```text
If you want your page to validate under XHTML 1.0 Strict,
you've got to put paragraph tags in your blockquotes:

    <blockquote>
        <p>For example.</p>
    </blockquote>
```

Output:

If you want your page to validate under XHTML 1.0 Strict, you've got to put paragraph tags in your blockquotes:

```text
<blockquote>
        <p>For example.</p>
    </blockquote>
```

