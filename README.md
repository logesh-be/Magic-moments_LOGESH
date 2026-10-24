# CampusConnect AI

**VecnaVerse National Level Hackathon 2026 | Domain: Software Development**
**Problem Statement:** Hyperlocal Event Discovery & Community Engagement

> Find your next opportunity. Connect beyond your campus.

CampusConnect AI is a web platform where students discover hackathons, workshops, symposiums, competitions, seminars and cultural events happening near them, and where organizers can post events and see how many people engage with them.

## Problem

Event information is scattered across WhatsApp groups, Instagram, LinkedIn, posters and individual websites. Students miss relevant events, and organizers struggle to reach the right audience nearby.

## Features

### For students
- **Category pages:** a dedicated page for Hackathons, Workshops, Symposiums, Competitions, Seminars and Cultural events.
- **Location-aware discovery:** filter by city (Indian city autocomplete), online or offline mode, fee and date.
- **Natural-language search:** type queries like `free hackathon near Chennai` or `online workshop`.
- **"For You" personalised ranking:** each event gets a match score (0-100%) with a transparent reason breakdown:
  interests (up to 50), skills (15), budget (up to 15), location or online (15), deadline urgency (5), verified listing (5).
- **Event detail page:** venue, address, fee, dates, tags and organizer contact (call / email).
- **Google Maps integration:** embedded map, "View on Google Maps" and "Get directions" for offline events.
- **Deadline tracker:** saved events sorted by registration deadline, with days-left countdown.
- **Registrations:** register or cancel, and view all your registrations.
- **Share:** copy event details to the clipboard to send to friends.
- **Closing soon** section on the home page to drive timely registrations.

### For organizers
- **Easy event posting:** create, edit and delete events (title, category, mode, venue, address, fee, dates, tags, registration link, contact details).
- **Validation:** deadline must be on or before the event date; offline events need a venue or address.
- **Engagement analytics:** per-event views, saves and registrations.
- **Verified badge** on trusted listings; new posts are marked pending review.

### General
- Light and dark theme toggle.
- Responsive layout (mobile friendly) and keyboard accessible.
- Data persisted in the browser (`localStorage`) with a **Reset demo data** button.
- 30+ seeded events across Chennai, Bengaluru, Hyderabad, Mumbai, Delhi, Pune, Kolkata, Kochi, Ahmedabad, Jaipur and more.

## Tech Stack

- HTML5, CSS3 (custom properties, responsive grid), vanilla JavaScript (ES6)
- Browser `localStorage` for persistence
- Google Maps embed and directions links
- Google Fonts (Inter, Bricolage Grotesque)
- No build step and no dependencies

## How to Run

```bash
git clone <your-repo-url>
cd CampusConnect-AI
# Option 1: just open index.html in a browser
# Option 2: serve locally
python3 -m http.server 8000   # then open http://localhost:8000
```

## Project Structure

```
CampusConnect-AI/
├── index.html   # complete application (UI, logic, seed data)
├── README.md
└── .gitignore
```

## How the Recommendation Score Works

The ranking is rule-based and explainable, so every event card shows *why* it was recommended (for example "Matches your interest in AI (+25)").

## Roadmap

- Backend (Node.js / Firebase) with real user accounts
- Real GPS-based "near me" sorting
- Organizer verification workflow and admin review
- Push / email reminders for deadlines
- Community features: follow organizers and clubs, event reviews, attendance streaks

## Team

Team Name: Magic Moments
Team Members: G Soorya Parkash, V A Moneshwaran , S Mozhiyarasu
