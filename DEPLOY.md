# GitHub Pages deploy checklist

If your Pages link shows a **GitHub 404 page** (not a map tile 404), this is usually a publishing/config issue.

## 1) Repo requirements
- Repo must exist and be accessible.
- If repo is private, your plan must support private Pages.

## 2) Pages settings
- Go to **Settings → Pages**.
- Under **Build and deployment**:
  - Source: **Deploy from a branch**
  - Branch: **main**
  - Folder: **/(root)**
- Click **Save**.

## 3) Wait for publish
- First publish can take 1–5 minutes.
- Check **Actions** tab for a failed Pages deployment.

## 4) Confirm file paths
- `index.html` must be committed at repo root.
- Optional safety files included in this repo:
  - `.nojekyll`
  - `404.html` (redirects to `index.html`)

## 5) Correct URL format
For a project repo:
- `https://<username>.github.io/<repo-name>/`

For a user/org site repo named exactly `<username>.github.io`:
- `https://<username>.github.io/`

## 6) Custom domain
If using a custom domain:
- Add DNS records exactly as GitHub Pages docs specify.
- In Pages settings, verify the domain and HTTPS cert status.
- DNS changes can take up to 24 hours.
