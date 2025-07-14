# 📝 My Hugo Blog – `mysite`

Static site built with [Hugo](https://gohugo.io/) and deployed to GitHub Pages.

---

## 🚀 Quick Workflow

### ✅ Create a New Post

```sh
cd mysite
hugo new posts/example.md
```

> ✏️ Edit the front matter (`draft: true` → `draft: false`) to make it visible.

---

### 🔧 Run Local Dev Server

```sh
hugo server -D
```

> Visit: [http://localhost:1313](http://localhost:1313)
Visit: [http://localhost:1313/arslankhanali/mysite/](http://localhost:1313/arslankhanali/mysite/)
---

### 📤 Publish to GitHub

```sh
git add -A
git commit -m "Create hugo.yaml"
git push
```
See progress [https://github.com/arslankhanali/mysite/actions](https://github.com/arslankhanali/mysite/actions)  
Live site: [https://arslankhanali.github.io/mysite/](https://arslankhanali.github.io/mysite/)

---

## 🛠️ Setup from Scratch

### 1. Install Hugo (macOS)

```sh
brew install hugo
hugo new site mydocs; cd mydocs
git init
git submodule add https://github.com/alex-shpak/hugo-book themes/hugo-book
cp -R themes/hugo-book/exampleSite/content.en/* ./content
```

## 🔃 Git Setup

```sh
echo "# mysite" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/arslankhanali/mysite.git
git push -u origin main
```

---

## 🎨 Add a Hugo Theme

Pick one theme and set it in `hugo.toml`.

1. Ananke

```sh
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> hugo.toml
```

2. Paper

```sh
git submodule add https://github.com/nanxiaobei/hugo-paper themes/paper
echo "theme = 'paper'" >> hugo.toml
```
3. Hugo Book
```sh
git submodule add https://github.com/alex-shpak/hugo-book.git themes/hugo-book
echo "theme = 'paper'" >> hugo.toml
```
---

## 📦 Deploy to GitHub Pages

Follow: [https://gohugo.io/host-and-deploy/host-on-github-pages/](https://gohugo.io/host-and-deploy/host-on-github-pages/)

---

## 🧼 Tips

- To switch themes, edit `hugo.toml` and restart server
- To update submodules: `git submodule update --remote`
- Draft posts are hidden unless you run `hugo server -D`
