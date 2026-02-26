# Deploying VoiceGivers to GitHub Pages

## One-time setup

1. **Create a GitHub account** (if you don't have one) at https://github.com

2. **Create a new repository:**
   - Go to https://github.com/new
   - Name it `voicegivers-web` (or anything you like)
   - Set it to **Public**
   - Click "Create repository"

3. **Upload your files:**
   - On the new repository page, click "uploading an existing file"
   - Drag in `index.html` and the `images/` folder (with your photos)
   - Click "Commit changes"

4. **Enable GitHub Pages:**
   - Go to your repository → **Settings** → **Pages** (left sidebar)
   - Under "Branch," select `main` and `/ (root)`
   - Click **Save**
   - Your site will be live at `https://yourusername.github.io/voicegivers-web/` within a minute or two

## Pointing voicegivers.org to GitHub Pages

Once the site is live on GitHub Pages, you can point your domain to it:

1. In GitHub Pages settings, add `voicegivers.org` as a Custom Domain
2. In your domain registrar (wherever voicegivers.org is registered), update the DNS:
   - Add 4 A records pointing to GitHub's IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add a CNAME record: `www` → `yourusername.github.io`
3. DNS changes can take up to 24 hours to propagate

GitHub Pages with a custom domain is **free**.

## Updating the site later

To update content, edit `index.html` directly in GitHub's web editor, or re-upload the file.
