# Syntheos — Corporate Preview Site

Static landing page for Syntheos Ltd. Hosted on GitHub Pages.

## Deploy

```bash
git init
git add .
git commit -m "Initial Syntheos corporate site"
gh repo create syntheos-site --public --source=. --push
```

Enable GitHub Pages: **Settings → Pages → Source: Deploy from branch → main → / (root)**

## Custom domain (syntheos.site)

1. DNS at your registrar — add these records:

```
A     @    185.199.108.153
A     @    185.199.109.153
A     @    185.199.110.153
A     @    185.199.111.153
CNAME www  YOUR_USERNAME.github.io
```

2. In repo: **Settings → Pages → Custom domain** → enter `syntheos.site` → Save.

3. Enable **Enforce HTTPS** once DNS propagates.
