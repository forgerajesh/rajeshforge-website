# Deploy RajeshForge PR Site on Vercel (Subdomain)

Target host: **product.rajeshforge.com**

## 1) Import repository
1. Open: https://vercel.com/new
2. Import `forgerajesh/rajeshforge-website`
3. Framework preset: **Other** (static site)
4. Root directory: `.`
5. Build command: *(leave empty)*
6. Output directory: *(leave empty)*
7. Click **Deploy**

## 2) Add custom domain
1. Vercel Project → **Settings** → **Domains**
2. Add only: `product.rajeshforge.com`

> Keep `rajeshforge.com` and `www.rajeshforge.com` untouched if they are already used by another app.

## 3) DNS records (at your domain provider)
Use the record shown by Vercel for this host. Typical setup:
- `CNAME` record: `product` → `cname.vercel-dns.com`

(If your DNS provider does not allow CNAME for this case, use the fallback record Vercel suggests.)

## 4) Final settings
- In Vercel domains, set `product.rajeshforge.com` as production domain.
- SSL is auto-issued and auto-renewed by Vercel.

## 5) Post-deploy checks
- `https://product.rajeshforge.com` loads over HTTPS
- All menu links work
- Contact page loads
- Mobile layout looks correct

---
If you share Vercel project invite, I can validate DNS propagation and production readiness instantly.
