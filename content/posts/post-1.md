+++
title = '01. freshPink'
date = 2024-01-01
draft = false
featured_image = "https://raw.githubusercontent.com/ElecBrandy/freshpink/gh-pages/basic.png"
tags = ['tag_a']
+++

<br>

## freshPink
____
![Thumbnail](https://raw.githubusercontent.com/ElecBrandy/freshpink/main/images/tn.png)  
![Screenshot](https://raw.githubusercontent.com/elecBrandy/freshpink/main/images/screenshot.png)

Hello! Let me introduce the **freshPink** theme!

<br>
<br>

## Demo Site
____
Check out the [Demo Site](https://elecBrandy.github.io/freshpink/) for a simple example and detailed tutorial.

<br>
<br>

## Getting Started with freshPink
____
This guide explains how to install and apply the theme using **Hugo Modules** (recommended). Follow these steps to get your blog up and running:

### 1. Create a New Hugo Site

Open your terminal and run:

```bash
hugo new site my-blog
cd my-blog
```

### 2. Initialize Hugo Modules

Initialize your Hugo site as a module by running:

```bash
hugo mod init github.com/yourname/my-blog
```

### 3. Configure Your Site

Open your `hugo.toml` file and customize it to match your site. For example:

```toml
baseURL = "https://yourusername.github.io/your-repo-name/"
title = "My Awesome Blog"
canonifyURLs = true
relativeURLs = false
```

- **baseURL**: Set this to the URL of your GitHub Pages site (usually in the format `https://username.github.io/repo-name/`).
- **title**: Choose a name for your blog.
- Make sure the `baseURL` matches the repository name you use for GitHub Pages.

### 4. Add freshPink as a Hugo Module

In the same `hugo.toml` file, add the following section to import the theme:

```toml
[module]
  [[module.imports]]
    path = "github.com/ElecBrandy/freshpink"
```

### 5. Download the Theme Module

Run this command in your terminal to download the theme:

```bash
hugo mod get github.com/ElecBrandy/freshpink
```

### 6. Run Your Site

Finally, run the Hugo server:

```bash
hugo server
```

Open your browser and visit [http://localhost:1313](http://localhost:1313) to see your site with the freshPink theme applied.

<br>
<br>

## Keeping the Theme Up to Date
____
To update the theme to the latest commit in the future, run:

```bash
hugo mod get -u github.com/ElecBrandy/freshpink
```

If you encounter any cache issues, you can clean up Hugo Modules with:

```bash
hugo mod clean
```

<br>
<br>

## Need Help?
____
If you have any issues or questions, please feel free to open an issue on the [GitHub repository](https://github.com/ElecBrandy/freshpink/issues).

Thank you for choosing the freshPink theme! Enjoy your blogging experience!