# freshPink – Hugo Theme

![Thumbnail](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/tn.png)
![Screenshot](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png)

Welcome to the **freshPink** theme! A clean and minimalist theme for [Hugo](https://gohugo.io/), designed to give your blog a fresh look.

## Demo Site

Check out the [**Demo Site**](https://elecbrandy.github.io/freshpink/) for an example and detailed instructions.

## Quick Start Guide

This guide shows you how to set up the **freshPink** theme with a new Hugo site using **Hugo Modules**, the recommended modern approach.

## Prerequisites

Before you start, ensure you have:

* Hugo **v0.110+ (extended)**
* Git installed
* Terminal access (macOS/Linux/WSL)

Check your Hugo version:

```bash
hugo version
```

## Step-by-Step Installation

### 1. Create a New Hugo Site

```bash
hugo new site myblog
cd myblog
```

### 2. Initialize Hugo Modules

```bash
hugo mod init github.com/yourusername/myblog
```

> Replace `yourusername/myblog` with your GitHub username and repository name (or any unique identifier).

### 2. Configure `hugo.toml`

Open `hugo.toml` and modify it as follows.
After copying and pasting, fill in the content according to your situation.
In particular, `[params]` -> `githubUsername = 'githubUsername` must be filled with your GitHub account so that the theme will come out normally and beautifully.

```toml
baseURL = 'https://example.org/' # your git repository address
title = 'freshpink' # your own blog title
languageCode = 'en-us'
canonifyURLs = true

[[menus.main]]
name = 'Home'
pageRef = '/'
weight = 10

[[menus.main]]
name = 'TAGS'
pageRef = '/tags/'
weight = 20

[[menus.main]]
name = 'ABOUT'
pageRef = '/about/'
weight = 30

[module]
  [module.hugoVersion]
    extended = true
    min = "0.116.0"
  [[module.imports]]
    path = "github.com/elecbrandy/freshpink"

[params]
  googleAnalytics = 'G-000000000' # your GoogleAnalytics code
  githubUsername = 'githubUsername' # your githubUsername
  copyright = 'Copyright © 2024 elecbrandy'
  math = true

[taxonomies]
  tag = 'tags'

[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      unsafe = true
```

> ⚠️ **Important:** Do **not** add `theme = "freshpink"` as this will cause errors with Hugo Modules.

### 4. Download the Theme

Run the following command:

```bash
hugo mod tidy
```

> If you encounter an error like `could not read Username for 'https://github.com'`, use SSH:

```bash
git config --global url."git@github.com:".insteadOf "https://github.com/"
```

### 5. Create Your First Post

```bash
hugo new posts/hello.md
```

Edit the file `content/posts/hello.md`:

* Change `draft: true` → `draft: false`
* Add your content

### 6. Run the Local Server

```bash
hugo server -D
```

Visit [http://localhost:1313](http://localhost:1313) in your browser.

Congratulations! Your site is now running with the **freshPink** theme! 🎉

## 📌 Credits

* Theme repository: [github.com/ElecBrandy/freshpink](https://github.com/ElecBrandy/freshpink)
* Guide maintained by [@yourusername](https://github.com/yourusername)
