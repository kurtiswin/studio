# kurtiswin website

A static site: no build step. Vercel serves `index.html` as the home page.

## Put it live on Vercel

**Option A, Vercel CLI (quickest)**
1. Unzip this folder.
2. In a terminal, go into the folder and run `npx vercel`, then follow the prompts (log in, accept the defaults).
3. Run `npx vercel --prod` to make it the live version.

**Option B, from GitHub**
1. Create a new GitHub repository and upload the contents of this folder (index.html at the top level).
2. In Vercel: Add New > Project > import that repository.
3. Framework preset: **Other**. Leave the build command and output directory empty. Deploy.

## Connect your domain
Vercel project > Settings > Domains > add your domain, then follow the DNS records Vercel shows.

## Email sign-up
Sign-ups go to Kit form 10152446. To change it, edit `const KIT_FORM_ID` near the bottom of `index.html`.
