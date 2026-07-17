# suitberry-publisher

Daily deploy pipeline for suitberry.com. Clones the private content repo with a
read-only deploy key and deploys the static site to Cloudflare Workers, then
pings IndexNow. Runs on a schedule (03:00 and 09:00 UTC) and on manual dispatch.

No site content lives here; this repo exists so the recurring job runs on free
public-repo Actions minutes.
