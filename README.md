# Betty landing

Static marketing site of Betty, served at https://betty.artysan.dev. Plain HTML and CSS, no build
step:

- `index.html`: the landing page and its contact form
- `conditions.html`: terms of use
- `confidentialite.html`: privacy policy
- `brand/`: icon and logotypes (SVG)

## Preview locally

Open `index.html` in a browser, or serve the folder with any static server:

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Publishing

GitHub Pages publishes the default branch as is, on the domain set in `CNAME`
(`betty.artysan.dev`): whatever is pushed there is live.

## Contact form

`CONTACT_ENDPOINT` is still empty in `index.html` (`// TODO`), so the form opens the visitor's mail
app with a `mailto:` to contact@artysan.dev. Set it to a form service URL (Formspree, Web3Forms, an
API route...) that accepts a POST of form data to send submissions there instead.
