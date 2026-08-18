Please do the following two small manual steps after this commit:

1) Upload the lace background image you provided into the repository at:
   /assets/lace.png
   - The CSS expects the image at that path and will use it behind the hero name on the home page.
   - If you prefer a different filename or path, update styles.css (the .hero.texture-dark rule).

2) Configure Formspree for the contact form:
   - Sign in to Formspree (https://formspree.io) and create a new form — you'll be given a form endpoint id such as `f/abcdxyz`.
   - Open contact.html and replace the action value on the <form> tag with your form endpoint. Example:
       action="https://formspree.io/f/abcdxyz"
   - Optionally replace or remove the _next hidden field if you want a custom success URL.

What I changed in this commit:
- Updated contact.html: added a two-column layout (info card + contact form) and Formspree-ready form + JS to show a success message after redirect.
- Updated index.html: left markup in place; styles updated so the hero uses a lace background image at /assets/lace.png.
- Updated styles.css: added hero lace background rule and new contact form styles that match the reference layout more closely.

If you want, I can also upload the lace image into the repo for you — you'll need to confirm I should use the image you attached in chat as the file /assets/lace.png and I'll add it in a follow-up commit.
