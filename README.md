# roamly

A responsive group-travel planning prototype. Create a trip, list friends, choose how much you already know, and collect trip preferences through a survey.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL shown by Vite.

## Deploy to GitHub Pages

Run `npm run build`, then publish the `dist/` output with a GitHub Actions Pages workflow or `gh-pages` tool. Vite's relative `base: './'` supports repository subpaths. The app uses hash-based URLs to avoid static-host routing errors.

## Important prototype limitation

**All data is stored in localStorage, not a server.** Trip details and survey submissions are only visible in the same browser/device. Copying an invitation URL to another device does **not** share the trip yet. This is a UI and flow prototype, not a production multi-user app.

## Next milestones

1. Supabase database for trips, invitations, participants, and responses.
2. Anonymous invite access with secure per-trip tokens and row-level security.
3. Real date availability picker and overlapping date calculations.
4. Group budget and departure-city comparisons.
5. AI-generated destination suggestions and itineraries (server-side API key only).

Do not collect sensitive personal calendar details until authentication, access controls, and privacy settings are implemented.
