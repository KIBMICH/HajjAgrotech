# Hajj Hussain Agrotech

Responsive React + TypeScript company website using Vite, Tailwind CSS and Lucide React.

## Start the site

1. Install dependencies with `npm install`.
2. Run `npm run dev`.

## Enquiry form integration

The form validates required fields and email addresses in the browser. It only reports a sent enquiry after a successful backend response. To connect it, copy `.env.example` to `.env.local` and set `VITE_ENQUIRY_ENDPOINT` to an endpoint that accepts JSON by POST and returns a successful HTTP status. Without that configuration, the form directs visitors to the listed phone and email contacts instead of pretending the enquiry was sent.

## Video showcase

The page accepts YouTube and Vimeo URLs or an MP4 URL. The MP4 picker previews a selected file locally in the current browser session. Permanent uploads and multi-video administration require a storage service and admin backend.

## Business assets and content

Agricultural photographs are stored locally in `public/images`, so the page does not depend on remote image requests. Add the supplied company logo and leadership portrait when available; the leadership area intentionally shows a placeholder rather than an unrelated person's photo. The company details and contact copy are in `src/App.tsx`; equipment and service entries are data-driven arrays near the top of that file, ready to move to a content API later.
