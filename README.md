# FMA at Hofstra Website

Official website for the **Financial Management Association (FMA) at Hofstra University**, built to provide students with a centralized place to learn about the organization, explore upcoming events, meet the executive board, view chapter activities, and get involved.

## About the Project

The FMA at Hofstra website was created to strengthen the chapter's digital presence and make information about the organization more accessible to students.

Rather than relying on scattered social media posts and external platforms, the site brings together FMA's events, leadership, professional development opportunities, chapter resources, and membership information in one place.

The website is currently built as a lightweight static application using **HTML, CSS, and vanilla JavaScript**, allowing it to be hosted easily through platforms such as GitHub Pages without requiring a backend.

## Features

The website includes:

- **Responsive Landing Page** — Branded homepage introducing FMA at Hofstra and its mission.
- **About FMA** — Overview of the Hofstra chapter and its affiliation with FMA International.
- **What We Offer** — Professional development opportunities including guest speakers, networking, stock pitches, workshops, career development, and quantitative competitions.
- **Dynamic Event Calendar** — Events are automatically classified as upcoming or past based on their dates.
- **Event Details** — Visitors can view event descriptions, locations, times, and event categories.
- **Google Calendar Integration** — Events can be added directly to a user's Google Calendar.
- **Executive Board Directory** — Displays FMA leadership with roles, academic information, LinkedIn profiles, and contact information.
- **Photo Gallery** — Highlights chapter meetings, competitions, professional events, and social activities.
- **Chapter Merchandise** — Dedicated section for FMA apparel and merchandise.
- **Member Testimonials** — Highlights experiences and outcomes from FMA members.
- **Membership Section** — Provides students with information about joining the organization.
- **GroupMe and Social Links** — Direct access to FMA's communication and social platforms.
- **Live Financial Market Content** — TradingView integrations provide market information directly on the website.

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- TradingView Widgets
- Google Calendar Integration
- GitHub Pages

No frontend framework or backend is currently required.

## How the Site Works

Much of the site's content is stored in JavaScript arrays and objects.

For example:

```javascript
const EVENTS = [
  {
    title: 'Event Name',
    date: '2026-10-20',
    time: '8:00 PM',
    location: 'Zoom',
    tag: 'Guest Speaker',
    desc: 'Event description'
  }
];

The JavaScript dynamically renders this information into the corresponding sections of the website.

This makes it possible to update events, officers, testimonials, offerings, merchandise, and gallery content without rebuilding the site's HTML structure.

Event Management

Events are automatically separated into Upcoming Events and Past Events based on the current date.

function isPastEvent(ev) {
  const d = new Date(ev.date + 'T23:59:59');
  return d < new Date();
}

This allows the website to maintain an event archive automatically as the semester progresses.

Project Structure
fma-hofstra/
│
├── index.html
├── README.md
└── LICENSE

The current version is intentionally lightweight, with the majority of the website contained within index.html.

Running Locally

Clone the repository:

git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git

Navigate into the project:

cd YOUR-REPOSITORY

Then open index.html in your browser.

For the best development experience, the site can also be served using a local development server such as VS Code Live Server.

## Deployment

The website can be deployed using GitHub Pages.

Open the repository on GitHub.
Navigate to Settings → Pages.
Select the branch containing the website.
Select the root directory.
Save the configuration.

GitHub will generate a public URL for the website.

## Future Development

Potential future improvements include:

Administrative dashboard for chapter leadership
Database-backed event management
Online RSVP system
Alumni directory
Member authentication
Automated event registration
Expanded photo gallery
Internship and job opportunity board
Newsletter integration
Analytics dashboard
Content management system for future FMA boards
Organization

Financial Management Association at Hofstra University

Zarb School of Business
Hofstra University
Hempstead, New York

FMA at Hofstra connects students with finance professionals, alumni, faculty, and fellow students through professional development, networking, competitions, workshops, and educational programming.

Connect With FMA
Instagram: @fma.hofstra
LinkedIn: FMA at Hofstra University
Hofstra GetInvolved: Financial Management Association
Email: fma@pride.hofstra.edu
Contributing

This repository supports the FMA at Hofstra chapter website.

Future executive board members maintaining the website should carefully review JavaScript data objects before committing changes. Because the site dynamically renders several sections from JavaScript, a syntax error in a data object can prevent multiple sections from rendering.

## When making updates:

Create or update the appropriate content entry.
Verify JavaScript syntax.
Test the website locally.
Confirm links and images load correctly.
Commit changes with a descriptive commit message.
Deploy the updated version.
Maintainer

Developed and maintained for the Financial Management Association at Hofstra University.

FMA at Hofstra University
Bridging theory and practice.
