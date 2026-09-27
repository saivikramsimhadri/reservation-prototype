# Reservation Assistant Prototype

Mid-fidelity clickable prototype for MSMA 5033 Human-Computer Interaction, Module 5.

**Live:** https://saivikramsimhadri.github.io/reservation-prototype/

## What this is

A reservation assistant that parses a booking request into editable constraint chips,
then refuses to book while any constraint is unverified.

Eight states from an open composer to a completed booking, with a branch at state 4.
The parse on that screen reads "party of 5" against a request for 6. The error is
deliberate: the prototype exists to test whether a user notices and corrects it before
booking.

## AI interaction states

| State | Type | Behavior |
|---|---|---|
| 3 | Loading | Four chip outlines preview the shape of the result instead of a spinner |
| 4 | Explainability | The parse is shown before any search runs |
| 5 | Error recovery | Inline editor quotes the original message as evidence |
| 7 | Uncertainty | Verification source per row; confirm disabled while one row is unverified |

## Running it

Single file, no build step and no dependencies. Open `index.html` in any browser.

Sai Vikram Simhadri
