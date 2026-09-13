# JobPal — General Portfolio Site

A single hand-authored static page (`index.html` + `style.css`) — not part of the JobPal app.
No database, no backend, no build step. Edit the HTML directly and publish it yourself.

This is the **one general portfolio** referenced in the app: once published, paste its URL into
your profile's **Portfolio URL** field (Profile page) so generated resumes and cover letters can
reference it.

## Editing

Open `index.html` in any editor and replace the placeholder text (marked with comments like
`<!-- Replace with your name -->`) section by section:

1. **Hero** — your name, headline, tagline, and a few standout skills as chips.
2. **About** — a short paragraph (can reuse your profile's Summary field).
3. **Projects** — copy the `<article class="project">` block once per project you want to
   showcase; alternate `class="project"` / `class="project flip"` so the layout zig-zags.
4. **Skills** — one `<div class="skill">` per skill.
5. **Experience** — copy the `<div class="jstep">` block once per job or education entry, most
   recent first.
6. **Contact** — your email, phone, GitHub, LinkedIn.

### Adding images

Put files in `assets/` and reference them, e.g.:

```html
<img class="avatar" src="assets/photo.jpg" alt="Your Name">
```

```html
<div class="shot"><img src="assets/project-1.png" alt="Project 1 screenshot"></div>
```

(replaces the `<div class="placeholder">...</div>` box in a project block).

## Previewing locally

Just open `index.html` directly in a browser — no server needed.

## Publishing to GitHub Pages

1. Push this `portfolio-site/` folder to a GitHub repository (a new repo, or a subfolder of an
   existing one — your choice).
2. In the repo's **Settings → Pages**, set the source to the branch/folder containing
   `index.html`.
3. GitHub gives you a URL like `https://yourusername.github.io/your-repo/`. Wait a minute or two
   for the first deploy.
4. Paste that URL into your JobPal profile's **Portfolio URL** field.

Re-publishing after an edit is just another commit + push — GitHub Pages redeploys automatically.
