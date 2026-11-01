# greg7gkb.github.io

Serves `/.well-known/assetlinks.json`, which lets the [Deputy](https://github.com/greg7gkb/deputy)
Android app open its own `https://greg7gkb.github.io/deputy/activity/<id>` links (Android App
Links). Deputy writes those links into things it creates, like a calendar hold, so tapping one
opens that entry in Deputy's Activity log.

- `.well-known/assetlinks.json`: the app's package name and its signing certificate's public
  SHA-256 fingerprint. If the app is signed with a different key, add that fingerprint here.
- `.nojekyll`: serve files as-is (Jekyll would otherwise skip the `.well-known` folder).
- `404.html`: what someone without the app sees if they open a Deputy link.

The repo that used to live at this name (a friend's portfolio I helped debug in 2022) is
archived as `prince-website-2022`.
