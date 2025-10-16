<h1>Personal Portfolio — Website Architecture</h1>

<h2>1. Project Summary</h2>
<p>Responsive, component-based personal portfolio website with three pages: Landing, Projects, and Resume/Contact. Includes external links to the BIT degree progress website (Education section) and an Architectural Visualization site (Hobbies section).</p>

<h2>2. Pages Overview</h2>
<p><strong>Landing Page (/):</strong> About Me, Profile Summary, Experience, Projects Preview, Education, Certificates, Skills & Abilities, Hobbies, and Contact Information.</p>
<p><strong>Projects Page (/projects):</strong> Detailed project gallery with filters, tech tags, and individual project details.</p>
<p><strong>Resume/Contact Page (/resume):</strong> Printable resume, download CV option, and contact form integration.</p>

<h2>3. High-Level Architecture</h2>
<p>Static site hosted on GitHub Pages or Netlify with CI/CD via GitHub Actions. Content is rendered through reusable components and structured data files. Optimized for performance, accessibility, and SEO.</p>

<h2>4. Component Map</h2>
<p>Layout (Header, Footer, SEO Component)</p>
<p>Hero, About, ProjectCard, ExperienceTimeline, SkillsChart, CertificateList, ContactForm</p>
<p>Shared UI: Button, Icon, Badge, Modal, Card</p>

<h2>5. Data Model</h2>
<p>/data/projects.yaml — title, slug, description, images, tech stack, demo link, repo link</p>
<p>/data/experience.yaml — company, role, duration, highlights</p>
<p>/data/education.yaml — degree, institution, duration, external link (BIT progress)</p>
<p>/data/certificates.yaml — certificate name, issuer, date, file link</p>
<p>/data/skills.yaml — category, skill, proficiency level</p>

<h2>6. File Structure</h2>
<p>personal-portfolio/</p>
<p>├── README.md</p>
<p>├── public/</p>
<p>├── src/ (pages, components, styles, utils)</p>
<p>├── data/ (YAML or JSON files)</p>
<p>├── assets/ (images, pdfs)</p>
<p>└── .github/workflows/deploy.yml</p>

<h2>7. Technology Stack</h2>
<p>Frontend: React with Vite (or static HTML)</p>
<p>Styling: Tailwind CSS or SCSS</p>
<p>Hosting: GitHub Pages / Netlify</p>
<p>Deployment: GitHub Actions</p>
<p>Forms: Netlify Forms / Formspree</p>
<p>Analytics: Plausible / Google Analytics</p>

<h2>8. Performance and Accessibility</h2>
<p>Optimized images (WebP/AVIF)</p>
<p>Lazy-loading and static rendering</p>
<p>Accessible components with proper ARIA labels</p>
<p>Semantic HTML structure and heading hierarchy</p>
<p>Lighthouse targets: Performance > 90, Accessibility > 90</p>

<h2>9. CI/CD Workflow</h2>
<p>Trigger: Push to main branch</p>
<p>Steps: Lint → Test → Build → Deploy</p>
<p>Deployment: Automatic to GitHub Pages or Netlify</p>
<p>Branch protection enabled for main branch</p>

<h2>10. Maintenance Guide</h2>
<p>Add a new project: Update /data/projects.yaml and add images</p>
<p>Add a new certificate: Update /data/certificates.yaml</p>
<p>Run Lighthouse monthly to monitor performance</p>
<p>Keep dependencies updated regularly</p>

<h2>11. External Links</h2>
<p>BIT Degree Progress Website — linked under Education section</p>
<p>Architectural Visualization Website — linked under Hobbies section</p>

<h2>12. Summary</h2>
<p>Personal Portfolio showcasing About, Projects, Education, Skills, and Hobbies across three pages. Built with modern web standards, easily maintainable, and deployed seamlessly through GitHub Pages or Netlify.</p>
