# Madaba Tourism Directorate – Official Website Prototype

## Project contents
- `index.html`: single-page application with separate navigable sections.
- `css/style.css`: responsive visual design.
- `js/i18n.js`: interface/content language dictionaries.
- `js/about-data.js`: localized Directorate profile, achievements, vision, mission, values, organizational chart, staff and tasks in the 11 supported languages (Arabic, English, French, German, Spanish, Italian, Russian, Chinese, Turkish, Hungarian and Bulgarian).
- `js/app.js`: navigation, language persistence, gallery lightbox, map initialization.
- `assets/`: supplied Ministry logo, Jordan brand mark, and Madaba Tourism Directorate building photo.
- `manifest.webmanifest`, `sw.js`: PWA basics for static hosting.

## Deploy to GitHub Pages
1. Create a NEW repository for this Directorate project; do not overwrite the Madaba Visitor Center repository.
2. Upload the contents of this folder (not the ZIP file) to the repository root.
3. Keep `index.html` at the root.
4. Enable GitHub Pages from the `main` branch and `/ (root)`.
5. Open the published URL and test the language menu and sections on mobile and desktop.

## Important publication and verification notes
- The complaints/suggestions section now displays the Directorate-approved receiving email (Madaba@mota.gov.jo), phone (+962 7 7227 8468), and responsible office (Director of Madaba Tourism Directorate). The form UI is prepared for attachments and eleven-language display. Submission and file upload remain disabled until a secure backend, database, admin authentication, storage, and email-notification service are configured and tested; no personal data is transmitted or stored by this static prototype.
- Directorate phone, email, exact address, working hours, exact site coordinates are placeholders pending official confirmation. The About the Directorate section now uses the supplied organizational chart and staff details.
- The map initially marks the general Madaba city area, not a verified building entrance or all tourism sites.
- Images other than the supplied Directorate building and supplied Ministry/Jordan marks are not used as factual site photographs. The gallery is clearly labelled as temporary illustrative material.
- External Leaflet/OpenStreetMap tiles and Google Fonts require an internet connection. The main site remains usable without map tiles, but interactive maps will not load offline.
- Ministry reference sections and national strategy links point to official Ministry websites. Review links before formal government publication.


## Phase 1: official content additions
- Added the Ministry's visa notice, fees and exact Arabic wording from its visa page.
- Added the nine tourist-guide qualification conditions and course duration note from the Ministry page.
- Added links to Ministry tourism-profession categories and the service-card titles surfaced in the official site listing.
- Added links to the official profession guide PDF, start-your-tourism-business procedures, e-services portal and e-services user guide.
- Ministry PDF download endpoints timed out during retrieval. Original PDF files are linked at their Ministry pages and are not bundled locally yet.
- The e-services portal displays a notice that several tourism-establishment licensing services were moved to other regulatory entities under the 2024 Tourism Law amendment and stopped on that portal.


## Phase 2: official regulations and direct service-card PDFs
- Added the Ministry's current regulations listing, which currently displays regulations dated 2025 and 2026.
- Expanded the start-your-tourism-business listing description to reflect the categories currently displayed by the Ministry.
- Added direct official PDF links for the tourist-guide first-time licence, adding a language to a guide licence, and renewing a tourist-guide licence.
- Updated the first-time guide licensing, adding-language, and renewal service cards to open their identified PDF files directly.
- Added an explicit note that the Ministry's e-services user guide contains video tutorials.
- The remaining service cards still open the official service-card listing because individual verified PDF destinations were not identified for each one. No missing service details have been invented.
- The Arabic Ministry material remains Arabic in this phase. The site's existing ten-language interface is retained; these new official sections have not yet been fully translated into all ten languages.
- PDF links open on the Ministry's website; the PDF files themselves are not copied into this project archive.


## Phase 3: service-card links and Madaba Directorate contact
- Preserved the exact eleven service titles displayed on the Ministry's official service-cards page.
- Added direct PDF destinations for six cards where the exact official PDF URL was verified: adding a language, renewing a tourist-guide licence, first-time tourist-guide licence, temporary tourist-accompaniment permits, heritage-building rehabilitation/development, and classification-grade/category or facility addition.
- The other five service cards open the official Ministry listing page. Their cards explicitly say that an individual PDF link was not verified; no guessed PDF URLs were added.
- Added the Ministry-published contact details for Madaba Tourism Directorate: main phone 0096264603360, extension 751, and the published address entry "Madaba". No unverified local street address, email, or local working hours were added.
- These added Arabic official service titles and contact details are displayed in Arabic; the original ten-language site interface remains intact. This phase does not claim that every new official content paragraph has been translated into all ten languages.


## Complaints and suggestions – pre-publication setup
- Receiving office: Director of Madaba Tourism Directorate.
- Official receiving email: Madaba@mota.gov.jo.
- Directorate phone: +962 7 7227 8468.
- Requested workflow: email notification plus an authenticated admin dashboard, file attachments, and an automatic receipt confirmation.
- These requirements are recorded in the interface, but actual submission is deliberately not enabled in the static prototype. Before publication, connect a secure backend and verify database access rules, private file storage, admin sign-in, email delivery, and confirmation messages. Do not place service-role secrets or SMTP credentials in browser JavaScript.


## Interactive Madaba tourism map – draft implementation
- Added the supplied Madaba tourism brochure image as the primary static map image.
- Added an interactive Leaflet map and a searchable/filterable directory of the 19 locations explicitly confirmed by the user.
- Added multilingual site names and interface controls for all eleven site languages.
- Added Google Maps search/directions links for each location.
- Map pins are currently resolved at runtime using the OpenStreetMap Nominatim geocoder and cached locally in the visitor's browser. This is not the same as extracting and validating exact Google Maps coordinates; pin placement and visitor entrances still require a final site-by-site verification.
- Site detail descriptions are available in Arabic and English; other languages currently use the English description fallback. Verified site photographs have not yet been bundled, so per-site photo galleries remain outstanding.
- The brochure image, interactive map, list and details are responsive. External map tiles/geocoding require an internet connection.

## Interactive Madaba map update
- The supplied Madaba tourism brochure is retained as the map image.
- The interactive directory contains 19 approved locations, translated site names, categories, and short descriptions in all 11 site languages.
- Verified Jordan Tourism Board image assets are displayed for locations where a matching official image was available. Locations without a confirmed matching image do not use a guessed photograph.
- Directions open Google Maps using the site's search name. Marker coordinates are currently resolved through OpenStreetMap Nominatim at runtime; they are not Google Maps-sourced coordinates and should be field-checked against visitor entrances before public launch.
- The service worker cache version was incremented to refresh updated map files.
