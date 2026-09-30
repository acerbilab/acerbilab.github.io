# acerbilab.github.io

The organisation site of acerbilab, served at <https://acerbilab.org>.

Because this repo carries the organisation's custom domain, every other acerbilab repo that
publishes a GitHub Pages site is served under it, at `acerbilab.org/<repo>/` (for example
`acerbilab.org/pyvbmc/`), and its `acerbilab.github.io/<repo>/` address redirects there. A
repo that sets a custom domain of its own is the exception.

`index.html` redirects the root, `acerbilab.org`, to the hub of the lab's model-fitting
tools at `acerbilab.org/model-fitting/` (repository `acerbilab/model-fitting`). A folder
added here is served at `acerbilab.org/<folder>/`, unless a repository has the same name.

## Domain

- **Registrar:** Namecheap; `acerbilab.org` is registered until 2029-09-30. If it lapses,
  every link that uses the domain breaks.
- **DNS** (Namecheap, Advanced DNS): four A records for `@` to GitHub Pages
  (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`), a CNAME
  record from `www` to `acerbilab.github.io`, and the TXT record
  `_github-pages-challenge-acerbilab` that verifies the domain for the organisation.
- **GitHub:** the domain is verified in the organisation's Pages settings, and set with
  HTTPS enforced in this repo's Settings → Pages, which stores it in the `CNAME` file. The
  site deploys from `main`, at the root, with no build (`.nojekyll`).
