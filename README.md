# 9 Planets Local Preview

This folder contains the standalone static site files for the 9 Planets design.

## Open locally

1. Open a terminal.
2. Change to this folder:

```bash
cd "/Users/allenbope/Dropbox/Bopedesign/9 Planets/Web/Claude Design download/standalone"
```

3. Start a local server:

```bash
python3 -m http.server 8000
```

4. Open your browser and go to:

```
http://127.0.0.1:8000/index.html
```

## Alternative

Run the helper script:

```bash
./serve.sh
```

Then open:

```
http://127.0.0.1:8000/index.html
```

## Deploying to Vercel

This folder can be deployed directly as a static site on Vercel.

1. Create a Git repository for this folder.
2. Connect the repo to Vercel.
3. Deploy the project as a static site.

The included files help with Vercel and SEO:

- `vercel.json` — enables clean URLs and adds basic security headers.
- `robots.txt` — tells search engines to index the site.
- `sitemap.xml` — gives search engines a list of pages to crawl.

### Quick deploy command

If you install the Vercel CLI, you can deploy directly from this folder with:

```bash
cd "/Users/allenbope/Dropbox/Bopedesign/9 Planets/Web/Claude Design download/standalone"
vercel --prod
```

### Preview page

A local preview page is available at `preview.html` if you want a quick index of all site pages before deployment.

### Important SEO preparation

For a production-ready SEO site, make sure each page has:

- a unique `<title>`
- a unique `<meta name="description">`
- a canonical URL
- structured open graph metadata for social previews
- clear page content as HTML, not only as JavaScript-rendered content

If you want the site to be fully SEO-optimized, the best approach is to convert this into a normal static site or a static-rendered framework like Next.js or Astro, instead of leaving it as a client-bundled page loader.

## Notes

- The site pages are already available in this folder.
- The local server is recommended because the pages use embedded script loading and may not work reliably over `file://` in some browsers.
