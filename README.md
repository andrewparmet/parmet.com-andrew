# Andrew’s website

Jekyll source for https://parmet.com/andrew/.

- Edit root Markdown files for topic pages. Their `permalink` values define extensionless URLs such as `/andrew/cycling/`. Old `.html` URLs have no redirects.
- Add dated Markdown files under `_posts/` for blog posts.
- Edit `_data/galleries.yml` for gallery captions, thumbnail paths, full-size image paths, and alt text. Pages insert a gallery with `{% include gallery.html gallery=site.data.galleries.NAME %}`.
- Shared HTML lives in `_layouts/` and `_includes/`; all pages use `style.css`.

Run `bundle install`, then `bundle exec jekyll serve` and visit http://localhost:4000/andrew/ to preview.

Push to `main` to publish through GitHub Pages. Cloudflare proxies the published GitHub Pages site on request. No infrastructure rebuild is needed; GitHub Pages deployment and upstream caching can still delay updates. Keep links relative or under `/andrew/`.
