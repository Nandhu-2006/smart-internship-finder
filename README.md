# Pathway — Smart Internship Finder

A beginner-friendly student career app built with plain HTML, CSS, JavaScript, and localStorage. It works as a responsive mobile-style web page and needs no server or package installation.

## Run it

1. Open this folder and double-click `index.html` to launch it in a modern browser.
2. Choose **Create account** and enter your student name, email, password, college, department/course, and year of study.
3. Add skills in **My Profile** to see skill-based recommendations.

For the demo Admin workspace, choose **Admin** at sign-in and use:

- Email: `admin@pathway.demo`
- Password: `admin123`

## Student features

- Student registration and login, including college, course/department, and study year.
- Home dashboard with welcome, internship categories, recommended roles, and latest company listings.
- Search plus filters for domain, location, internship type, paid/unpaid stipend, and duration.
- Internship detail pages with company, role, skills, duration, stipend, eligibility, deadline, source, and Google Maps search.
- **Apply now** opens the external employer page for source-verified listings and adds a record to the local demo tracker. It does not submit an application on your behalf.
- My Applications supports Applied, Under Review, Shortlisted, Rejected, and Selected statuses for demonstration. These statuses do not come from employers.
- Saved internships, skill-based recommendations, and notifications for skill matches, admin-added demo listings, demo status changes, and approaching admin-demo deadlines.
- My Profile stores name, college, department, year, skills, project/certificate notes, and GitHub/LinkedIn links. Choosing a resume only stores its file name; the file is not uploaded.
- Courses includes beginner, intermediate, and advanced Java, Python, SQL, web development, and developer-tools resources.

## Admin demo

Admin can add, edit, and remove locally created demo internships, remove expired admin-demo listings, view student accounts and application records, and pause or restore demo student access. New admin entries appear in the student internship list. Verified company listings are protected from editing/deleting in this demo.

## Listing accuracy and external services

Company listings were checked against linked employer pages on October 26, 2026. Openings can close or change; the employer page is authoritative. If stipend or deadline is not published, the app says so rather than guessing. The **Search live internship listings on the web** button opens Google Search; this static app does not scrape or sync search results. Google Maps opens a map search for the stated location; an embedded Maps API integration would need an API key and backend configuration.

Admin-added listings, account data, saved roles, applications, and notifications are local demo data. They are stored in this browser and do not sync between users/devices. The demo has no backend, password encryption, real email verification, company ATS connection, or secure upload. Do not enter real passwords or sensitive documents.

## Files

- `index.html` — sign-in, student dashboard, profile, applications, and admin views.
- `styles.css` — responsive purple, pink, and charcoal app styling.\n- `pathway-motion-logo.svg` — original animated isometric career-growth logo, also used as the app favicon. It stops moving when reduced motion is enabled.
- `app.js` — source-checked listings, courses, sign-in, filters, recommendations, demo applications, notifications, admin tools, and local storage.

To add a verified listing, update `verifiedListings` in `app.js` and include the employer source, checked date, published stipend/deadline details, skills, eligibility, and location. If the source does not say, use “not stated.”
