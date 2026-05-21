# Maa-mee.studio · Digital Catalog

## Files
- `index.html` — Customer catalog (this is the link you put in your bio)
- `admin.html` — Your private panel to update the weekly fabric

---

## How to go live (5 minutes, free)

### Option A — Netlify Drop (easiest, recommended)
1. Go to https://app.netlify.com/drop
2. Drag the entire `maameestudio` folder onto the page
3. Netlify gives you a URL like `random-name.netlify.app`
4. Rename it under Site Settings → Domain → Custom subdomain
   e.g. `maameestudio.netlify.app`
5. Put `maameestudio.netlify.app` in your Instagram bio
6. Access your admin at `maameestudio.netlify.app/admin.html`

### Option B — GitHub Pages (free, slightly more steps)
1. Create a free GitHub account at github.com
2. Create a new repository called `maameestudio`
3. Upload both HTML files
4. Go to Settings → Pages → Deploy from main branch
5. Your site is at `yourusername.github.io/maameestudio`

---

## Admin panel login
Password: `maameestudio2026`

⚠️ Change this in `admin.html` line with `const ADMIN_PW = 'maameestudio2026'`
Change it to something only you know before going live.

---

## How to update weekly fabric (takes 2 minutes)

1. Go to `yoursite.netlify.app/admin.html`
2. Enter your password
3. Type the fabric name + description in Thai/English
4. Upload the fabric photo (drag & drop works)
5. If it's sold out, toggle "Sold Out" ON
6. Click บันทึกและอัพเดท Catalog
7. Open `index.html` in a new tab — it updates immediately ✓

---

## Updating your Line OA link
In the admin panel, paste your Line OA link (lin.ee/...) in the Line OA section and save.

---

## What customers see
- This week's fabric name + photo
- Collar mockup with gold/silver hardware selector
- Bandana mockup (no hardware)
- Size selector (XS / S / M)
- "สั่งผ่าน Line OA" button → opens your Line OA
- If sold out: button changes to "ทักหาเราเพื่อสอบถาม"
- No login, no data collection — just browse and contact you

---

## Important note on the admin panel
The admin panel saves data to the browser's localStorage.
This means: the catalog and admin must be **on the same device/browser** 
for changes to appear, OR you need to use a shared hosting solution.

For most cases (you update from your phone → customers open on any device):
→ Use Netlify or GitHub Pages — they serve static files only.
→ This localStorage approach works perfectly when admin and catalog are on the same domain and you access admin from the same phone/browser each week.

If you want true cross-device syncing later, let Claude know — we can upgrade to a simple Supabase or Airtable backend.
