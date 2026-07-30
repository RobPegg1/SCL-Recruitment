# SCL Recruitment website

Static website for SCL Recruitment Ltd (www.sclrecruitment.co.uk). Plain HTML, CSS and images -- no build step, no framework.

## Structure

- `index.html` and the other `*.html` files -- one file per page
- `css/style.css` -- all styling
- `images/` -- logo, photos, social share image
- `_redirects` -- old-URL redirects (Netlify reads this automatically)
- `sitemap.xml`, `robots.txt` -- search engine files
- `netlify.toml` -- hosting config (headers, caching)

## Hosting

Hosted on Netlify, connected to this repository. Any change pushed to the `main` branch publishes automatically within a minute or so. No manual upload needed once the repo is connected.

## Making a change

Small text edits can be made directly in GitHub: open the file, click the pencil icon, edit, commit. Netlify republishes on commit.

For anything structural (new page, new article, layout change), keep the pattern consistent with the existing pages -- each page repeats the same header and footer markup and links the shared stylesheet.

## Contact form

The contact form uses Netlify Forms (`data-netlify="true"`). Form detection must be enabled in the Netlify dashboard, and submissions appear under the Forms tab. Candidate registrations use a HubSpot embedded form and land in HubSpot, not Netlify.
