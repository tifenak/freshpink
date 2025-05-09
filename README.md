# freshPink

![Thumbnail](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/tn.png)  
![Screenshot](https://raw.githubusercontent.com/elecbrandy/freshpink/main/images/screenshot.png)

Hello! Let me introduce the **freshPink** theme!

<br>
<br>

## Demo Site

Check out the [_Demo Site_](https://elecbrandy.github.io/freshpink/) for a simple example and detailed tutorial.

<br>
<br>


This guide walks you through applying the [`freshpink`](https://github.com/ElecBrandy/freshpink) theme to a new [Hugo](https://gohugo.io/) site using **Hugo Modules** — the recommended modern way to manage themes.

---

## ✅ Prerequisites

- Hugo **v0.110+ extended**  
- Git installed  
- Terminal (macOS/Linux/WSL)  

Check your Hugo version:

```bash
hugo version
````

---

## 1️⃣ Create a New Hugo Site

```bash
hugo new site myblog
cd myblog
```

---

## 2️⃣ Initialize Hugo Modules

```bash
hugo mod init github.com/yourname/myblog
```

> Replace `yourname/myblog` with your GitHub path (or any unique identifier).

---

## 3️⃣ Update `hugo.toml`

Open the generated `hugo.toml` and **replace or edit** it like this:

```toml
baseURL = "https://example.org/"
title = "My Freshpink Blog"
languageCode = "en-us"

[params]
  author = "Your Name"
  description = "A Hugo blog using the freshpink theme"

[module]
  [[module.imports]]
    path = "github.com/ElecBrandy/freshpink"
```

> ❗ **Do not add `theme = "freshpink"`** — it's unnecessary with Modules and will cause errors.

---

## 4️⃣ Download the Theme

```bash
hugo mod tidy
```

> 💡 If you see an error like
> `could not read Username for 'https://github.com': terminal prompts disabled`,
> try running:

```bash
git config --global url."git@github.com:".insteadOf "https://github.com/"
```

---

## 5️⃣ Create Your First Post

```bash
hugo new posts/hello.md
```

Then edit the file at `content/posts/hello.md` and:

* Set `draft: false`
* Add some content

---

## 6️⃣ Run the Local Server

```bash
hugo server -D
```

Then open: [http://localhost:1313](http://localhost:1313)

You should see your blog styled with the **freshpink** theme! 🎉

---

## 🔧 Optional Next Steps

* 🧭 Add navigation menus: use `[menu]` config blocks
* 🌐 Deploy to GitHub Pages, Netlify, or Vercel
* 🎨 Customize the theme using `layouts/` and `assets/` overrides

---

## 📌 Credits

* Theme: [github.com/ElecBrandy/freshpink](https://github.com/ElecBrandy/freshpink)
* Guide maintained by [@yourname](https://github.com/yourname)

---

```

---

필요하면 `.md` 파일로 따로 만들어드릴 수도 있고, 메뉴나 다크모드 설명을 추가해 확장된 버전도 제작해드릴 수 있어요. 그대로 쓸까요, 아니면 포맷이나 내용 수정해드릴까요?
```
