# 🚌 CampusRide – Shuttle Seat Request System

A single-page web app where students request campus shuttle seats, and requests are tracked, searched, edited and approved in one place.
Built with plain **HTML, CSS and JavaScript** – no frameworks, no build step, no backend.

> CSE326 Student Project | 2026

## Features

- **Dashboard** – live counts of Total, Pending, Approved and Rejected requests
- **Seat request form** – name, student ID, department, route, pickup point, date, departure time, seats (1–4) and purpose of travel
- **Manage requests** – edit, delete, and change status (Pending / Approved / Rejected)
- **Search and filter** – by student name or ID, status, and route
- **Validation** – required fields, 1–4 seats, no past dates, and no duplicate request for the same student ID on the same date
- **Persistent data** – saved in the browser using `localStorage`
- **Safe output** – user input is HTML-escaped to prevent script injection
- **Responsive design** – works on desktop, tablet and mobile
- Toast notifications and smooth-scroll navigation

## Project Structure

```
CampusRide/
├── index.html    # Entire app (HTML + CSS + JS)
├── .nojekyll     # Tells GitHub Pages to skip Jekyll processing
└── README.md
```

## Run Locally

1. Download or clone the repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).

No installation or server needed.

## Deploy on GitHub Pages

1. Create a new repository on GitHub (e.g. `campusride`).
2. Upload `index.html`, `.nojekyll` and `README.md` to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*.
5. Select the `main` branch and the `/ (root)` folder, then click **Save**.
6. After a minute, your site will be live at:
   `https://<your-username>.github.io/<repository-name>/`

## How to Use

1. Click **Request a Seat** (or **Book Seat** in the menu).
2. Fill in the form and click **Submit Request**.
3. Open **My Requests** to see your bookings.
4. Use the dropdown in the *Status* column to approve or reject a request.
5. Use **Edit** to change details or **Delete** to remove a request.

## Tech Stack

| Layer   | Technology                          |
| ------- | ----------------------------------- |
| Markup  | HTML5                               |
| Styling | CSS3 (Grid, Flexbox, media queries) |
| Logic   | Vanilla JavaScript (ES6)            |
| Storage | Browser `localStorage`              |
| Font    | Inter (Google Fonts)                |

## Limitations

- Data is stored **only in the current browser**; it is not shared between devices or users.
- Clearing browser data will erase all requests.
- There is no login – anyone using the page can change request status. A real deployment would need a backend with authentication and an admin role.

## Possible Improvements

- Backend and database (e.g. Firebase, Node.js + MongoDB)
- Student login and a separate admin panel
- Seat-capacity limits per route and time slot
- Export requests to CSV
- Email or SMS notifications on approval

## License

Free to use for educational purposes.
