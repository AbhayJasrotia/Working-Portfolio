# Abhay Jasrotia — Portfolio

A sleek, dark-themed personal portfolio. Fully static — deploy on Vercel in seconds.

---

## ✉️ Activating the Contact Form (EmailJS — Free, No Backend)

The form uses [EmailJS](https://www.emailjs.com). Free tier = 200 emails/month.

### Step-by-step (~5 minutes):

1. **Sign up** at https://www.emailjs.com

2. **Add Email Service** → choose Gmail → connect `abhayjasrotia124@gmail.com`
   → copy the **Service ID** (`service_xxxxxxx`)

3. **Create Email Template** with variables `{{from_name}}` `{{reply_to}}` `{{message}}`
   Set To Email = `abhayjasrotia124@gmail.com` → copy the **Template ID** (`template_xxxxxxx`)

4. **Account → API Keys** → copy your **Public Key**

5. In `index.html` find these 3 lines and replace placeholders:
   ```js
   const EMAILJS_PUBLIC_KEY  = 'YOUR_PUBLIC_KEY';
   const EMAILJS_SERVICE_ID  = 'YOUR_SERVICE_ID';
   const EMAILJS_TEMPLATE_ID = 'YOUR_TEMPLATE_ID';
   ```

---

## 🚀 Deploy to Vercel

### Drag & Drop (Easiest)
Go to vercel.com → Add New Project → drag this folder in → Deploy.

### CLI
```bash
npm i -g vercel && vercel
```

### GitHub (Best — auto-deploys on every push)
Push to GitHub → Vercel → New Project → Import from GitHub.

---

## 📁 Files
- `index.html` — The complete portfolio (single file)
- `vercel.json` — Vercel deployment config
- `Abhay_J_resume_.pdf` — Your resume (add this file!)

## 🚀 Deploy to Vercel (3 ways)

### Option 1: Drag & Drop (Easiest — no account needed initially)
1. Go to [vercel.com](https://vercel.com) → Sign up / Log in
2. Click **"Add New Project"** → **"Import"**
3. Or just drag this folder into the Vercel dashboard

### Option 2: Vercel CLI
```bash
npm i -g vercel
cd portfolio/
vercel
```
Follow the prompts. Your site will be live in ~30 seconds.

### Option 3: GitHub → Vercel (Best for ongoing updates)
1. Push this folder to a GitHub repo
2. Go to vercel.com → New Project → Import from GitHub
3. Vercel auto-deploys on every `git push`

## ✏️ Customizations Before Deploying
1. **Add your resume PDF**: Place `Abhay_J_resume_.pdf` in the same folder
2. **Update GitHub URL**: Search for `AbhayJasrotia` and replace with your actual GitHub username
3. **Update LinkedIn URL**: Replace `abhayjasrotia` with your actual LinkedIn handle
4. **Update project links**: Find the 3 `href="#"` on project cards and add your actual repo/demo URLs
5. **Custom domain**: In Vercel dashboard → Settings → Domains → add your domain

## 🎨 Features
- Custom animated cursor
- Scroll-reveal animations
- Fully responsive (mobile-friendly)
- Active nav highlighting
- Working contact form (shows success state)
- Resume download button
- All 5 sections: About, Projects, GitHub, Resume, Contact
