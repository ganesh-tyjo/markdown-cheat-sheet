<p align="center">
<img src="./content/images/markdown-logo.png" alt="Markdown" heigh="150" width="150">
<p align="center">Markdown Cheat Sheet</p>
</p>

---

<br/>
<details open="open">
  <summary>Table Of Contents</summary>

- [Headers](#headers)
- [Quotes](#quotes)
- [Emphasis](#emphasis)
- [Horizontal Rule](#horizontal-rule)
- [Lists](#lists)
- [Links](#links)
- [Images](#images)
- [Code](#code)
- [Tables](#tables)
- [Custom HTML](#custom-html)
- [Custom CSS](#custom-css)

</details>

## Headers

Headers are defined by the '#' symbol. One '#' for H1, two for H2, etc.

# Heading 1

## Heading 2

### Heading 3

...

###### Heading 6

## Quotes

Quotes are defined by the '>' symbol.

> This is quote

> # This is header quote

## Emphasis

Add emphasis with asterisks '\*' and underscores '\_'.

Two before and after (no spaces) a section of texts makes it bold.

**This text** is bold

One before and after (no spaces) a section of texts makes it italic.

_This text_ is italic

Create strike through text using tilde '~'.

Two before and after (no spaces) a section of texts makes it strike-through.

~~This text~~ is strike-through

## Horizontal Rule

A horizontal rule gives a visible line break. You can create one by putting three or more hyphens, asterisks or underscores (-, \*, \_).

---

## Lists

You can create sub-lists by indenting.

Create unordered lists using '-', '\*', '+'.

- List Item 1
- List Item 2
- List Item 3
  - Sub-List Item 1
  - Sub-List Item 2

Create ordered lists using a number prefix.

1. List Item 1
2. List Item 2
3. List Item 3
   1. Sub-List Item 1
   2. Sub-List Item 2

Create task list using brackets [].

- [x] Task 1
- [x] Task 2
- [ ] Task 3

## Links

Create a link by surrounding it with angle bracket.

<https://github.com/ganesh-tyjo>

Create a link with text by surrounding text with brackets, [], and link immediately following with parenthesis ().

[My GitHub Profile](https://github.com/ganesh-tyjo)

You can also show alias for your original link when mouse gets hover over your link. You can do that by providing alias immediately after specifying link in parenthesis ().

[My GitHub Profile](https://github.com/ganesh-tyjo 'github/ganesh-tyjo')

What if you needed to reuse a link several times? Well, you could copy and paste that link each time. That means, if you need to update the link, you will have to do it each time its used. There's a better way!

Create reference style links by defining your link with the a 'key' inside of brackets, colon, space, and the link.

```
[my-profile-link]: https://github.com/ganesh-tyjo
```

[my-profile-link]: https://github.com/ganesh-tyjo

Then use the reference style link by using your text inside of brackets followed by the link 'key' inside of bracket.

[My GitHub Profile][my-profile-link]

You can also link to other locations on your markdown page. Remember, your Markdown will get converted to HTML, so you can, in theory, use a anchor tag to link to an element with a specific ID. You can find an example of this in the table of contents at the top of this document.

When we create a header tag for example, it implicitly creates an id property.

Ex '# Header' becomes `<h1 id="header">Header</h1>`

Names will be converted to ids by replacing spaces with hyphens and uppercase letters with lowercase letters (think css naming convention).

Ex 'Header Info' becomes header-info

[Go To Headers](#headers)

## Images

Defining an image is similar to defining a link, except you prefix it with '!'.

![Markdown Logo](./content/images/markdown-logo.png)

## Code

You can do inline code with `back-ticks` (\` \`).

You can do blocks of code by surround it with 3 back-ticks (\`\`\` \`\`\`).

```javascript
var num1 = 0;
var num2 = 0;
```

```html
<div>
  <p>This is an html example</p>
</div>
```

```bash
npm install
```

## Tables

Tables are useful for displaying rows and columns of data. Column headers can be defined in between pipes (|). Headers are separated from table content with a row of dashes (-) (still separated by pipes), and there must be at least 3 dashes between each header. The row data follows beneath (still separated by pipes).

| Header 1    | Header 2    | Header 3    |
| ----------- | ----------- | ----------- |
| Row 1 Col 1 | Row 1 Col 2 | Row 1 Col 3 |

You can also align (center, left, right) the text in a column by using colons (:) in the line breaks between headers and rows. No colon means the default **left alignment**. Colons on each side signifies **center alignment**. And a trailing colon means **right alignment**.

| Header 1                                  |                 Header 2                  |                                  Header 3 |
| ----------------------------------------- | :---------------------------------------: | ----------------------------------------: |
| Aligned Left                              |              Aligned Center               |                             Aligned Right |
| Large string to show alignment is working | Large string to show alignment is working | Large string to show alignment is working |

## Custom HTML

Since Markdown gets automatically converted to HTML, you can add raw HTML directly to your Markdown.

<p class="paragraph">This is a paragraph created with HTML</p>

## Custom CSS

You can also add custom CSS to your Markdown to add additional styling to your document. You can also include CSS by including a style tag.

```css
<style>
.paragraph{
  color:#31a1d6;
  border: 1px solid #e8e9ea;
  border-radius:15px;
  padding:10px;
}
</style>
```

<style>
.paragraph{
  color:#31a1d6;
  border: 1px solid #e8e9ea;
  border-radius:15px;
  padding:10px;
}
</style>
