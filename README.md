<h1>Personal Portfolio — Website Architecture</h1>

<h2>1. Project Summary</h2>
<p>Three-page static portfolio: Landing (index.html), Education progress (portfolio_bit_progress.html), Hobbies showcase (portfolio_hobbies.html). Core assets sit in css/, img/, and js/ folders.</p>

<h2>2. Pages Overview</h2>
<p><strong>Landing (index.html)</strong> — hero, about, profile summary, experience, projects preview, education link, certificates, skills & abilities, hobbies link, and contact information.</p>
<p><strong>Education (portfolio_bit_progress.html)</strong> — dedicated page or linked snapshot for BIT degree progress.</p>
<p><strong>Hobbies (portfolio_hobbies.html)</strong> — architectural visualization showcase.</p>

<h2>3. High-Level Architecture</h2>
<p>Static site deployed from a repository root containing three HTML pages and three top-level asset folders. CI/CD via GitHub Actions or direct GitHub Pages deploy is supported.</p>

<h2>4. Repository Structure</h2>
<p>Root files and folders as seen in the repository:</p>
<p>css/  — stylesheet files (global.css, theme, vendor css)</p>
<p>img/  — all image assets (hero, project thumbnails, certificates)</p>
<p>js/   — client scripts (navigation, analytics stubs, gallery)</p>
<p>README.md — project documentation and architecture overview</p>
<p>index.html — Landing page (primary entry)</p>
<p>portfolio_bit_progress.html — BIT progress showcase. Represent the bit degree program completion amount as a percentage</p>
<p>portfolio_hobbies.html — Hobbies (Architectural visualization) page included all the projects recently done as the hobby</p>

<h2>5. Content & Data</h2>
<p>Content is embedded in the HTML pages; consider moving structured content to /data (YAML/JSON) if you want programmatic rendering or easier updates.</p>

<h2>6. Deployment Notes</h2>
<p>To publish on GitHub Pages, set the repository to serve the root and ensure index.html is present.</p>
<p>Use GitHub Actions to run optional build steps (minify CSS/JS, image optimizations) before pushing final artifacts to the gh-pages branch or main branch for Pages.</p>

<h2>7. Maintenance Checklist</h2>
<p>Last update done on 16/10/2025 to the Readme file to update the website architecture.</p>
<p>Update pages: edit index.html, portfolio_bit_progress.html, and portfolio_hobbies.html as content changes.</p>

<h2>8. Quick README snippet</h2>
<p>Repo layout: css/, img/, js/, index.html, portfolio_bit_progress.html, portfolio_hobbies.html, README.md.</p>

<h2>9. External Links</h2>
<p>BIT degree progress and completion percentage can be review through the portfolio_bit_progress.html file.</p>
<p>Hobbies entry links to the portfolio_hobbies.html page in the repo.</p>

<h2>10. Summary</h2>
<p>Repository follows a straightforward static structure with three HTML pages and clear top-level asset folders matching the screenshot. This keeps deployment simple and content easy to manage.</p>
