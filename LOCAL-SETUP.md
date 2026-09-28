# Personal page

Personal site adapted from https://josepmarques01.github.io/ and
https://github.com/josepmarques01/josepmarques01.github.io.
This repository starts with a clean initial commit. The original license and
template acknowledgments are preserved.

## Immediate preview

From this folder in PowerShell:

```powershell
py -m http.server 4000 --bind 127.0.0.1 --directory _site
```

Open http://127.0.0.1:4000. Press Ctrl+C to stop.
The ignored `_site` folder contains a snapshot of the published page and its
assets. Source edits require a Jekyll build before appearing in this preview.

## Edit the site

- `_pages/about.md`: biography, publications, experience, projects, and education.
- `_config.yml`: name, contact details, social links, and repository settings.
- `_data/navigation.yml`: navigation links.
- `images/github.png`: profile photograph.
- `_sass/` and `assets/css/main.scss`: styling.

## Preview source changes

Ruby and Bundler are not currently available on PATH. After installing Ruby
with development tools and Bundler, run from this folder:

```powershell
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4000
```

Stop the snapshot server first if it is running. Jekyll rebuilds `_site` from
the source. Restart Jekyll after changing `_config.yml`.

## Publishing

This is a personal repository, separate from AIM-SKKU:
https://github.com/jmarques01/jmarques01.github.io.

The `origin` remote and the `repository` setting in `_config.yml` point to
`jmarques01/jmarques01.github.io`. GitHub Pages builds the Jekyll source from
`main` and publishes it
at https://jmarques01.github.io/. The local `_site` snapshot is not committed.
