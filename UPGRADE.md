# Upgrading Jekyll Plugins and Minimal Mistakes Theme

This guide explains how to upgrade the Jekyll plugins and the Minimal Mistakes Jekyll theme for your GitHub Pages site.

---

## 1. Update the Gemfile

Open your `Gemfile` and update the version numbers for the plugins and theme if you want to target a specific version. To always get the latest, you can remove version numbers:

```
gem "github-pages", group: :jekyll_plugins
gem "minimal-mistakes-jekyll"
```

---

## 2. Update Dependencies

Run the following command to update all gems (including Jekyll, plugins, and the theme):

```sh
bundle update
```

This will update the `Gemfile.lock` file with the latest compatible versions.

---

## 3. Test Your Site Locally

After updating, serve your site locally to ensure everything works:

```sh
bundle exec jekyll serve
```

Visit `http://localhost:4000` and check for errors or warnings in the terminal.

---

## 4. Commit and Push Changes

If everything works as expected, commit the updated `Gemfile` and `Gemfile.lock` files:

```sh
git add Gemfile Gemfile.lock
```

```sh
git commit -m "Upgrade Jekyll plugins and Minimal Mistakes theme"
git push
```

---

## 5. Additional Resources

- [Minimal Mistakes Upgrade Guide](https://mmistakes.github.io/minimal-mistakes/docs/upgrading/)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Dependency Versions](https://pages.github.com/versions/)

---

**Tip:** If you use GitHub Pages' default build, it will use the version of Jekyll and plugins specified by GitHub. For more control, use GitHub Actions or a custom build process.
