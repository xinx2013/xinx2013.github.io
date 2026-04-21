# XX-Lab Homepage

Lab homepage built with the [Allan Lab](https://github.com/mpa139/allanlab) Jekyll theme.

## Content Management

| What to change | File to edit |
|----------------|-------------|
| Home page intro | `_includes/content/home.md` |
| Openings info | `_includes/content/openings.md` |
| Publications | `_data/publist.yml` |
| News | `_data/news.yml` |
| Staff members | `_data/team_members.yml` |
| Students | `_data/students.yml` |
| Research highlights | `_data/highlights.yml` |

Member photos go in `photos/`; reference the filename in the yml file. Photos are auto-cropped to a square from the top.

Highlight images go in `images/highlights/`; reference the filename in `_data/highlights.yml`.

### Publication format

```yaml
- title: "Paper Title"
  authors: First Author, Xin Xin, and Last Author
  link:
    display: MICRO 2021
  paper: https://xxx.pdf         # optional
  slide: https://xxx-slides.pdf  # optional
```

### News format

```yaml
- date: 2026
  headline: "Paper accepted at <strong>ISCA 2026</strong>: Paper Title"
```

## Local Preview

```bash
bundle install
bundle exec jekyll serve --port 8080 --baseurl "" --host 0.0.0.0
```

## Deployment

Push to the `main` branch and GitHub Pages will build automatically.
