---
title: 'Post: Notice'
categories:
  - Post Formats
tags:
  - Post Formats
  - notice
---

# 2010-02-05-post-notice

A notice displays information that explains nearby content. Often used to call attention to a particular detail.

When using Kramdown `{: .notice}` can be added after a sentence to assign the `.notice` to the `<p></p>` element.

**Changes in Service:** We just updated our [privacy policy](2010-02-05-post-notice.md) here to better service our customers. We recommend reviewing the changes. {: .notice}

**Primary Notice:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. [Praesent libero](2010-02-05-post-notice.md). Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. {: .notice--primary}

 \*\*Primary Notice with code block:\*\* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. \[Praesent libero\]\(\#\). Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. \`\`\`htmlSome body. \`\`\`

**Info Notice:** Lorem ipsum dolor sit amet, [consectetur adipiscing elit](2010-02-05-post-notice.md). Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. {: .notice--info}

**Warning Notice:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. [Integer nec odio](2010-02-05-post-notice.md). Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. {: .notice--warning}

**Danger Notice:** Lorem ipsum dolor sit amet, [consectetur adipiscing](2010-02-05-post-notice.md) elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. {: .notice--danger}

**Success Notice:** Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at [nibh elementum](2010-02-05-post-notice.md) imperdiet. {: .notice--success}

Want to wrap several paragraphs or other elements in a notice? Using Liquid to capture the content and then filter it with `markdownify` is a good way to go.

```markup
{% raw %}{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}{{ notice-2 | markdownify }}{% endraw %}</div>
```

 {{ notice-2 \| markdownify }}

Or you could skip the capture and stick with straight HTML.

```markup
<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>
```

## Message

A basic message.

