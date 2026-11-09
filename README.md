# caudal-callback

A single static page used as the HTTPS redirect URL for [Caudal](https://github.com/lgiucleab)'s bank connections (Enable Banking only accepts `https://` redirects in production).

It reads `code`, `state` and `error` from the query string, validates them, and forwards them to the desktop app via `caudal://bank-callback`. It has no external scripts, no analytics and no storage. The authorization code is single-use, short-lived, and useless without the app's private key.

Also hosts the app's [privacy policy](https://lgiucleab.github.io/caudal-callback/privacy.html) and [terms of use](https://lgiucleab.github.io/caudal-callback/terms.html), required by Enable Banking's application registration.
