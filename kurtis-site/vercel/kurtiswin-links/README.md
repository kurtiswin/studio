# Kurtis Win · link page (link.kurtiswin.com)

A static page with no build step. Vercel serves `index.html` as the home page.

## Put it live on Vercel (as its own project)
1. Unzip this folder.
2. In a terminal, go into the folder and run `npx vercel`. When asked, create a **new** project (e.g. `kurtiswin-links`) and accept the defaults.
3. Run `npx vercel --prod`.
   (Or: upload the folder to a new GitHub repo, then Vercel > Add New > Project > import it, preset **Other**, no build command.)

## Add link.kurtiswin.com
In the new project: Settings > Domains > add `link.kurtiswin.com`.
kurtiswin.com already uses Vercel's nameservers, so Vercel sets up the record and the HTTPS certificate itself.

## What's wired up
- The KurtisWin logo links to https://www.kurtiswin.com
- Email sign-up goes to Kit form 10152446 (change `KIT_FORM_ID` near the bottom of index.html to use another form)
- Java Bonito and Woolton FC link to their sites; Stories from Football has no link until the new domain is ready
