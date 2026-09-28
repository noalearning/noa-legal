# Noa legal

The support page, privacy policy and terms of service for the Noa iOS app,
served over GitHub Pages. App Store Connect points at `support.html` (Support
URL) and `privacy.html` (Privacy Policy URL); the root redirects to Support.

**Do not edit the HTML here.** It is generated. The sources of truth are in the
app repo (`noalearning/noa-app`): `App/Resources/Legal/*.md` for the two legal
documents, which is the same Markdown the app bundles and renders in Settings,
and `Marketing/site/support.md` for Support. A hand edit here makes the hosted
policy and the in-app policy disagree.

To update, from the app repo:

```bash
python3 Tools/release/legal-site.py --out build/noa-legal
```

then copy the output over this repo and push.
