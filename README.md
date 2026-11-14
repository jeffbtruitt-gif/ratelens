# RateLens

Daily interest rate dashboard (US Treasury par curve, prime / fed funds / IORB, Freddie Mac mortgage rates).

Live site: https://jeffbtruitt-gif.github.io/ratelens/

The page is a single static `index.html` that reads directly from the Supabase warehouse (`rate_series` / `rate_observations`) using a publishable, read-only key. Data is refreshed daily by the loader in the private `benchmark-rates` repo, so the site picks up new rates automatically — no redeploy needed.
