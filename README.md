# Data Sculptor — public site

The public-facing site for **Data Sculptor**, a local-first, deterministic tool for
transforming messy tabular data, built by Red5Sorcery.

**This repository contains the website only.** The engine is in development and is not
published here yet.

## What Data Sculptor is

A local-first analytical workbench for office analysts — the people who receive a CSV,
small enough to open in Excel or far too large for it, and have to turn it into an answer
somebody else can trust. Not a tool for data engineers, and not a programming environment.

CSV in. Excel and CSV out.

The premise is that human analytical judgment is the scarce resource in data work, and
that most tools throw it away: once a file is cleaned, nothing distinguishes a measured
value from a value somebody guessed.

Data Sculptor keeps that distinction. Every cell carries its origin, source identity
survives combination operations, and fabricated values are marked permanently — with the
mark propagating into anything computed from them.

## Status

Prototype 001 is in development. There is no release, no installer, and no beta.
The recipe format — how a sequence of decisions is stored and replayed — is deliberately
unsettled and is not documented here.

## Running locally

No build step, no dependencies. Open `index.html` in a browser, or:

```
python3 -m http.server 8000
```

## Publishing

Served by GitHub Pages from the default branch, repository root.
`.nojekyll` disables Jekyll processing, which this site doesn't need.

To use a custom domain, add a `CNAME` file containing the bare hostname and point a
DNS record at GitHub Pages.

## Licence

Not yet licensed. All rights reserved pending a deliberate decision on the engine's
licence.
