
# Rowing Club Website (Free, with Admin CMS)

**Stack:** Eleventy (11ty) + Decap CMS + Netlify (free) + custom domain.

- Free hosting on Netlify
- Free CMS at `/admin` for editing pages, news posts, and gallery
- Images upload into the repo under `images/uploads`
- Custom domain + HTTPS supported

## Quick Start

1. Create a **new GitHub repo** and upload these files.
2. Go to **Netlify** → **Add new site** → **Import from Git** → connect your GitHub repo.
3. Accept defaults; build command `npm run build`, publish dir `_site`.
4. Once deployed, open **Netlify → Identity**:
   - Click **Enable Identity**.
   - Under **Services**, enable **Git Gateway**.
   - Invite your admins via **Invite Users** (they’ll get an email).
5. Visit `https://YOURDOMAIN/admin` to log in and start editing.
6. Add a **custom domain** in Netlify → Domain Management (you only pay your domain registrar).

## Local development (optional)
- Install Node 18+
- Run: `npm install` then `npm run dev`

## Editing Structure
- Static pages: Home, About, Learn to Row, Contact
- News posts (create many): `news`
- Gallery items (image + caption): `gallery`

## Notes
- The CMS stores content and images directly in your Git repository via Git Gateway.
- You can add more pages/collections by editing `admin/config.yml`.
