# Moonlight Rental Car — Operations Console (Prototype)

A visual prototype of a car rental operations platform: Dashboard, Fleet, Rentals, Reservations, Customers, SunPass, Payments, Maintenance, and Settings.

## What this is

This is a **static, front-end-only prototype** built for review and demonstration purposes. It is a single self-contained `index.html` file — there is no server, no database, and no real backend. All data (vehicles, rentals, customers, payments, etc.) is fictional sample data generated for demonstration and lives only in the browser's memory while the page is open. Refreshing the page resets any changes made during a session (e.g. converting a reservation to a rental, marking a rental as returned, editing notes).

There is a small "Prototype" indicator in the top bar of the app to make this clear to anyone viewing it.

## Running it

Because it's a single static HTML file, there is nothing to install or build. Two ways to view it:

- **Locally:** open `index.html` directly in any modern desktop browser (Chrome, Safari, Edge, Firefox).
- **Deployed:** this project is set up to be hosted as a static site on [Vercel](https://vercel.com), which serves `index.html` as the site's homepage with no build step required.

## Project structure

```
index.html   → the entire application (markup, styles, and logic in one file)
```

## Notes for future development

The in-app data layer is organized behind a small `api` accessor object inside `index.html`, so a real backend (database + authentication + payment processing) could be connected later without restructuring the UI layer.
