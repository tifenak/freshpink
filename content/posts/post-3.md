+++
title = '03. Shortcuts'
date = 2025-03-28
draft = false
featured_image = "https://raw.githubusercontent.com/elecbrandy/freshpink/gh-pages/basic.png"
tags = ['tag_b']
+++

<br>

## Index-title
____
This shortcut is made separately for insertion at the top of each page _index.md. It's just for the theme, so maybe you won't have to use it personally. The instructions are as follows, and basically, a line is inserted at the bottom.

### Example

``` html
{{</* index-title */>}}placeholder{{</* /index-title */>}}
```

{{<index-title>}}placeholder{{</index-title>}}


<br>
<br>

## Github log img
____
With this feature, you can attach images to your GitHub account's commit and push logs. The account is specified in the githubUsername part of the `hugo.toml` file. and If we wanted to change the colorset for this image, we could go into /layouts/shortcodes/githubcommit.html and just change the color code in the middle (the part `here!!!`).

### Setting user name
``` toml
[params]
	githubUsername = "your_username"
```

### Set color
```html
<div class="commit">
	<img src="https://ghchart.rshah.org/here!!!/{{ .Site.Params.githubUsername }}"/>
</div>
```

### Example
``` html
{{</* githubcommit */>}}
```

{{<githubcommit>}}

<br>
<br>

## Series.html
____
Sometimes there are articles that are difficult to categorize using tags alone. In this case, I wanted to organize certain articles into a series, for example, the “freshPink.” Creating a series would make it easier to manage related articles in one place. Adding a collapsible list-like link to each freshPink-specific markdown file would make it easier to jump from article to article, and organize the series.  

<br>

### Setting

<br>

> Create a Series Data File

First, you need to create a data file that contains the information about the documents in each series. Create a YAML file under Hugo’s `data*/` folder to manage the series information..

Example: `data/series/freshPink.yaml`

``` yaml
title: "freshPink"
items:
  - name: "01. freshPink"
    link: "shpink/posts/post-1"
  - name: "03. features"
    link: "https://elecbrandy.github.io/freshpink/posts/post-2"
  - name: "03. shortcuts"
    link: "https://elecbrandy.github.io/freshpink/posts/post-3"
```

In this file, the `items` list includes the name and link of each document that belongs to the series.

<br>

> Create the Shortcode File

To display the series in a markdown file, you can use the shortcode like this:

``` markdown
{{</* series title="📚 /freshPink tutorial" series="freshPink" */>}}
```

- `title`: This will be the title that users can click to expand the list.
- `series`: Refers to the YAML file name inside the `data/series/` directory (without the file extension).

<br>

### Example
When you include that code in your markdown file, the following collapsible list will be generated:

{{< series title="📚 /freshPink tutorial" series="freshPink" >}}

<br>
<br>
