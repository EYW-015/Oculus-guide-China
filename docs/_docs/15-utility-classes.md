---
title: Utility Classes
permalink: /docs/utility-classes/
excerpt: 'CSS classes for aligning text/image, styling buttons and notices, and more.'
last_modified_at: '2018-11-26T00:46:43.000Z'
toc: true
toc_label: Utility Classes
toc_icon: cogs
---

# 15-utility-classes

Using the Kramdown Markdown renderer with Jekyll allows you to add [block](http://kramdown.gettalong.org/quickref.html#block-attributes) and [inline attributes](http://kramdown.gettalong.org/quickref.html#inline-attributes). This is nice if you want to add custom styling to text and image, and still write in Markdown.

**Jekyll 3:** Kramdown is the default for `jekyll new` sites and those hosted on GitHub Pages. Not using Kramdown? That's OK. The following classes are still available when used with standard HTML. {: .notice--warning}

## Text alignment

Align text blocks with the following classes.

Left aligned text `.text-left` {: .text-left}

```text
Left aligned text
{: .text-left}
```

Center aligned text. `.text-center` {: .text-center}

```text
Center aligned text.
{: .text-center}
```

Right aligned text. `.text-right` {: .text-right}

```text
Right aligned text.
{: .text-right}
```

**Justified text.** `.text-justify` Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque vel eleifend odio, eu elementum purus. In hac habitasse platea dictumst. Fusce sed sapien eleifend, sollicitudin neque non, faucibus est. Proin tempus nisi eu arcu facilisis, eget venenatis eros consequat. {: .text-justify}

```text
Justified text.
{: .text-justify}
```

No wrap text. `.text-nowrap` {: .text-nowrap}

```text
No wrap text.
{: .text-nowrap}
```

## Image alignment

Position images with the following classes.

!\[image-center\]\(\){: .align-center}

The image above happens to be **centered**.

```text
![image-center](/assets/images/filename.jpg){: .align-center}
```

!\[image-left\]\(\){: .align-left} The rest of this paragraph is filler for the sake of seeing the text wrap around the 150×150 image, which is **left aligned**. There should be plenty of room above, below, and to the right of the image. Just look at him there --- Hey guy! Way to rock that left side. I don't care what the right aligned image says, you look great. Don't let anyone else tell you differently.

```text
![image-left](/assets/images/filename.jpg){: .align-left}
```

!\[image-right\]\(\){: .align-right}

And now we're going to shift things to the **right align**. Again, there should be plenty of room above, below, and to the left of the image. Just look at him there --- Hey guy! Way to rock that right side. I don't care what the left aligned image says, you look great. Don't let anyone else tell you differently.

```text
![image-right](/assets/images/filename.jpg){: .align-right}
```

!\[full\]\(\) {: .full}

The image above should extend outside of the parent container on right.

```text
![full](/assets/images/filename.jpg)
{: .full}
```

## Buttons

Make any link standout more when applying the `.btn .btn--primary` classes.

```markup
<a href="#" class="btn btn--primary">Link Text</a>
```

| Button Type | Example | Class | Kramdown |
| :--- | :--- | :--- | :--- |
| Default | [Text](15-utility-classes.md#link){: .btn} | `.btn` | `[Text](#link){: .btn}` |
| Primary | [Text](15-utility-classes.md#link){: .btn .btn--primary} | `.btn .btn--primary` | `[Text](#link){: .btn .btn--primary}` |
| Success | [Text](15-utility-classes.md#link){: .btn .btn--success} | `.btn .btn--success` | `[Text](#link){: .btn .btn--success}` |
| Warning | [Text](15-utility-classes.md#link){: .btn .btn--warning} | `.btn .btn--warning` | `[Text](#link){: .btn .btn--warning}` |
| Danger | [Text](15-utility-classes.md#link){: .btn .btn--danger} | `.btn .btn--danger` | `[Text](#link){: .btn .btn--danger}` |
| Info | [Text](15-utility-classes.md#link){: .btn .btn--info} | `.btn .btn--info` | `[Text](#link){: .btn .btn--info}` |
| Inverse | [Text](15-utility-classes.md#link){: .btn .btn--inverse} | `.btn .btn--inverse` | `[Text](#link){: .btn .btn--inverse}` |
| Light Outline | [Text](15-utility-classes.md#link){: .btn .btn--light-outline} | `.btn .btn--light-outline` | `[Text](#link){: .btn .btn--light-outline}` |

| Button Size | Example | Class | Kramdown |
| :--- | :--- | :--- | :--- |
| X-Large | [X-Large Button](15-utility-classes.md){: .btn .btn--primary .btn--x-large} | `.btn .btn--primary .btn--x-large` | `[Text](#link){: .btn .btn--primary .btn--x-large}` |
| Large | [Large Button](15-utility-classes.md){: .btn .btn--primary .btn--large} | `.btn .btn--primary .btn--large` | `[Text](#link){: .btn .btn--primary .btn--large}` |
| Default | [Default Button](15-utility-classes.md){: .btn .btn--primary} | `.btn .btn--primary` | `[Text](#link){: .btn .btn--primary }` |
| Small | [Small Button](15-utility-classes.md){: .btn .btn--primary .btn--small} | `.btn .btn--primary .btn--small` | `[Text](#link){: .btn .btn--primary .btn--small}` |

## Notices

Call attention to a block of text.

| Notice Type | Class |
| :--- | :--- |
| Default | `.notice` |
| Primary | `.notice--primary` |
| Info | `.notice--info` |
| Warning | `.notice--warning` |
| Success | `.notice--success` |
| Danger | `.notice--danger` |

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice}` class. {: .notice}

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice--primary}` class. {: .notice--primary}

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice--info}` class. {: .notice--info}

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice--warning}` class. {: .notice--warning}

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice--success}` class. {: .notice--success}

**Watch out!** This paragraph of text has been [emphasized](15-utility-classes.md) with the `{: .notice--danger}` class. {: .notice--danger}

### Notice Headline:

 {{ notice-text \| markdownify }}

