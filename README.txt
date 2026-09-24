SUB ROSA / AMICHAY PERETZ KLOPSHTOCK - LANDING PAGE
Static site for GitHub Pages, custom domain https://www.buysubrosa.com/

DEPLOY (GitHub Pages)
1. Put every file from this folder in the root of the repository's Pages
   branch (keep them together). CNAME already contains www.buysubrosa.com and
   .nojekyll stops GitHub from processing the files.
2. In the repository's Pages settings, set the custom domain to
   www.buysubrosa.com and enable HTTPS once DNS points to GitHub.

CONTACT FORM
The form uses action="mailto:amichay@buysubrosa.com" (no third-party
processor). When a visitor submits, their own email app opens with the message
filled in. Visitors without a configured email app will see nothing happen, so
the page also shows the email address next to the form.

BEFORE GOING LIVE
1. Recommendations: three real testimonials scroll in a marquee. Each card
   appears twice in the HTML (two identical lists) so the loop has no gap.
   To edit a quote, change its English text in both lists (data-i18n="t1q",
   "t1n", "t1r", ...) and the Hebrew text in the HE dictionary at the bottom
   of index.html. To add a card, add it to both lists with new keys.
2. Logos: logo-*.png / logo-mekorot.svg are your supplied logos, trimmed and
   given transparent backgrounds. To replace one, overwrite the file with the
   same name. To add one, copy an <img> line in every <ul> of the logo
   marquee (four identical lists); use class="tall" for square or tall
   emblems and class="lite" for pale logos such as yellow ones.
3. Portrait: in English the photo sits to the right of the text and looks
   toward it. In Hebrew the layout flips, so the photo is mirrored (see
   [dir=rtl] .hero-portrait in the CSS).
   On desktop with a mouse it also tilts up to 8 degrees toward the cursor
   (constant MAX in the script at the bottom of index.html).
4. Privacy: the site sets no cookies and runs no analytics, but Google Fonts
   loads from Google's servers. Self-host Inter and Heebo if you want the
   "completely anonymous" statement to be fully accurate.
5. Accessibility: the marquees pause on hover (and on keyboard focus for the
   recommendations). Run an audit before publishing a WCAG 2.1 AAA claim.
