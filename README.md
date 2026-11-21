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

- [x] Remove the concept bar at the top of `index.html`
- [x] Remove `<meta name="robots" content="noindex, nofollow">` from `index.html`
- [x] Delete the `[[headers]]` noindex block in `netlify.toml`
- [ ] Send test quote requests through the live form (markup is wired for Netlify Forms; confirm both inboxes get the email)
- [ ] Replace every `[bracketed]` placeholder (all remaining ones are inside hidden sections, so visitors cannot see them)
- [ ] Add artcraftsports.com in Netlify (external DNS), then update the A and www CNAME records at GoDaddy (DNS is on GoDaddy nameservers; Wix only hosts the old site). Leave MX/TXT records alone: email runs on Microsoft 365
- [ ] Confirm HTTPS is active in Netlify
- [ ] Update the Google Business Profile address
- [ ] Cancel the Wix site plan only after a week live

## Launch assumptions (Nov 21, 2026)

Set without owner confirmation. Change the site if any turn out wrong.

- Shop address: 2525 E Thomas Rd, Phoenix, AZ 85016
- Turnaround: about 3 weeks after proof approval
- Minimum order: $100
- Pickup only; shipping on the customer's carrier account
- Quote requests go to wil@artcraftsports.com and getharbingerconsulting@gmail.com (set in Netlify form notifications)
- Department price sheets are costs; website prices use a 50% margin (cost x 2)
- Garment costs are still samples, so the estimate shows decoration only and garments are "priced on your quote". Load real SanMar costs in private/costs.json, set "sample" to false and re-run the build script to switch garment prices on
- Hidden until content exists: Our Work, Our Story, customer logos and review, jacket FAQ, recent-work tiles on the Who We Serve pages
- Netlify: Free plan to start, up to $20/month approved if needed
