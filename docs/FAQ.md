# Ishi Mapbox — Frequently Asked Questions

## How is my location determined?

When you open the app, your browser asks for permission to share your location. If you allow it, the app uses your device's built-in GPS (on phones) or Wi-Fi/network-based location (on laptops/desktops) to find where you are. You'll see a blue pulsing dot on the map at your current position. If you deny the permission, the map defaults to a preset location (Dubai).

You can tap **My Location** in the toolbar at any time to re-center the map on your current position.

## How does the map know about streets, restaurants, and places?

The map data comes from **Mapbox**, a mapping platform similar to Google Maps. Mapbox maintains a global database of roads, buildings, parks, restaurants, and other points of interest. This data is sourced from a combination of:

- **OpenStreetMap** — a community-maintained open map database (think Wikipedia but for maps)
- **Government and public datasets** — official road networks, boundaries, etc.
- **Commercial data partners** — business listings, satellite imagery, etc.

The app itself doesn't store any of this map data — it streams the map tiles and place information directly from Mapbox's servers in real time.

## Is the map data up to date?

Mapbox updates their map data regularly, but it's not instant. Major roads and well-known businesses are generally accurate and up to date. Newer streets, recently opened shops, or very recent changes might take days to weeks to appear. This is similar to how Google Maps or Apple Maps work — there's always a small delay between real-world changes and map updates.

## What are pins and where are they saved?

Pins are markers you place on the map by clicking/tapping any spot. Each pin can have a text note attached to it and a color of your choice. Your pins are saved in your **browser's local storage** — this means:

- They are only on **your device**, in **this browser**
- They are **not uploaded** anywhere — no account, no cloud, no server
- If you clear your browser data or use a different browser/device, your pins won't be there
- They persist across page refreshes and closing/reopening the browser tab

## Can other people see my pins?

No. Your pins exist only in your browser's local storage. Nobody else can see them, and they are never sent to any server.

## What do the different map styles do?

You can switch between five map styles using the dropdown in the toolbar:

- **Streets** — the default, showing roads, labels, and points of interest
- **Satellite** — aerial/satellite imagery with street labels overlaid
- **Dark** — a dark-themed map, easier on the eyes in low light
- **Light** — a minimal, light-colored map with less visual noise
- **Outdoors** — emphasizes terrain, hiking trails, and elevation contours

Switching styles doesn't affect your pins — they stay in place regardless of the style.

## What does the "Go to" feature do?

The longitude, latitude, and zoom fields in the toolbar let you jump to any location on Earth by entering coordinates. For example:

- **London**: lng `-0.1276`, lat `51.5074`
- **New York**: lng `-74.006`, lat `40.7128`
- **Tokyo**: lng `139.6917`, lat `35.6895`

Type the values and click **Go** — the map will fly to that location.

## Does the app use my data or track me?

No. The app runs entirely in your browser. There is no backend server, no user accounts, no analytics, and no tracking. The only external service used is Mapbox for rendering the map tiles.
