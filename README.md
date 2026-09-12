# Busfest Wayfinder

A single-file web app for finding your way around Busfest at the Three Counties Showground, Malvern.
Open `index.html` on a phone (it needs HTTPS or `file://` for GPS to work).

- Pannable, pinch-zoomable official Busfest 2026 site map (embedded as a data URI).
- Live GPS dot with accuracy ring, placed on the map via an estimated north-up alignment.
- "Fix my position": tap where you actually are to correct the alignment. Two taps at well-separated
  spots also correct the map scale. Corrections are saved in `localStorage`.
- Place finder: stages, gates, camping zones, toilets/showers, first aid, security, ATM, food, trade.
  Each shows distance and compass direction from you, plus a dashed line on the map.
- "Pin my van" saves your pitch so you can navigate back to it.
- Compass cone where the browser exposes device orientation.

The printed compass rose on the official map is wrong; the map is north-up (Blackmore Park Road on the right,
Hanley Road along the bottom), and the app treats it that way.
