# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 174,406 endpoints from 11,421 services, tested 14–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- The repository holds a 1,000-row sample and the services list; the full list is the release download Environment_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 170k-environment-apis-for-agents (was environment-api-endpoints).
- Left out: 962 rows whose URL carried a credential-looking parameter or a login.
- Left out: 2 rows with an email-like address.
- Left out: 2,510 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 24 layers marked editable in the title (they can hold entries that people added).
- Left out: 338 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 2 rows that passed a data call only from a network location in India.
- Left out: 6 rows whose address or title held a token-like string, a private address or a similar string.
- Left out: 731 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 93 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
