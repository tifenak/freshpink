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
![tn.png](https://raw.githubusercontent.com/ElecBrandy/freshpink/main/images/tn.png)
![screenshot.png](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png)

Hello! Let me introduce the **freshPink** theme!  

<br>

## Demo Site
____
Here is the demo site where you can find a simple example and a detailed tutorial.
[Go to Demo site](https://elecbrandy.github.io/freshpink/).

<br>
<br>

## Getting Started with freshpink
____

> This guide explains how to install and apply the theme using **Hugo Modules** (recommended).

#### 1. Create a New Hugo Site

```bash
hugo new site my-blog
cd my-blog
```

#### 2. Initialize Hugo Modules

```bash
hugo mod init github.com/yourname/my-blog
```

#### 3. Configure the Theme
Open your `hugo.toml` file and customize it to match your site. For example:

```toml
baseURL = "https://yourusername.github.io/your-repo-name/"
title = "My Awesome Blog"
```

- `baseURL`: Set this to the URL of your GitHub Pages site (usually `https://username.github.io/repo-name/`).
- `title`: Choose any name you want to appear as your blog title.

Make sure this `baseURL` matches the **repository name** you're using for GitHub Pages.

#### 4. Run Your Site

```bash
hugo server
```
Visit `http://localhost:1313` in your browser :)

<br>
<br>

## Update theme
____

#### Keeping the Theme Up to Date

```bash
hugo mod get -u github.com/elecBrandy/freshpink
```

#### Optional: Clean Up Hugo Modules Cache

If you face any cache issues

```bash
hugo mod clean
```

<br>
<br>

## Need Help?
____

If you encounter any issues or have questions, feel free to open an issue on the [GitHub repository](https://github.com/ElecBrandy/freshpink/issues).

Thank you for choosing the freshPink theme! :)
