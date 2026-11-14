# app-policy

What the apps read to know whether they may still run, and the pages the stores link to.

- `crewlink.json`, `policy.json` — the owner's signed word on each app's builds (`{"p": "<policy>", "sig": "<ECDSA P-256>"}`).
  Only a file signed with the owner's key counts, so this can be served from anywhere public.
  Written by `peer-kit/tools/policy/sign_policy.py`, which publishes here and to z4.
- `privacy/` — the privacy policy pages Google Play and the App Store link to.

Served by GitHub Pages at https://vinhthaipham.github.io/app-policy/ . Nothing here is secret; the private key never leaves the owner's Mac.
