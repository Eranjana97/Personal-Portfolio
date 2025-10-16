# Website architecture — Personal Portfolio (3 pages)

1️⃣ **Project summary**
   🔹A responsive, accessible, single-repository portfolio site with three routed pages:
         -Landing (home) — hero, about, profile summary, experience (timeline), projects, education (links to BIT progress site), certificates, skills & abilities, hobbies (links to your architectural visualization site), and contact.
         -Projects — detailed project gallery (cards → detail modal or page).
         -Resume / Contact — printable resume and a contact form (optional serverless submission).
   🔹External links:
         -BIT program progress site (linked from Education)
         -Architectural visualization site (linked from Hobbies)
   🔹Primary goals: clarity, quick load, maximum discoverability, strong UX on mobile and desktop, and easy maintainability.

2️⃣**High-level architecture diagram**
[User browser] 
    ↕ (HTTPS)
[Static site (GitHub Pages / CDN)]
    ├─ HTML (index.html + route handling)
    ├─ CSS (tailwind / separated stylesheet)
    ├─ JS bundle (React/Vite or vanilla)
    ├─ Assets (images, svgs, fonts)
    └─ Meta files (sitemap.xml, robots.txt)
         ↕
    ├─ External services
    │    ├─ Analytics (e.g., Plausible / Google Analytics)
    │    ├─ Forms (Netlify Functions / Formspree / Email API)
    │    └─ Linked sites (BIT progress site, ArchViz site)
    └─ CI/CD (GitHub Actions → build → deploy to GitHub Pages or Netlify)
    
3️⃣**Pages and component map**
   🔹Pages
     Landing (/)
       Header (site nav — sticky)
       Hero (name, tagline, CTA)
       About (short bio + profile photo)
       Profile summary (quick bullets: focus areas, tech stack)
       Experience (timeline cards with role, company, date range, highlights)
       Projects (compact cards with thumbnails, short descriptions, tech tags; each card opens detail)
       Education (degree, institution, graduation, link to BIT progress website)
       Certificates (list or carousel; downloadable PDFs)
       Skills & Abilities (skill groups, proficiency indicators)
       Hobbies (short text + link to architectural visualization site)
       Footer (contact channels, social links, copyright)
   🔹Projects (/projects)
   🔹Resume & Contact (
    
