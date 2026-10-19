# Shivankur Portfolio: multi-page static site

Routes:
- `/work` (hero + selected work)
- `/case-studies` (current featured projects; ready for additional case studies)
- `/about`
- `/thinking`
- `/beyond`

Shared styling is in `styles.css`. Assets and CV files stay at the project root. Navigation, breadcrumb links, LFG CV/print chooser, and mobile menu are shared across routes.

Deploy the contents of this folder to the existing Vercel project. The static directory routes are represented by `work/index.html`, `case-studies/index.html`, etc.

## Creator-led Travel case study viewer

The case study is shown as a one-page-at-a-time image viewer at `/case-studies`, with Previous/Next navigation and direct contact CTAs. The source PDF is not included in the deploy package, and the viewer does not provide a download or full-screen control. Context-menu and drag actions are discouraged and the viewer is hidden in print styles. This is a deterrent, not absolute copy protection: any publicly viewable web content can still be captured by screenshots or browser developer tools. For enforceable access restrictions, use authenticated hosting and access controls.


Case study PDF viewer update:
- Replace `case-studies/index.html` and `styles.css` from this package.
- Add `assets/case-studies/creator-led-travel.pdf` at the same path.
- Keep the existing `vercel.json` and other page/assets structure.
- The case studies page embeds the PDF with its toolbar hidden where supported; browser PDF behavior can vary, and public assets cannot be made impossible to download.


## Case studies grid update
The Case Studies route now has a searchable, filterable responsive grid, PDF viewer, drag-and-drop tile selection, and a recommendation engine that ranks related case studies by shared tags and category. All case study PDFs are in `assets/case-studies/`. The Partner Acquisition Engine card links to https://nobroker.in/dsa-loan and distinguishes the web designer’s landing-page build from Shivankur’s end-to-end customer/client journey ownership.
