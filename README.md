# remote-hub-pages

Public pages for the Remote Hub Android app (privacy policy, terms of use and support), served by GitHub Pages from the root of `main`.

| page | URL |
|---|---|
| Privacy policy | https://arsh1219.github.io/remote-hub-pages/privacy |
| Terms of use | https://arsh1219.github.io/remote-hub-pages/terms |
| Support | https://arsh1219.github.io/remote-hub-pages/support |

The app reads these URLs from `app/src/main/res/values/ph_config.xml` (`privacy_url`, `terms_url`) in the app repo. Change both together.

Each page is self contained: inline CSS, system fonts, no scripts, no requests to other hosts. `.nojekyll` makes GitHub Pages serve the files exactly as committed.

`app-ads.txt` for AdMob is **not** in this repo. AdMob only reads it from the root of the developer website domain, so it lives in the `arsh1219.github.io` repo and is served at https://arsh1219.github.io/app-ads.txt. The Play Store listing's developer website must point at `https://arsh1219.github.io/` (or a page under it) for AdMob to find it.
