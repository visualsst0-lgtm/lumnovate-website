# LUMNOVATE Website — Responsive Static Starter

A polished, responsive, premium dark-gradient website with glass-style cards, cyan/lime accents, smooth rounded UI and the selected LUMNOVATE wordmark. Social profiles are text links (Instagram, LinkedIn, YouTube), not platform logos.

## Technology used

- **HTML5** — page structure and content.
- **CSS3** — responsive layout, gradients, translucent/glass surfaces, animations and mobile UI.
- **Vanilla JavaScript** — mobile navigation, portfolio filtering, modal video player, enquiry form and WhatsApp draft generation.
- **Google Fonts** — DM Sans and Space Grotesk, loaded from Google Fonts when online.
- **Google Drive / YouTube / direct MP4 embeds** — optional portfolio playback sources.
- **GitHub Pages** — can host the static site for free.
- **Python is not required to run the website.** A Python local server is only an optional way to preview it locally. Java is not used; JavaScript is a different language from Java.
- **No backend/database is included.** Secure direct client uploads, private client accounts, app logins, bookings or a dashboard would need a backend/storage provider and access controls.

## Services represented

- Editing Only — ₹17,999/month for 15 Reels; no Meta Ads management.
- Growth Engine — ₹24,999/month for 15 Reels + Meta Ads management; ad spend is separate.
- AI Product Ads — from ₹4,999/ad, scoped by complexity.
- Website development / landing pages — from ₹24,999, final scope confirmed in writing.
- E-commerce / digital storefronts — custom quote based on catalogue, integrations and checkout needs.
- Website care & maintenance — from ₹2,500/month for an agreed scope.
- App development — project estimate after discovery; don't advertise a fixed price before scope is understood.
- AI Workflow Automation — Coming Soon; not available for purchase yet.

These are proposed starting prices, not independently verified market averages. Confirm scope, revisions, timeline, tax treatment and third-party costs in a written quotation before accepting a project.

## Before publishing

1. Open `js/site-data.js`.
2. Confirm the configured WhatsApp number `917721819359` (+91 77218 19359) opens the correct business account.
3. Add approved portfolio work to the `portfolio` array. Set `approvedForPublicDisplay: true` only after the client grants permission.
4. Test every social link, WhatsApp CTA, mobile navigation, form and video playback on a real phone.

## Add a Reel to the portfolio

Add an object in `js/site-data.js`:

```js
{
  title: "Footwear product Reel",
  category: "reels", // reels | ads | ai | web
  label: "VIDEO EDITING",
  description: "Short-form product edit with captions and sound design.",
  mediaUrl: "https://drive.google.com/file/d/FILE_ID/view?usp=sharing",
  coverUrl: "", // optional public image URL or path to a cover image
  mediaType: "drive", // mp4 | drive | youtube
  client: "Client name only with permission",
  approvedForPublicDisplay: true,
  demo: false
}
```

For Google Drive, the video owner must approve public display and enable “Anyone with the link — Viewer” where appropriate. The site converts a standard Drive file link into the Drive preview player. Playback varies by browser/account, so test every file. For reliable playback, use a video host that provides an embeddable player or direct MP4 URL. Do not commit large videos to GitHub Pages.

## Client submissions

The website does not offer a direct video-upload portal. Clients use the enquiry form to describe their project; file transfer and final delivery are coordinated directly over WhatsApp or another agreed method. Do not ask clients to share account passwords or credentials.

## Run locally

Open `index.html` in a modern browser. Optionally, from this folder run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`. Python is just a local preview server here; the deployed website itself is HTML/CSS/JavaScript.

## Publish on GitHub Pages

1. Create a GitHub repository, e.g. `lumnovate-website`.
2. Upload the contents of this folder (not the ZIP file) into the repository root.
3. Open **Settings → Pages** and select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Save, wait for deployment, then test the published URL on mobile.
5. Configure a custom domain separately if needed.


## V6 positioning notes
- LUMNOVATE is described as a founder-led independent business, not a large studio.
- Client counts and founder-journey claims are intentionally omitted for now; add a dedicated founder story later when ready. No view counts, ROAS or fabricated testimonials are used.
- The uploaded reference screenshots were used only as design inspiration; they are not included as LUMNOVATE portfolio assets. Add your own work photos/videos and obtain client approval before publishing.
- Replace the founder photo placeholder with an actual photo of you working. Do not use competitor-site screenshots as portfolio proof.
- App development is quoted after requirements are understood; only promise delivery that you or your confirmed development partner can support.


## V7 design update
The manifesto section has been simplified: removed the decorative “LV / STUDIO” stamp and the redundant “Make it meaningful” side block. The section now uses one aligned headline, supporting paragraph and a quiet text sign-off.


## Version 8 update

- Removed the client-count / founder-journey section so the site can grow without maintaining fixed numbers.
- Social profiles use icon-only links for Instagram, LinkedIn, and YouTube. WhatsApp uses its icon plus the contact number, without a text label.
- Keep accessible labels on icon links; they appear to screen readers and on hover tooltips.
