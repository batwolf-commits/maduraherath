# Madura Bhathiya Herath — Personal Portfolio

Personal and academic portfolio of **Madura Bhathiya Herath**, a Business Analyst
and HCI/UX researcher based in Sweden. Built with [Jekyll](https://jekyllrb.com/)
using the [al-folio](https://github.com/alshedivat/al-folio) theme.

**Live site:** https://batwolf-commits.github.io/maduraherath/

## What's here

- **About** — background, research interests, and contact.
- **Publications** — papers and academic writing.
- **Projects** — selected research and applied work.
- **Dev Projects** — software I build, including [LeftSpace](https://github.com/batwolf-commits/leftspace), a native macOS storage cleaner.
- **CV** — full curriculum vitae.
- **Blog & News** — occasional writing and updates.

## Local development

```bash
bundle install          # install Ruby gems
npm install             # install Node dependencies
bundle exec jekyll serve
```

The site is then available at `http://localhost:4000/maduraherath/` (note the
`baseurl`).

To produce a production build:

```bash
bundle exec jekyll build --baseurl /maduraherath
```

## Editing content

Pages live in `_pages/`, posts in `_posts/`, and site-wide settings (name, title,
navigation, plugins) in `_config.yml`. Layouts, styles, and runtime behavior come
from the versioned al-folio plugin gems, so content edits stay in this repo.

## Deployment

Pushing to `main` triggers the **Deploy site** GitHub Actions workflow, which
builds the site and publishes it to GitHub Pages.

## License

Content © Madura Bhathiya Herath. The underlying theme is
[al-folio](https://github.com/alshedivat/al-folio), released under the MIT License.
