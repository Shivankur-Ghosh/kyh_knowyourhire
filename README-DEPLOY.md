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

## Interaction updates

- Removed the guided tutorial sequence. A small animated LFG pointer appears in the top navigation area and can be dismissed with Escape.
- Case study cards include a Preview PDF action that opens a separate overlay viewer directly. Visitors can scroll through the document and switch between case-study PDFs; full-screen mode uses a two-Escape close sequence.
- The Download this masterpiece action remains passcode- and lead-form-gated; submitting opens prefilled email and WhatsApp drafts and starts the watermarked PDF download.
- The PDF viewer allows switching between case study PDFs and entering full-screen mode. While in full screen, Escape exits full screen; a second Escape closes the viewer.
- CV chooser, Gang Gang celebration, lead gate and PDF viewer panels are aligned to the top of the viewport.


## Search and navigation QA

- All 16 supplied case studies are represented by catalogue entries 0 through 15.
- Search supports case identifiers, project-name aliases and multi-term matching; a new search clears a selected category filter.
- Empty results provide a one-click clear-search-and-filters action.
- Work page links explicitly target Case Study 2 (The Great Loan Shark), Case Study 5 (Partner Acquisition Engine), Case Study 6 (Digital Partner Catalogue), and Case Study 3 (Elements Mall).
