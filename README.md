# homepage

Personal site for opanmustopah.com: posts and projects. Built with
[Hugo](https://gohugo.io) v0.169.0 and a small theme in `layouts/` (no
third-party theme).

## Run

```bash
hugo server -D        # http://localhost:1313, -D shows drafts
hugo --gc --minify    # build into public/
```

## Write

- **Post:** `hugo new posts/my-post.md`, write Markdown, remove `draft: true`.
  For a post with images, make a folder instead (`content/posts/my-post/index.md`
  with the images next to it) and use `{{< figure src="photo.jpg" caption="…" >}}`.
- **Project:** add `content/projects/<name>/index.md` with `title`, `tagline`,
  `weight` (order), `live`, `repo`, `stack`, and a `cover.png` screenshot.
- **About text:** `content/_index.md`. Avatar: `assets/images/avatar.jpg`.

## Layout

| Path | |
|---|---|
| `layouts/baseof.html` | page shell: head, nav, footer |
| `layouts/home.html` | intro, latest posts, projects |
| `layouts/page.html`, `section.html` | posts and generic pages |
| `layouts/projects/` | project cards and pages |
| `assets/css/main.css` | all styles; light/dark via `prefers-color-scheme` |
| `assets/css/syntax.css` | code highlighting, from `hugo gen chromastyles` |
