# Java Bonito · link page (link.javabonito.com)

A static page with no build step. Vercel serves `index.html` as the home page.

## Put it live on Vercel (as its own project)
1. Unzip this folder, open a terminal in it and run `npx vercel`. Create a **new** project (e.g. `javabonito-link`).
2. Run `npx vercel --prod`.

## Add link.javabonito.com
javabonito.com's DNS is NOT managed by Vercel (unlike kurtiswin.com), so this takes one extra step:
1. In the new project: Settings > Domains > add `link.javabonito.com`.
2. Vercel shows a **CNAME** record. Copy it exactly (usually Name `link`, Value `cname.vercel-dns.com` or a project-specific `...vercel-dns-017.com`).
3. Log in wherever javabonito.com's DNS lives (the company you bought it from, or where it's currently hosted) and add that CNAME record. Only add the `link` record; leave everything else for javabonito.com alone.
4. Wait for Vercel to show "Valid Configuration" (usually minutes, up to a few hours). HTTPS is then set up automatically.

## Email sign-up
Not sending anywhere yet. Paste the Java Bonito Kit form ID into `var KIT_FORM_ID = '';` near the bottom of index.html.
Until then, pressing the arrow does nothing and no message shows.
