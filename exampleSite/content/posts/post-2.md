+++
title = '02. Features'
date = 2025-03-28
draft = false
featured_image = "https://raw.githubusercontent.com/elecbrandy/freshpink/gh-pages/basic.png"
tags = ['tag_a', 'tag_c']
+++

<br>

## 1. Image Area
This theme provides an image area feature. You can insert a wide image area of your choice at the top of your `.md` file according to the tomel format: `featured_image = “ ”`.Insert a nice image that represents your post.

<br>
<br>

## 2. Tag
____

In each `.md` file, you'll also find a `tags = []` field in the front matter. This is where you can assign tags to your post. For example:

```toml
tags = ['tag_a']
```

You can assign **multiple tags** to a single post, like this:

```toml
tags = ['tag_a', 'tag_c']
```

On my own blog, I often use tags like `['c', 'unix']`.

Now, what if you want to browse all posts by tag? Naturally, you’d want a **Tags** page where your custom tags are listed and clickable. Here's how to enable that ->

1. Go to your `content/tags` directory (create it if it doesn’t exist).
2. Inside, create one `.md` file for each tag you want to appear — for example ->

```
content/tags/tag_a/_index.md
```

That’s it! Hugo will automatically generate tag listing pages for you. Simple, right?

<br>
<br>

## 3. TOC
____
This theme has a TOC. It's on the left side of the body, and by default, it's transparent so it doesn't get in the way of reading the post. When you hover over it, it actually turns into an actionable text. As for the `<h1>` tag, it's considered a heading tag and can be hard to recognize to prevent abuse! Similar to hugo's tendency.

<br>
<br>

## 4. Back to Top Button
A "Back to Top" button, implemented via [**Vanilla Back to Top**](https://github.com/vfeskov/vanilla-back-to-top), enhances navigation on your blog. This convenience feature makes it easy for readers to return to the top of the page, improving the overall user experience.

<br>
<br>
