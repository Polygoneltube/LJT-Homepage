# LJT-Homepage

Personal academic homepage for Junteng Liu, built with the [Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll template and customized using only the profile information available in the connected memory store.

The site is intentionally limited to:

- An About/home page with academic background, research experience, skills and research themes, honors, contact details, and the complete publication list.
- A dedicated Publications page containing the same six publications.
- A contact anchor in the About/home page.

The navigation contains only About, Publications, and Contact. Inherited template demo pages, sample collections, and sample files are removed by the publish workflow's cleanup step before the static site is built and deployed to the `gh-pages` branch.

## Local development

```bash
bundle install
bundle exec jekyll serve --baseurl "/LJT-Homepage"
```

Then open `http://localhost:4000/LJT-Homepage/`.

## Deployment

The manual **Build and publish LJT-Homepage** workflow in `.github/workflows/site-check.yml` builds the site with `--baseurl /LJT-Homepage`, removes inherited sample content in the runner and commits those source cleanups back to `master`, then replaces the `gh-pages` branch with the generated `_site` output.
