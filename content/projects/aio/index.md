---
title: All-in-One
tagline: The super-app I'm building for my own everyday problems, and the login behind my other apps.
weight: 30
live: https://aio.opanmustopah.com/
repo: https://github.com/opan/all-in-one
stack: [Go, Svelte, TypeScript, WebSocket, OpenTelemetry]
---
All-in-One collects the small tools I kept wanting in one place:

- **Listings.** Topics with your own JSON schema, and items inside them.
- **Chat.** Real-time conversations over WebSocket, with invites.
- **Short links.**

It's also the account system for [Tally](/projects/tally/) and
[Cashflow](/projects/cashflow/): it acts as an OpenID Connect provider, with
optional TOTP two-factor login and password reset by email.

Look around without signing up: log in with username `demo`, password `demo123`.
