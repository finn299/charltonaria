Charlton Aria Acquisition Corporation — charltonaria.com

Static IR-style website (single-file pages, one shared stylesheet).

Files
-----
index.html        — Home / hero / key facts
about.html        — Company facts, structure, governance
strategy.html     — Acquisition strategy, target criteria, process
team.html         — Management & board (current state, post Feb 2026 resignations)
sponsor.html      — ST Sponsor II Limited
filings.html      — Selected SEC filings with EDGAR links
contact.html      — Inquiry form + registered office

Assets
------
styles.css                 — Shared stylesheet (navy + gold)
logo-charlton-aria.svg     — Full crest logo (used on hero)
favicon.svg                — Browser favicon (mini shield mark)

Color palette
-------------
Navy primary:     #0a1d3d
Navy gradient:    #15315f (top) → #061330 (bottom)
Gold:             #c79b3f
Gold light:       #e7c573
Gold dark:        #9b7728
Background warm:  #f6f3ec
Border:           #e3dfd2

Fonts
-----
Serif: Cormorant Garamond (Google Fonts) — headings
Sans:  Inter (Google Fonts) — body, navigation, UI

Notes
-----
- Mobile menu fix applied (opaque background, explicit z-index)
- All pages use identical <nav> and <footer> blocks
- EDGAR CIK is 0002024459. Replace stub filing links with permanent
  EDGAR accession URLs as they become available.

Contact form (info@charltonaria.com)
------------------------------------
The contact form posts to FormSubmit.co, a free relay service that
forwards submissions as email. No account or API key is required.

ACTIVATION (one-time):
1. Publish the site so contact.html is reachable on a public URL
2. Submit the form once with any test data
3. FormSubmit will email info@charltonaria.com a one-time activation
   link. Click it to authorize the address.
4. All subsequent submissions will arrive at info@charltonaria.com.

If you'd prefer a different provider (Formspree, Netlify Forms,
Resend with a serverless function, etc.), update the <form action>
attribute in contact.html.

To do before production
-----------------------
1. Replace the SVG logo with the official high-resolution logo file
2. Activate FormSubmit (first submission triggers an activation email)
3. Replace stub 8-K filing URLs with specific EDGAR accession links
4. Confirm director biographies with the company (kept conservative)
5. Add SEO meta tags (og:image, twitter card) per page
6. Add real analytics (GA4 or similar) if desired
