# Tools

**Generator**: hugo v0.124.1
**Theme**: https://adityatelange.github.io/hugo-PaperMod/ (Installed `31st March 2024`)

# Setup

### Initiate the site
```
mkdir teleported.in
cd teleported.in
hugo new site . --format yaml
ls
```

### Install the theme
```
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)
```

Open `hugo.yaml` and set the theme

```
theme: ["PaperMod"]

```

Now edit out the contents of the file `teleported.in/themes/PaperMod/layouts/partials/home_info.html` so as not hide the unnecessary banner.

### Create the about page
From within the `teleported.in` directory

Create:
```
hugo new about.md
```

Edit:
```
content/about.md
```

Configure `hugo.yaml`:
```
menu:
  main:
    - identifier: "about"
      name: "About"
      url: "/about/"
      weight: 2

```

Build and publish

### Writing a new post
From within the `teleported.in` directory

Create a new post:
```
hugo new content posts/my-first-post.md
```

Edit the post:
```
vim content/posts/my-first-post.md
```
Guidelines on the layout are here:

```
hugo serve
```


### Publish

From within the `teleported.in` directory

```
hugo
```

```
cp public/* ..
```

### Configurations

* `hugo.yaml` is the configuration file
* Follow https://adityatelange.github.io/hugo-PaperMod/posts/papermod/papermod-features/