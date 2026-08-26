# Synoro

Static website for [synoro.ch](https://synoro.ch).

The site has no framework, package manager, runtime, or backend. All markup,
styles, and browser behavior live in `index.html`; the images it uses live in
`public/images/`.

## Local preview

Run a static file server with `public/` as its root after copying the entry
page:

```sh
cp index.html public/index.html
python3 -m http.server --directory public 8080
```

Then visit `http://localhost:8080`.

## Deployment

Netlify copies `index.html` into `public/` and publishes that directory. The
deployment command is defined in `netlify.toml`.
