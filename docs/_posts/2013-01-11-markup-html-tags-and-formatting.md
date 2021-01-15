---
title: 'Markup: HTML Tags and Formatting'
header:
  teaser: assets/images/markup-syntax-highlighting-teaser.jpg
categories:
  - Markup
tags:
  - content
  - css
  - formatting
  - html
  - markup
toc: true
---

# 2013-01-11-markup-html-tags-and-formatting

A variety of common markup showing how the theme styles them.

### Header two

#### Header three

**Header four**

**Header five**

**Header six**

### Blockquotes

Single line blockquote:

> Stay hungry. Stay foolish.

Multi line blockquote with a cite reference:

> People think focus means saying yes to the thing you've got to focus on. But that's not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I'm actually as proud of the things we haven't done as the things I have done. Innovation is saying no to 1,000 things.

Steve Jobs --- Apple Worldwide Developers' Conference, 1997 {: .small}

### Tables

| Employee | Salary |  |
| :--- | :--- | :--- |
| [John Doe](2013-01-11-markup-html-tags-and-formatting.md) | $1 | Because that's all Steve Jobs needed for a salary. |
| [Jane Doe](2013-01-11-markup-html-tags-and-formatting.md) | $100K | For all the blogging she does. |
| [Fred Bloggs](2013-01-11-markup-html-tags-and-formatting.md) | $100M | Pictures are worth a thousand words, right? So Jane × 1,000. |
| [Jane Bloggs](2013-01-11-markup-html-tags-and-formatting.md) | $100B | With hair like that?! Enough said. |

| Header1 | Header2 | Header3 |
| :--- | :---: | ---: |
| cell1 | cell2 | cell3 |
| cell4 | cell5 | cell6 |
| ----------------------------- |  |  |
| cell1 | cell2 | cell3 |
| cell4 | cell5 | cell6 |
| ============================= |  |  |
| Foot1 | Foot2 | Foot3 |

### Definition Lists

Definition List Title : Definition list division.

Startup : A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.

## dowork

: Coined by Rob Dyrdek and his personal body guard Christopher "Big Black" Boykins, "Do Work" works as a self motivator, to motivating your friends.

Do It Live : I'll let Bill O'Reilly \[explain\]\([https://www.youtube.com/watch?v=O\_HyZ5aW76c](https://www.youtube.com/watch?v=O_HyZ5aW76c) "We'll Do It Live"\) this one.

### Unordered Lists \(Nested\)

* List item one 
  * List item one 
    * List item one
    * List item two
    * List item three
    * List item four
  * List item two
  * List item three
  * List item four
* List item two
* List item three
* List item four

### Ordered List \(Nested\)

1. List item one 
   1. List item one 
      1. List item one
      2. List item two
      3. List item three
      4. List item four
   2. List item two
   3. List item three
   4. List item four
2. List item two
3. List item three
4. List item four

### Forms

Personalia: Name:   
 Email:   
 Date of birth: 

### Buttons

Make any link standout more when applying the `.btn` class.

```markup
<a href="#" class="btn--success">Success Button</a>
```

[Default Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn} [Primary Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--primary} [Success Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--success} [Warning Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--warning} [Danger Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--danger} [Info Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--info} [Inverse Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--inverse} [Light Outline Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--light-outline}

```text
[Default Button Text](#link){: .btn}
[Primary Button Text](#link){: .btn .btn--primary}
[Success Button Text](#link){: .btn .btn--success}
[Warning Button Text](#link){: .btn .btn--warning}
[Danger Button Text](#link){: .btn .btn--danger}
[Info Button Text](#link){: .btn .btn--info}
[Inverse Button](#link){: .btn .btn--inverse}
[Light Outline Button](#link){: .btn .btn--light-outline}
```

[X-Large Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--primary .btn--x-large} [Large Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--primary .btn--large} [Default Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--primary } [Small Button](2013-01-11-markup-html-tags-and-formatting.md){: .btn .btn--primary .btn--small}

```text
[X-Large Button](#link){: .btn .btn--primary .btn--x-large}
[Large Button](#link){: .btn .btn--primary .btn--large}
[Default Button](#link){: .btn .btn--primary }
[Small Button](#link){: .btn .btn--primary .btn--small}
```

### Notices

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice}` class. {: .notice}

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice--primary}` class. {: .notice--primary}

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice--info}` class. {: .notice--info}

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice--warning}` class. {: .notice--warning}

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice--success}` class. {: .notice--success}

**Watch out!** This paragraph of text has been [emphasized](2013-01-11-markup-html-tags-and-formatting.md) with the `{: .notice--danger}` class. {: .notice--danger}

### HTML Tags

#### Address Tag

 1 Infinite Loop  
 Cupertino, CA 95014  
 United States

#### Anchor Tag \(aka. Link\)

This is an example of a [link](http://apple.com).

#### Abbreviation Tag

The abbreviation CSS stands for "Cascading Style Sheets".

\*\[CSS\]: Cascading Style Sheets

#### Cite Tag

"Code is poetry." ---Automattic

#### Code Tag

You will learn later on in these tests that `word-wrap: break-word;` will be your best friend.

#### Strike Tag

This tag will let you strikeout text.

#### Emphasize Tag

The emphasize tag should _italicize_ text.

#### Insert Tag

This tag should denote inserted text.

#### Keyboard Tag

This scarcely known tag emulates keyboard text, which is usually styled like the `<code>` tag.

#### Preformatted Tag

This tag styles large blocks of code.

```text

.post-title {
    margin: 0 0 5px;
    font-weight: bold;
    font-size: 38px;
    line-height: 1.2;
    and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
```

#### Quote Tag

Developers, developers, developers… –Steve Ballmer

#### Strong Tag

This tag shows **bold text**.

#### Subscript Tag

Getting our science styling on with H2O, which should push the "2" down.

#### Superscript Tag

Still sticking with science and Albert Einstein's E = MC2, which should lift the 2 up.

#### Variable Tag

This allows you to denote variables.

