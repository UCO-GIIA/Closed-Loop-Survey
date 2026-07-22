# Closed-loop edge configurator — GitHub Pages package

This package contains a static, client-side HTML configurator for the article:

**Closed-Loop Data Reduction for Edge Time-Series: A Design-Oriented Survey**

## Files

- `index.html`: standalone HTML/CSS/JavaScript configurator.
- `.nojekyll`: disables Jekyll processing in GitHub Pages.

## Recommended deployment with GitHub Pages

1. Create a public GitHub repository, for example:
   `closed-loop-edge-configurator`
2. Upload `index.html` and `.nojekyll` to the root of the repository.
3. Go to **Settings > Pages**.
4. Under **Build and deployment**, select:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Save and wait for GitHub Pages to publish the site.

The resulting URL will normally have this form:

```text
https://<github-user-or-organization>.github.io/closed-loop-edge-configurator/
```

Use that URL in the LaTeX macro:

```latex
\newcommand{\configuratorurl}{https://<github-user-or-organization>.github.io/closed-loop-edge-configurator/}
```

## WordPress note

The configurator uses inline JavaScript, browser-side state, and JSON import/export. Some WordPress configurations sanitize or block inline scripts and event handlers when HTML is inserted inside a page or post. Hosting it as a standalone static page avoids that problem.
