# Orbis Forum

**Conference management platform built to make offline events fully digital.**

Orbis Forum replaces paper chits, printed schedules, clipboards, and manual attendance tracking with a real-time mobile and web application. Built solo by Thakur Garg, Grade 12, Strawberry Fields High School, Chandigarh.

This repository is a **showcase** of the project — README, screenshots, and live deployment stats. The full source code is proprietary and kept in a private repository.

---

## Deployed At

**SFHS MUN and PDC 2026**
Strawberry Fields High School Model United Nations Conference and Parliamentary Debate Championship
May 14–16, 2026, Chandigarh, India

Participating schools: Strawberry Fields High School, Vivek High School, The Shri Ram School, Pinegrove, Yadavindra Public School, Bhavan Vidyalaya Chandigarh, La Martiniere College, St. Kabir Public School, Holy Angels, KK Blossoms, First Steps School, Chitkara, and S.D. Vidya.

---

## Live Stats from Deployment

| Metric | Value |
|---|---|
| Total registered users | 419 |
| Peak daily active users | 150 |
| Monthly active users | 213 |
| Total Firestore reads | 153,000 |
| Total Firestore writes | 6,100 |
| Peak simultaneous listeners | 68 |
| Peak active connections | 37 |
| Data served | 475.12 MB |
| Storage used | 193.47 MB |
| Downtime | 0 |

---

## Screenshots

### Login Screen
![Login Screen](screenshots/login.png)

### Dashboard
![Dashboard](screenshots/dashboard.png)

### Chit System
![Chit Screen](screenshots/chits.png)

### Firebase — Live User Activity (150 Peak DAU, 213 MAU)
![Firebase Auth Stats](screenshots/firebase_auth.png)

### Firebase — Hosting Traffic (475 MB served)
![Firebase Hosting Stats](screenshots/firebase_hosting.png)

### Firebase — Database Operations (153K reads)
![Firestore Stats](screenshots/firestore_stats.png)

---

## Features

**Delegate Access**
- Personal QR code for entry and meal scanning
- Real-time chit passing with chairs and other delegates
- Committee announcements feed
- Event schedule and documents
- Committee and portfolio information
- Awards announcements

**Organising Committee**
- QR-based delegate entry scanning
- QR-based meal coupon scanning
- Announcements management
- Delegate directory

**Executive Board (Chairs)**
- Committee attendance tracking
- Chit moderation and delivery
- Awards submission

**Admin**
- Full user management with role assignment
- Bulk user import via Excel
- Meal configuration
- Attendance confirmation
- Real-time notifications to all users
- Database management

**Parliamentary Debate (PDC) Module**
- Separate PDC dashboard
- Team and adjudicator management
- Round pairings and scheduling
- Live ballot submission by adjudicators
- Automatic tabulation and leaderboard
- Results release

**Other Roles**
- TIC (Teacher In Charge) — school delegate supervision
- Security — entry scanning only dashboard

---

## User Roles

| Role | Description |
|---|---|
| admin | Full platform access |
| eb | Executive board — chairs, vice chairs, rapporteurs |
| oc | Organising committee — general, F&B, IP, PDC subtypes |
| tic | Teacher in charge |
| security | Entry scanning only |
| delegate | Standard conference access |
| pdc_team | PDC debate team member |
| pdc_adjudicator | PDC judge |
| pdc_core_adjudicator | PDC head judge |

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Flutter (Dart) |
| Mobile | Android APK |
| Web | Flutter Web |
| Database | Firebase Firestore |
| Authentication | Firebase Auth |
| Hosting | Firebase Hosting |
| Domain | app.sfhsmun.com |

Built on **94 dependencies** across the app and CI pipeline — Firebase SDKs, Flutter platform plugins, and GitHub Actions for deployment.

---

## Distribution

- Delegates accessed the web app via link and QR code at app.sfhsmun.com
- Android users installed via APK shared through the app's announcements
- iOS users accessed the web app as a PWA
- OC team used the Android APK for camera-based QR scanning

---

## Architecture Highlights

- Role-based access control across 9 distinct user roles
- Real-time Firestore listeners across all active screens
- QR code generation per user, linked to their UID
- Dual-app system — MUN and PDC modules accessible from one login
- Code of Conduct gate for delegates before dashboard access
- Bulk user import system via Excel to Firebase Admin SDK
- End-of-day reset system for entry and location data

---

## Development Timeline

Built solo over 5 weeks, from empty repo to a production app running a live 3-day, 300+ participant conference:

| Date | Milestone |
|---|---|
| Apr 10 | Initial app setup, base user screen |
| Apr 21 | Role restructure — IP/F&B roles, admin chits, announcements |
| Apr 25 | Meals, scanner, QR entry system |
| Apr 29 | Core MUN feature set complete |
| May 6 | Parliamentary Debate Championship (PDC) module built |
| May 10 | Feature-complete app |
| May 11–13 | Firebase Hosting integration, final polish |
| May 14 | **Shipped — final app deployed for the live event** |

---

## Business

Orbis Forum is being developed as a commercial product for conference organizers. Trademark application filed for the name and logo under Software Applications and Event Planning/Organizing categories.

Target: 50+ events. Pricing: Rs. 5,000–15,000 per event.

---

## License

This repository is a showcase only. Source code is proprietary and not included here — all rights reserved.

---

## About

Built by Thakur Garg
Grade 12, Strawberry Fields High School, Chandigarh
Founder, Orbis Forum
