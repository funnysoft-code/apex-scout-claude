---
name: find-a-track-day
description: Use when a person asks about track days, open pit lane days or booking a day at a race Circuit in Europe, for example "any track days at Portimão in March?" or "where can I drive my car on track in Spain?".
---

# Find a track day

Help a Driver find a Listed Day with the Apex Scout connector. A Listed Day is a day an organiser opens for booking at a Circuit.

## Steps

1. Ask for what is missing: the country, the Circuit and the dates. One short question is enough; do not ask for what the Driver already said.
2. Call `find-listed-days` with the country (two letters, such as PT or ES), the Circuit, and `from` and `to` as YYYY-MM-DD. Pass `language` when you know the Driver's language, so the links open in it.
3. Show each Listed Day with its date, Circuit, organiser, price and link. Give the price as the tool returns it, and say so when none is shown. Keep the list short and in date order.
4. Booking always happens on the organiser's own site. Send the Driver there, using the link the tool gives (for the organiser's website, call `get-organiser`). Apex Scout does not sell or hold places.
5. For follow-ups, call `get-circuit` (facts about a Circuit and its upcoming days) or `get-organiser` (the organiser's details and upcoming days).

## Rules

- Never invent a Listed Day, a price, a date or an organiser. Say only what the tools return.
- When the tool says more days exist, tell the Driver and offer to narrow by dates or Circuit.
- When nothing is listed, say so plainly and suggest nearby dates or nearby Circuits, then search again if the Driver agrees.
- If a Circuit is not found, say so and search by country instead.
