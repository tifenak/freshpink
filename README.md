# freshPink – Hugo Theme

<img src="https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/tn.png" width="600">
<img src="https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png" width="600">

Welcome to the **freshPink** theme! A clean and minimalist theme for [Hugo](https://gohugo.io/), designed to give your blog a fresh look.

<br>

> [!NOTE] 
> Hugo **v0.110+ extended**  

<br>

## 🚀 Updates — 2025.09.07

We’ve added new customization options to make your site more flexible and personalized!

### Theme & Display
- **`primaryColor`**: Set your theme’s primary color (hex code). ex: `"#fa8b84"`.
- **`math`**: Enable or disable math rendering with KaTeX (`true` / `false`).

### 🖼️ Main Image
- **`mainImageUrl`**: URL of the main image shown on the homepage.  
- **`showMainImage`**: Toggle the main image on or off (`true` / `false`).

### 📊 GitHub Contribution Graph
- **`githubUsername`**: Your GitHub username (used to fetch the contribution graph).  
- **`showGithubChart`**: Show or hide the GitHub contributions chart on the homepage (`true` / `false`).

### 🔖 Site Metadata
- **`googleAnalytics`**: Your Google Analytics tracking ID (e.g., `"G-000000000"`).  
- **`copyright`**: Footer copyright.

### Example `hugo.toml`
```toml
[params]
  # --- Site Metadata ---
  googleAnalytics = "G-000000000"
  copyright = "Copyright © 2024 elecbrandy"

  # --- Theme & Display Settings ---
  primaryColor = "#fa8b84"
  math = true

  # --- GitHub Chart ---
  githubUsername = "elecbrandy"
  showGithubChart = true

  # --- Main Image ---
  mainImageUrl = "https://i.imgur.com/URQWyyY.png"
  showMainImage = true
```

<br>
<br>

## Demo Site

Check out the [**Demo Site**](https://elecbrandy.github.io/freshpink/) for an example and detailed instructions.  

This guide walks you through applying the freshpink theme to a new Hugo site using **Hugo Modules** — the recommended modern way to manage themes.

<br>

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

Replace `yourname/myblog` with your GitHub path (or any unique identifier).
That means the repository address that you will host through GitHub. In my case, I made it `hugo mod init github.com/elecbrandy/elecbrandy.github.io`.

<br>

## 3. Update `hugo.toml`

Open the generated `hugo.toml` file and **replace its contents completely** with the configuration below. Then, update it with your own information:

* `baseURL`: Enter the URL of your GitHub repository (e.g. `https://elecbrandy.github.io/`)
* `title`: Choose the name you want for your blog
* `githubUsername`: Your GitHub username — this is required to display your contribution graph (grass) on the homepage
* `googleAnalytics`: (Optional) If you want to use Google Analytics, add your tracking ID here
* Important: **Do not add or define a `theme` field.** We're using Hugo Modules to manage the theme, so this must be left out.

``` toml
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
  googleAnalytics   = "G-000000000"   # Your Google Analytics tracking ID
  primaryColor      = "#ec42ff"     # Primary theme color (hex code)
  githubUsername    = "elecbrandy"    # GitHub username for contribution chart
  showGithubChart   = true            # Set to true to display the GitHub contributions chart
  math = true
  copyright = 'Copyright © 2024 elecbrandy'

[taxonomies]
  tag = 'tags'

[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      unsafe = true
```

<br>

## 4. Download the Theme

```bash
hugo mod tidy
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

Then open (local check) -> [http://localhost:1313](http://localhost:1313)

You should see your blog styled with the **freshpink** theme! 🎉
