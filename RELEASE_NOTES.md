## Environment API endpoints, snapshot 15 Nov 2026

- 174,406 endpoints passed a keyless data call, tested 14–15 Nov 2026 (IST)
- 11,421 services · 251 country codes · 117,721 keyless JSON rows

### Download

- `Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 174,406 rows, 8.2 MB gzipped (54.8 MB as CSV), SHA-256 `1c3a65098508df0afee82bbfebab89b0921cf35239b85738f5b434a64a7948de`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 34,035 · Wrap one URL pattern as a get_species_records tool: pass a country code and a group, return species names, dates and coordinates; page with offset for more.
- 📱 App features: 5,880 · Draw protected areas, habitats, tree cover, noise zones, contaminated sites or waste points as a map layer, and show the nearest one on a card.
- 🧠 Grounding and data pipelines: 13,026 · Load emissions, waste, forest and radiation series on a schedule into your own store, so answers about the environment cite a dated source.
- 🧪 Evals and testing: 174,406 · Run your environment tool against a fixed set of URLs across formats; check that species, pollutant, value, unit and date parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 962 rows whose URL carried a credential-looking parameter or a login.
- Left out: 2 rows with an email-like address.
- Left out: 2,510 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 24 layers marked editable in the title (they can hold entries that people added).
- Left out: 338 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 2 rows that passed a data call only from a network location in India.
- Left out: 6 rows whose address or title held a token-like string, a private address or a similar string.
- Left out: 731 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 93 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 13,423 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 405 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 4,612 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 1,448 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 587 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 4,201 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 12,408 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 117,721 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 40 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 11 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 1 of these URLs is also in 12k-parking-apis-for-agents.
- Overlap: 36 of these URLs are also in 10k-earthquake-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 14–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Environment API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
