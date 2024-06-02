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

### Configurations

* `hugo.yaml` is the configuration file
* Follow https://adityatelange.github.io/hugo-PaperMod/posts/papermod/papermod-features/