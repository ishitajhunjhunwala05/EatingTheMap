# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

"Favorite Food Spots" - A single-page web app for saving and sharing restaurant locations on an interactive map. Built with Mapbox GL JS for mapping and Supabase for backend persistence.

## Architecture

**Single HTML File Application** (`index.html`)
- All HTML, CSS, and JavaScript in one file
- No build process or bundler required
- External dependencies loaded via CDN (Mapbox GL JS v3.9.4, Supabase JS v2)

**Configuration** (`config.js`)
- Contains Mapbox token and Supabase credentials
- Gitignored - must be created locally with `MAPBOX_TOKEN`, `SUPABASE_URL`, `SUPABASE_ANON_KEY`

**Data Layer**
- Supabase table: `FoodSpots` with columns: `id`, `Name`, `Description`, `Lat`, `Lng`, `created_at`
- CRUD operations via Supabase JS client

## Development

Open `index.html` directly in a browser - no server required for basic development. For geolocation features, serve via HTTPS or localhost.

## Key Code Patterns

- Map markers are DOM elements (`.pin-dot` class) created per spot
- Popups use Mapbox GL's Popup API with inline HTML forms
- User location shown as pulsing blue marker (`.user-marker`)
- Five map styles available: Streets, Satellite, Dark, Light, Outdoors
- Default center: Dubai (55.27, 25.2)
