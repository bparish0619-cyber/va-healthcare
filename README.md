# va-healthcare

VA Health Care Quick Guide, 2026 edition: priority group copays (medication tiers, primary and specialty care, urgent care), key services, enrollment steps, and the contacts that matter.

**Live:** [va.northbrand.net](https://va.northbrand.net) (Cloudflare Pages, project `va-healthcare`)

Copay figures were verified against VA.gov's published 2026 rates before the 2026 edition shipped; they are unchanged from 2025.

## Editing and publishing

Everything is in one file, `index.html` (`index-original.html` keeps the pristine 2025 version for reference). There is no build step.

1. Edit the local master: `~/workspace/va-healthcare/index.html`
2. Copy it to the staging folder: `~/workspace/cloudflare-sites/va-healthcare/`
3. Deploy: `python3 ~/workspace/custom-connectors/custom.cloudflare/bin/cloudflare_deploy.py va-healthcare ~/workspace/cloudflare-sites/va-healthcare`
4. Commit the same `index.html` to this repo so the archive matches the live page, then verify https://va.northbrand.net

An older copy still answers at va-healthcare.vercel.app, untouched; the northbrand.net address is the current one.

## Design

Slate accent inside the Northbrand shell (gold, serif display, the footer lockup). The shared design DNA lives in the northbrand-hub repo.
