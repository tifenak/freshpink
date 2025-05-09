# freshPink – Hugo Theme

<img src="https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/tn.png" width="600">
<img src="https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png" width="600">

Welcome to the **freshPink** theme! A clean and minimalist theme for [Hugo](https://gohugo.io/), designed to give your blog a fresh look.

## Demo Site

Check out the [**Demo Site**](https://elecbrandy.github.io/freshpink/) for an example and detailed instructions.  

This guide walks you through applying the [`freshpink`](https://github.com/ElecBrandy/freshpink) theme to a new [Hugo](https://gohugo.io/) site using **Hugo Modules** — the recommended modern way to manage themes.

<br>

## Prerequisites

- Hugo **v0.110+ extended**  
- Git installed  
- Terminal (macOS/Linux/WSL)  

Check your Hugo version!

```bash
hugo version
```

<br>

## 1. Create a New Hugo Site

```bash
hugo new site myblog
cd myblog
```

<br>

## 2. Initialize Hugo Modules

```bash
hugo mod init github.com/yourname/myblog
```

> Replace `yourname/myblog` with your GitHub path (or any unique identifier).

## 3. Update `hugo.toml`

Open the generated `hugo.toml` and **replace or edit** it like this ->

```toml
baseURL = "https://example.org/"
title = "My Freshpink Blog"
languageCode = "en-us"

[params]
  author = "Your Name"
  description = "A Hugo blog using the freshpink theme"

[module]
  [module.hugoVersion]
    extended = true
    min = "0.116.0"
  [[module.imports]]
    path = "github.com/ElecBrandy/freshpink"
```

> ❗ **Do not add `theme = "freshpink"`** — it's unnecessary with Modules and will cause errors.

<br>

## 4. Download the Theme

```bash
hugo mod tidy
```

> 💡 If you see an error like
> `could not read Username for 'https://github.com': terminal prompts disabled`,
> try running:

```bash
git config --global url."git@github.com:".insteadOf "https://github.com/"
```

<br>

## 5. Create Your First Post

```bash
hugo new posts/hello.md
```
<br>

## 6. Run the Local Server

```bash
hugo server -D
```

Then open -> [http://localhost:1313](http://localhost:1313)

You should see your blog styled with the **freshpink** theme! 🎉
