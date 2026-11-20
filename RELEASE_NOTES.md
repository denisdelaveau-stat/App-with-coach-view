# Volley Live Capture v1.8.0 — Release Notes

## Coach View
A new `COACH VIEW` button on Home opens a dedicated live-analysis interface inspired by the four supplied visual references. It contains one-tap navigation between `Vue coach`, `Équipe` and `Joueurs`, plus the complete Player Detail page.

## Live overview and rotations
The Overview displays the score, set status, rotation/phase context, six sample-qualified KPIs, the current court, recent-rally momentum and one priority signal. Rotation Analysis adds P1–P6 and phase filters, selected-rotation context, court reconstruction and transparent rally differentials.

## Players and detail
Players can be filtered by presence and role. Ranking uses the explicit `points − errors` delta rather than an unexplained score. The approved `Voir le détail joueur` CTA opens the selected player with period, rotation, phase and skill context retained; browser and in-page Back paths restore the Players screen.

## Data, responsive UI and PWA
Live data comes from the existing match and event stores. Without a saved match, the screen uses clearly labelled demonstration data. The UI supports 320 CSS px through desktop, keyboard focus and reduced motion. `coach.css` and `coach.js` are cached offline; the PWA cache is `volley-live-capture-v1.8.0`.

## Compatibility and validation
All v1.7.0 capture, setup, scoring, substitution, report and JSON features remain supported. JavaScript syntax validation and the complete automated suite pass: **28 tests passed**.

---

## v1.7.0 baseline retained

## New application entry flow
The Home screen now uses the user-supplied `Font_app_ref.jpg` artwork. The active match appears inside `CONTINUE / VIEW MATCH`, `OPEN MATCH .JSON` is renamed `OPEN ARCHIVES`, and the separate Statistics control is removed. Teams and Settings are directly accessible from Home.

## Reusable Teams
A single editor now creates, loads, clones, edits, deletes and saves team rosters. Players use jersey numbers 1–40 and the established SET/OH/MB/OPP/LIB color system. Match-specific Focus selection is intentionally excluded from reusable team data.

## New Match
The match flow selects a saved team, confirms player presence and Focus tracking, then builds the initial court from the setter's P1–P6 position. The S → OH1 → MB1 → OPP → OH2 → MB2 sequence preserves opposite role pairs. Service/Reception selection updates the preview; the libero starts on the bench and can replace a back-row MB in Reception.

## Settings
Match format and capture detail level are now configured in Settings and applied to new matches.

## Compatibility
Existing capture, scoring, substitutions, reports and format-version-1 JSON files remain supported. The PWA cache is `volley-live-capture-v1.7.0` and includes the supplied Home artwork.
