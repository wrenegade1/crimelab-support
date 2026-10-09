# Crime Lab — Support Site

Static one-page support site hosted on GitHub Pages. Used as the Support URL for the App Store listing.

Live URL (after enabling Pages): `https://wrenegad3.github.io/crimelab-support/`

## Deploy

```bash
cd ~/Desktop/crimelab-support
git init
git branch -M main
git add .
git commit -m "Initial support site"
gh repo create crimelab-support --public --source=. --remote=origin --push
# Enable Pages (branch: main, folder: /)
gh api -X POST repos/wrenegad3/crimelab-support/pages -f source[branch]=main -f source[path]=/
```

Give it ~1 minute, then the URL above goes live.
