# Shivankur Ghosh Portfolio - full static site

## Routes
- `/work` - portfolio home and selected work
- `/case-studies` - searchable catalogue of all 16 case studies, numbered 0-15 to match their supplied source documents
- `/about`
- `/thinking`
- `/beyond`

## Structure
- `styles.css` - shared site styling
- `assets/` - required site media, favicon, updated watermarked CV and case study PDFs
- `case-studies/index.html` - searchable case study catalogue and gated download flow
- `work/index.html` - selected work with direct case study routes
- `vercel.json` - clean static routes

## Case study PDFs
The website includes watermarked, searchable PDF copies of all 16 supplied case studies under `assets/case-studies/`. The original unwatermarked PDFs are not included in the public deployment assets. The PDFs retain their original page content and page count, with a subtle diagonal `SHIVANKUR GHOSH | PORTFOLIO COPY` watermark.

The catalogue asks for the configured passcode and a short lead form before initiating a download. Because this is a static front end, the passcode is a UI gate and not server-side access control; the deployed PDF URLs remain public to anyone who knows them. Do not treat the gate as secure document authorization.

## Deploy
Deploy the contents of this folder to the existing Vercel static project. Preserve the directory structure and all referenced local assets.
