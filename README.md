# FindBack — Web-Based Lost and Found Management System for Addis Ababa

## About FindBack

**FindBack** is a centralized, web-based lost-and-found management platform designed for students, commuters, and residents in **Addis Ababa**.

Today, recovering lost belongings in Addis Ababa mostly relies on unstructured Facebook/Telegram posts and physical notice boards, where reports get buried quickly, key details (area, landmark, date) are missing, personal information (IDs, phone numbers) is exposed publicly, and fake claims are hard to prevent.

FindBack solves these gaps with:
- **Structured Reporting:** Guided lost-item and found-item forms requiring category, Addis Ababa area (e.g., Bole, Piassa, Mercato, Arat Kilo, Megenagna), landmark, date, and clear field examples.
- **Search & Match Suggestions:** Keyword search, multi-criteria filtering, and automatic match scoring (`≥ 0.60` threshold) pairing lost and found reports.
- **Privacy-First Ownership Verification:** Finders can store one **hidden private identifying detail** (e.g., phone wallpaper or charger brand) that is never shown publicly; claimants must describe it to prove ownership, and sensitive photos (e.g., IDs/wallets) are displayed blurred.
- **In-App Messaging & Handover Points:** Owner and finder coordinate safely inside the platform without sharing phone numbers, with optional physical handover locations (e.g., campus security offices).
- **Full Status Lifecycle:** Every report moves through clear, tracked stages:  
  `Active` → `Potential Match Found` → `Verification in Progress` → `Recovered` → `Closed`
- **Administrator Oversight:** Moderation tools for flagged reports, ownership disputes, user accounts, and system summaries.

---

## Frontend Project Structure

```text
findback/
├── index.html                  # Home page
├── pages/
│   ├── login.html              # Login page
│   ├── register.html           # Registration page
│   ├── profile.html            # User profile page
│   ├── dashboard.html          # User reports & notifications
│   ├── report-lost.html        # Report lost item form
│   ├── report-found.html       # Report found item form
│   ├── browse.html             # Search & filter items
│   ├── item-detail.html        # Single item details
│   ├── matches.html            # Suggested matches
│   ├── claim-verify.html       # Claim & ownership verification
│   ├── messages.html           # In-app chat
│   └── admin.html              # Admin dashboard
├── css/
│   ├── style.css               # Shared styles (colors, navbar, footer)
│   ├── home.css                # Home page styles
│   ├── account.css             # Login, register, profile & dashboard styles
│   ├── report.css              # Lost & found form styles
│   ├── browse.css              # Browse & item detail styles
│   ├── recovery.css            # Matches, verification & chat styles
│   └── admin.css               # Admin dashboard styles
├── js/
│   └── main.js                 # Shared UI scripts
├── assets/
│   └── images/                 # Icons & sample images
└── README.md
```

---

## Frontend Work Division

| Area | Files |
| :--- | :--- |
| **Shared Layout & Home Page** | `css/style.css`, `index.html`, `css/home.css`, `js/main.js` |
| **Auth, Profile & User Dashboard** | `pages/login.html`, `pages/register.html`, `pages/profile.html`, `pages/dashboard.html`, `css/account.css` |
| **Lost & Found Reporting Forms** | `pages/report-lost.html`, `pages/report-found.html`, `css/report.css` |
| **Browse Catalogue & Item Detail** | `pages/browse.html`, `pages/item-detail.html`, `css/browse.css` |
| **Matches, Verification & Chat** | `pages/matches.html`, `pages/claim-verify.html`, `pages/messages.html`, `css/recovery.css` |
| **Admin Dashboard** | `pages/admin.html`, `css/admin.css` |

---

## Collaborators

- Adonias Hailu — `ETS0103/17`
- Abemelek Samson — `ETS0043/17`
- Awach Awach Garang — `ETS1869/17`
- Biniam Girma — `ETS0312/17`
- Befikir Shimelis — `ETS0237/17`
- Abel Gebregziabher — `ETS0028/17`
