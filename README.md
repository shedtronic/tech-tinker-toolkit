# Tech Tinker Toolkit

A friendly Hugo website for creative technology teachers, makers, students, and STEAM learners.

## Local development

1. Install Hugo 0.163.3 or newer.
2. Run:

```bash
hugo server
```

3. Open `http://localhost:1313` in your browser.

## Build the site

```bash
hugo
```

The generated site will appear in the `public/` folder.

## Deploy to Netlify

This site is prepared for Netlify deployment with `netlify.toml`.

- Build command: `hugo`
- Publish directory: `public`
- Environment: `HUGO_VERSION=0.163.3`

## Notes

This is a separate site from `soundportfolio2026` and does not include references to that project.

## Adding or updating Resources (Teachers Pay Teachers)

To add a new live Teachers Pay Teachers product card, edit `layouts/resources/list.html` and add a new `article.card` in the "Live on Teachers Pay Teachers" section. Provide the product title, short description, category tag, and a button linking to the TPT URL using `target="_blank" rel="noopener"`.

For placeholder (Coming Soon) items, add a card in the "Coming Soon" section and use a non-clickable label or a `span` with the `button` class and `aria-disabled="true"`.

Alternatively, to add a full resource page, create a markdown file under `content/resources/` with front matter including `title`, `summary`, `category`, and `level`. The site template will display resource pages automatically unless overridden by the custom layout.
