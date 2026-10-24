# Voicu Eduard-Alexandru

Software developer. I mostly build web apps end to end, from the backend and the data
model to the page someone actually clicks on. Lately I've been working on projects where a language
model is one part of a bigger system, and on making sure it only does the part it's good at.

I like small, readable code, writing down why something works the way it does, and finishing what I
start. A good chunk of what's below was built at hackathons in 24 hours, the rest on my own time.

**Stack I use most:** Python, JavaScript / TypeScript, Node.js, React / Next.js, FastAPI, Express,
PostgreSQL, SQLite, Docker, Git. Also MATLAB / Octave for numerical work.

---

## Projects

### [AccessRoute](https://github.com/edvt-exe/AccessRoute)
`Next.js` `React` `TypeScript` `Tailwind` `Zod` `Vitest`

Voice guidance for blind and partially sighted people on their first days at a new job. A colleague
walks a room once with their phone (steps counted from the walking rhythm, turns from the gyroscope),
marks the corners, places and obstacles, and someone reviews the map before it goes live. After that
the new employee can ask "where's the coffee?" and gets guided there wall by wall, the way orientation
and mobility instructors teach it. Includes a first-day tour for HR and an accessibility report of the
office. Built in 24 hours with Ghiduc and Marcelin at the *First Job, Full Potential* hackathon.

### [TrueRoute AI](https://github.com/edvt-exe/TrueRoute-AI)
`Python` `FastAPI` `PostgreSQL` `SQLAlchemy` `Alembic` `Leaflet`

Plans multi-day walking trips in any city from real OpenStreetMap data. The idea behind it: the model
never writes a place name, coordinate or distance. Python geocodes the city, pulls places from
Overpass, ranks them, and hands the model only a list of references to pick and order. The answer is
forced through a JSON schema, validated again in Python, then routed on foot with openrouteservice
(OSRM as fallback). Also has full account handling: argon2id hashing, sessions, OTP, breached
password checks and rate limiting.

### [LeetCode Portfolio](https://github.com/edvt-exe/leetcode-portfolio) + [leetcode-explained](https://github.com/edvt-exe/leetcode-explained)
`JavaScript` `Node.js` `Express` `Chart.js` `GitHub Actions`

180+ problems solved in Python, each with its own notes. The portfolio site reads the solutions repo
through a sync script, builds a JSON database and serves it: filters, search, per-problem notes and
struggle ratings, analytics charts and a flashcard mode that shows the problems I missed more often.
A GitHub Actions workflow keeps it in sync.

### [VoiceCraft](https://github.com/edvt-exe/text-to-speech-app)
`Node.js` `Express` `SQLite` `Docker`

Text-to-speech web app. Instant preview in the browser with the Web Speech API, MP3 generation on the
server. Requests are hashed (SHA-256) so repeated text comes straight from the cache, which takes a
response from about 2 s down to under 50 ms. Shareable player links with OpenGraph previews, per-IP
rate limiting, and a multi-stage Docker image that runs as a non-root user.

### [FlashTickets](https://github.com/edvt-exe/FlashTickets)
`React` `TypeScript` `Python`

Event ticketing platform built in a team of two. I worked mainly on the backend: login and accounts,
billing and card logic, orders, interests and the recommendation part, plus some frontend pages.

### [LedHack](https://github.com/edvt-exe/LedHack)
`Python` `Pygame` `UDP`

Hackathon project: interactive games for a room with LED walls and buttons, driven over UDP with a
custom checksum. We wrote the controllers, a local simulator and several games (a Simon-style memory
game, a team game, a shooting game).

### [KMeans-Clustering](https://github.com/edvt-exe/KMeans-Clustering)
`Octave / MATLAB`

Image compression with K-Means, written from scratch with no ML functions, just to understand the
algorithm properly. Includes tests on hand-checked data and a comparison of quality vs. size for
different values of K.

### [StepBackLogo](https://github.com/edvt-exe/StepBackLogo)
`HTML` `CSS` `JavaScript`

A daily browser game: guess the brand from a heavily zoomed logo, and every wrong guess zooms out a
bit. Four difficulty levels, daily packs, streaks, tokens for hints and extra lives. No framework, no
backend, everything saved in localStorage.

---

## Other

- Hands-on Git, GitHub and Markdown workshops (the workshop repos are forked on my profile).
- Numerical methods work in MATLAB: kernel regression and anomaly detection.

## Contact

- GitHub: [@edvt-exe](https://github.com/edvt-exe)
- Email: eduardvoicu05@gmail.com
