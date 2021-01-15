---
title: 'Post: Image (Standard)'
categories:
  - Post Formats
tags:
  - image
  - Post Formats
---

# 2010-08-05-post-image-standard

The preferred way of using images is placing them in the `/assets/images/` directory and referencing them with an absolute path. Prepending the filename with \`

\` will make sure your images display properly in feeds and such.

Standard image with no width modifier classes applied.

**HTML:**

```markup
{% raw %}<img src="{{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg" alt="">{% endraw %}
```

**or Kramdown:**

```text
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg){% endraw %}
```

![Unsplash image 9](https://github.com/eyw015/Oculus-Net-for-China/tree/2ba99564d79f651cb996c64aea9ca0fa00c344df/test/_posts/%7B%7B%20site.url%20%7D%7D%7B%7B%20site.baseurl%20%7D%7D/assets/images/unsplash-image-9.jpg)

Image that fills page content container by adding the `.full` class with:

**HTML:**

```markup
{% raw %}<img src="{{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg" alt="" class="full">{% endraw %}
```

**or Kramdown:**

```text
{% raw %}![alt]({{ site.url }}{{ site.baseurl }}/assets/images/filename.jpg)
{: .full}{% endraw %}
```

![Unsplash image 10](https://github.com/eyw015/Oculus-Net-for-China/tree/2ba99564d79f651cb996c64aea9ca0fa00c344df/test/_posts/%7B%7B%20site.url%20%7D%7D%7B%7B%20site.baseurl%20%7D%7D/assets/images/unsplash-image-10.jpg) {: .full}

