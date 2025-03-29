+++
title = '01. freshPink'
date = 2024-01-01
draft = false
featured_image = "https://raw.githubusercontent.com/ElecBrandy/freshpink/gh-pages/basic.png"
tags = ['tag_a']
+++

<br>

## Getting Started
____

To begin using freshPink for your development blog, follow the installation and customization instructions available on our [_GitHub repository_](https://github.com/your-repo/freshpink-hugo-theme). Dive into the world of blogging with a theme that's as dynamic and vibrant as your ideas.

<br>

### Demo Site
Here is the demo site where you can find a simple example and a detailed tutorial.  
[_Go to Demo site_](https://elecbrandy.github.io/freshpink/)

<br>

### Installation
There are two methods to install the freshPink theme. You can either use Git submodules (recommended for easy updates) or download it directly. Unless there's a specific reason, we recommend using the submodule method.  

<br>

> Method 1: Install via Git Submodule (Recommended)

1. **Navigate to Your Hugo Site Directory**:
   Open a terminal and navigate to the root directory of your Hugo site. If you haven’t created a Hugo site yet, you can do so with the following command:

```bash
hugo new site yourSiteName
```

2. **Add Theme as a Git Submodule**:
   Add the freshPink theme to your site as a Git submodule. Run the following command in the terminal:

```bash
git submodule add git@github.com:ElecBrandy/freshpink.git themes/freshpink
```

3. **Update Site hugouration**:
   Open your site’s `hugo.toml` file in a text editor and update the `theme` variable to `"freshpink"`:

```toml
theme = "freshpink"
```

4. **Preview Your Site**:
   To ensure everything works correctly, run the following command to start the local server and preview your site:

```bash
hugo server
```

<br>
<br>

> Method 2: Download and Install Manually

1. **Download the Theme**:
   Go to the [FreshPink GitHub repository](https://github.com/ElecBrandy/freshpink) and download the theme as a ZIP file.

2. **Extract and Move the Theme**:
   Extract the ZIP file and move the extracted folder to the `themes` directory in your Hugo site.

3. **Update Site hugouration**:
   Just like with the Git submodule method, open your `hugo.toml` file and set the `theme` variable to `"freshpink"`.

4. **Preview Your Site**:
   Run the following command to build and preview your site locally:

```bash
hugo server
```

<br>
<br>

## Customizing the Theme
____
The freshPink theme is designed to be easily customizable. You can modify the styles, layouts, and content as needed to fit your site. Follow the tutorial on the demo site and try customizing it yourself!

<br>
<br>

## Need Help?
____
If you encounter any issues or have questions, feel free to open an issue on the [GitHub repository](https://github.com/ElecBrandy/freshpink/issues).

<br>
<br>
