# Nursery Rota

A single-page tool for building a fair rotating volunteer schedule for a church nursery. No build step, no dependencies, no server.

## Use it

Open `index.html` in a browser, or publish it with GitHub Pages (Settings > Pages > Deploy from branch > `main` / root).

1. Set the first date, number of weeks, services, and how many leads and helpers each service needs.
2. Add volunteers, mark who is lead-qualified, and add the dates each person cannot serve.
3. Press **Build schedule**. Change any spot from its dropdown, then use **Copy as text** to share it.

Data is stored only in your browser (localStorage). It is not sent anywhere.

## Scheduling rules

- Nobody is scheduled on a date they marked unavailable, or beyond their monthly maximum.
- Lead spots go only to lead-qualified volunteers; leads can also fill helper spots.
- People with fewer turns so far are picked first. Optionally avoids back-to-back Sundays and more than one service per Sunday.
- Spots that cannot be filled are shown as open.
