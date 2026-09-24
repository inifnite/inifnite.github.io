# Professional portfolio

A minimal static portfolio matching the approved charcoal-and-amber design.
It uses HTML, CSS, system fonts, and a small local SVG. No JavaScript, build step,
package installation, external font request, analytics, or paid service is needed.

## Open it locally

Open `index.html` in a browser, or run this from this folder:

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Visit <http://127.0.0.1:4173>. Stop the server with Ctrl+C.

## Files

```text
professional-portfolio/
  index.html          Content and page structure
  styles.css          Theme, layout, mobile, and print styles
  assets/favicon.svg  Browser icon
  .nojekyll           Disable Jekyll processing on GitHub Pages
  .gitignore          Keep local artifacts and résumé documents out of Git
  README.md
```

## Personalize

The content now uses the reference profile provided in the conversation, including
its roles, dates, research paper, project, education, skills, and sample contact
details. It is draft content to edit, not independently verified biographical or
publication information. The employer and institute names are anonymized labels.
No separate résumé file or raw résumé transcript has been created.

Edit `index.html` to:

1. Replace **Your Name** in the title, wordmark, accessible link label, and hero.
2. Replace the employer and institute labels and review the roles, dates,
   contributions, degree, GPA, project, and numerical claims.
3. Confirm the RBAC paper title and publication details; add its actual URL.
4. Add the analytics project's repository or demo URL if you want one shown.
5. Replace the sample email and phone number. Add real LinkedIn and GitHub URLs
   in place of the non-clickable profile placeholders.
6. Update the description metadata and remove **Draft · Reference profile** once
   the page contains confirmed details.

The unknown profile URLs remain text placeholders. Email and phone use `mailto:`
and `tel:` links with the supplied sample details. Native expandable sections
hold the longer role, research, and project descriptions without JavaScript.
Navigation, **Explore my work**, and **Back to top** are functional anchor links.
The page supports keyboard focus, a skip link, reduced motion, mobile layouts,
and a light print layout. CSS theme variables are at the top of `styles.css`.

## Publish on GitHub Pages when ready

No repository has been created and nothing has been published by this project.
GitHub Pages supports free hosting from a **public repository** using its default
`github.io` address. A custom domain is optional and may cost money.

1. Create a public repository such as `portfolio` or `YOUR-USERNAME.github.io`.
2. Upload the **contents of this folder** into the repository root, so that
   `index.html`, `styles.css`, and `assets/` are at the root. Do not upload the
   parent Portfolio workspace or its design explorations.
3. Open **Settings → Pages → Build and deployment**.
4. Select **Deploy from a branch**, the branch containing these files (usually
   `main`), and **`/(root)`**, then save.
5. Wait for GitHub's deployment. The Pages settings will display the published URL.

For a repository named `portfolio`, the usual address is
`https://YOUR-USERNAME.github.io/portfolio/`. A repository named exactly
`YOUR-USERNAME.github.io` is served at `https://YOUR-USERNAME.github.io/`.
All asset paths are relative, so either URL structure works. Subsequent commits
to the selected branch update the site automatically.

If instead you publish from the parent workspace repository, GitHub's branch
publisher cannot select an arbitrary `professional-portfolio` folder. Use this
folder as the separate repository root as described above, or explicitly
configure a GitHub Actions deployment with this directory as its artifact.

[Official GitHub Pages setup documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
