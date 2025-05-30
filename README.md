# spsarkar.github.io

## Setup Instructions

This site uses [Jekyll](https://jekyllrb.com/) with the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme.

### Prerequisites

- Ruby ([installation guide](https://www.ruby-lang.org/en/documentation/installation/))
- Bundler (`gem install bundler`)

### Local Development

1. Install dependencies:

   ```sh
   bundle install
   ```

2. Serve locally:

   ```sh
   bundle exec jekyll serve
   ```

3. Visit `http://localhost:4000` in your browser.

### Deployment

Push your changes to the `main` branch of your GitHub repository. GitHub Pages will build and deploy your site automatically.

---

## Directory Structure

- `_config.yml`: Site configuration
- `Gemfile`: Ruby dependencies
- `_pages/`: Custom pages (e.g., home)
- `_posts/`: Blog posts
- `.gitignore`: Ignore build and cache files

---

For more customization, see the [Minimal Mistakes documentation](https://mmistakes.github.io/minimal-mistakes/docs/).
