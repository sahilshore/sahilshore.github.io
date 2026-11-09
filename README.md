# Sahil Khan — Personal Portfolio

A responsive, static portfolio inspired by the section flow and project storytelling of Khushi Khurana's portfolio, rewritten around Sahil Khan's own profile and projects.

## Files

```text
sahil-portfolio/
├── index.html
├── styles.css
├── script.js
├── .nojekyll
├── README.md
└── assets/
    ├── favicon.svg
    └── Sahil_Khan_Resume.pdf
```

## Run locally

No Node.js, Python backend, or build step is required.

- Open `index.html` directly in a browser, or
- From this folder, run `python -m http.server 5500` and open `http://localhost:5500`.

## Publish using GitHub Pages (recommended)

The simplest setup is a **user site** repository named exactly `sahilshore.github.io`.

1. On GitHub, create a **public** repository named `sahilshore.github.io`.
2. Extract this folder. Upload the *contents* of `sahil-portfolio` into the root of the new repository. `index.html` must be at the repository root.
3. Commit and push the files. For example, from the extracted folder in PowerShell:

   ```powershell
   git init
   git add .
   git commit -m "Add personal portfolio"
   git branch -M main
   git remote add origin https://github.com/sahilshore/sahilshore.github.io.git
   git push -u origin main
   ```

   If the repository already has a commit (for example, a README created on GitHub), clone it first and copy the site files into the cloned repository instead of running `git init` again.

4. Open the repository on GitHub and go to **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select branch **main** and folder **/(root)**, then click **Save**.
7. Wait for the Pages workflow to finish. The site address will be:

   `https://sahilshore.github.io/`

GitHub Pages is available for public repositories on GitHub Free. The site is static; it serves HTML, CSS, JavaScript, images and PDFs. It does not run Python, Flask, FastAPI, Streamlit, a database, or other server-side code.

## What to customize before publishing

- Confirm the preferred public contact email. The current version uses the personal email from `CV.pdf`.
- Replace `assets/Sahil_Khan_Resume.pdf` whenever you update your resume.
- Add live demo URLs to project cards only after the relevant app is deployed and publicly accessible. At present, project cards link to source repositories; this avoids presenting an unverified demo as live.
- Kaggle is linked, but no notebook titles or Kaggle metrics are stated because the public profile did not expose readable notebook details during preparation.
- Add a high-resolution portrait in a future revision if desired. The current hero uses a designed monogram visual rather than a low-resolution profile thumbnail.

## Contact behavior

The contact call-to-action uses a `mailto:` link. It opens the visitor's default email application; there is no server-backed contact form, database, or message collection.

## Design and interaction

- Mobile navigation menu
- Smooth anchor navigation
- Scroll progress indicator
- Reveal-on-scroll section animations
- Reduced-motion support
- Responsive layouts for desktop, tablet and mobile
