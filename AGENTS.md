# Agent guidance

## Project structure
- This is a static web app. The main application is `Version001.html`.
- Keep changes focused and preserve the existing no-build workflow unless asked to change it.
- Update this file if the app structure or development workflow changes.

## Maps and external services
- The app uses Leaflet and CARTO Voyager tiles.
- Keep the CARTO key query parameter and visible CARTO/OpenStreetMap attribution intact.
- Do not replace the tile provider or change service configuration unless requested.
- Geocoding uses postcodes.io and Nominatim. Respect each service's current usage policy.

## Input and correctness
- Treat addresses, names, and geocoder responses as untrusted data. Escape them or insert them as text; do not interpolate raw values into HTML.
- Preserve existing workflows for map pinning, selecting, grouping, copying, and sorting unless the requested change calls for a behavior change.
- When changing an interaction, check its related clear/reset and in-progress states as well.

## Verification
- Verify changed behavior in the browser when practical.
- Report what was checked and call out anything that could not be verified.