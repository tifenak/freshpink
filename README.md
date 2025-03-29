# freshPink

![tn.png](https://raw.githubusercontent.com/ElecBrandy/freshpink/main/images/tn.png)
![screenshot.png](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png)

Hello! Let me introduce the **freshPink** theme!  

<br>

## Demo Site
Here is the demo site where you can find a simple example and a detailed tutorial.
[Go to Demo site](https://elecbrandy.github.io/freshpink/).


## Getting Started with freshpink

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

Open `hugo.toml` and add the following

``` toml
baseURL = "https://yourname.github.io/"
languageCode = "en-us"
title = "My Blog"
canonifyURLs = true

theme = "github.com/elecBrandy/freshpink"

[module]
  [[module.imports]]
    path = "github.com/elecBrandy/freshpink"

[taxonomies]
  tag = "tags"

[markup]
  [markup.goldmark]
    [markup.goldmark.renderer]
      unsafe = true
```

#### 4. Run Your Site

```bash
hugo server
```
Visit `http://localhost:1313` in your browser :)



#### 5. Keeping the Theme Up to Date

```bash
hugo mod get -u github.com/elecBrandy/freshpink
```

#### 6. Optional: Clean Up Hugo Modules Cache

If you face any cache issues

```bash
hugo mod clean
```

## Need Help?
If you encounter any issues or have questions, feel free to open an issue on the [GitHub repository](https://github.com/ElecBrandy/freshpink/issues).

Thank you for choosing the freshPink theme! :)
