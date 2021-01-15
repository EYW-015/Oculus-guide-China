---
title: 'Layout: Post with Sticky Table of Contents'
tags:
  - table of contents
toc: true
toc_sticky: true
---

# 2012-01-03-layout-table-of-contents-sticky

"Stick" table of contents to the top of a page by adding `toc_sticky: true` to its YAML Front Matter.

```yaml
---
toc: true
toc_sticky: true
---
```

## HTML Elements

Below is just about everything you'll need to style in the theme. Check the source code to see the many embedded elements within paragraphs.

## Body text

Lorem ipsum dolor sit amet, test link adipiscing elit. **This is strong**. Nullam dignissim convallis est. Quisque aliquam.

![Smithsonian Image](https://github.com/eyw015/Oculus-Net-for-China/tree/2ba99564d79f651cb996c64aea9ca0fa00c344df/test/_posts/%7B%7B%20site.url%20%7D%7D%7B%7B%20site.baseurl%20%7D%7D/assets/images/3953273590_704e3899d5_m.jpg) {: .image-right}

_This is emphasized_. Donec faucibus. Nunc iaculis suscipit dui. 53 = 125. Water is H2O. Nam sit amet sem. Aliquam libero nisi, imperdiet at, tincidunt nec, gravida vehicula, nisl. The New York Times \(That’s a citation\). Underline.Maecenas ornare tortor. Donec sed tellus eget sapien fringilla nonummy. Mauris a ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus.

HTML and CSS are our tools. Mauris a ante. Suspendisse quam sem, consequat at, commodo vitae, feugiat in, nunc. Morbi imperdiet augue quis tellus. Praesent mattis, massa quis luctus fermentum, turpis mi volutpat justo, eu volutpat enim diam eget metus.

### Blockquotes

> Lorem ipsum dolor sit amet, test link adipiscing elit. Nullam dignissim convallis est. Quisque aliquam.

## List Types

### Ordered Lists

1. Item one
   1. sub item one
   2. sub item two
   3. sub item three
2. Item two

### Unordered Lists

* Item one
* Item two
* Item three

## Tables

| Header1 | Header2 | Header3 |
| :--- | :---: | ---: |
| cell1 | cell2 | cell3 |
| cell4 | cell5 | cell6 |
| ---- |  |  |
| cell1 | cell2 | cell3 |
| cell4 | cell5 | cell6 |
| ===== |  |  |
| Foot1 | Foot2 | Foot3 |

{: rules="groups"}

## Code Snippets

```css
#container {
  float: left;
  margin: 0 -240px 0 0;
  width: 100%;
}
```

## Buttons

Make any link standout more when applying the `.btn` class.

```markup
<a href="#" class="btn btn--success">Success Button</a>
```

[Primary Button](2012-01-03-layout-table-of-contents-sticky.md)[Success Button](2012-01-03-layout-table-of-contents-sticky.md)[Warning Button](2012-01-03-layout-table-of-contents-sticky.md)[Danger Button](2012-01-03-layout-table-of-contents-sticky.md)[Info Button](2012-01-03-layout-table-of-contents-sticky.md)

## Notices

**Watch out!** You can also add notices by appending `{: .notice}` to a paragraph. {: .notice}

