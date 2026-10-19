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
