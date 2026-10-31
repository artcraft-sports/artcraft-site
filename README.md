# artcraftsports.com

Website for Artcraft Sports Apparel (Phoenix, est. 1953, veteran owned).

Plain HTML, no build step. Netlify publishes this repo automatically:

- Push to `main` → live site updates in about a minute.
- Open a pull request → Netlify posts a **Deploy Preview** link to share before merging.

## Edit and publish

```powershell
git pull
# edit index.html in VS Code
git add .
git commit -m "What changed"
git push
```

## Launch checklist

- [ ] Remove the concept bar at the top of `index.html`
- [ ] Remove `<meta name="robots" content="noindex, nofollow">` from `index.html`
- [ ] Delete the `[[headers]]` noindex block in `netlify.toml`
- [ ] Wire the quote form to Netlify Forms and send test requests
- [ ] Replace every `[bracketed]` placeholder
- [ ] Add artcraftsports.com in Netlify (external DNS), then update the A and www CNAME records at Wix. Leave MX/TXT (email) records alone
- [ ] Confirm HTTPS is active in Netlify
- [ ] Update the Google Business Profile address
- [ ] Cancel the Wix site plan only after a week live (keep the domain registration)
