Ersona Dental Live Demo

Important Notice: This repository contains a web-based live demo of the Ersona Dental application, which is a fully functional, cross-platform app built using C# with .NET MAUI on .NET 8, targeting iOS, Android, Windows, and macOS. The real MAUI app includes native performance, advanced features like appointment booking, and potential backend integration (e.g., SQLite or REST API). This demo, built with HTML5, CSS3, and JavaScript, is a lightweight preview of the MAUI app’s frontend UI and navigation, designed for stakeholders to explore the app’s look and feel in a browser without native dependencies.

Overview
The Ersona Dental Live Demo showcases the UI and core functionality of Dr. Mina Emad’s dental clinics in Cairo, Egypt, including clinic details, appointment schedules, and a before/after gallery. It supports bilingual English/Arabic text with RTL (right-to-left) layout for Arabic, mimicking the MAUI app’s mobile-first design (375px width) while being responsive for desktop.
The primary .NET MAUI app offers native performance, cross-platform support, and advanced features (e.g., offline data, push notifications) not present in this static demo.
Features
Live Demo (Web)

Bilingual Support: Toggle between English and Arabic with dynamic RTL layout adjustments.
Mobile-First Design: Optimized for 375px width, centered on desktop with a clean, modern UI.
Navigation:
Homepage with clinic and feature cards.
Burger menu for Share and About Developer pages.
Dedicated pages for About Dr. Mina Emad, clinic details, appointments, before/after, and contact.


Clinic Information: Static details for Maadi, El Ahram, and Helwan clinics (hours, contact, location).
Interactive Elements:
Language toggle button in header (العربية/English).
Dynamic clinic details via query params (e.g., clinicdetails.html?clinic=maadi).
Language preference saved using localStorage.


Accessibility: Semantic HTML, lang attributes for screen readers.

.NET MAUI App (Primary App, Not Included)

Cross-Platform: Native support for iOS, Android, Windows, and macOS using a single codebase.
Advanced Features: (Planned or implemented) Appointment booking, offline data caching, push notifications.
UI: Built with XAML and C# using MVVM pattern, mirroring the demo’s design.
Backend: (TBD) Likely uses SQLite or REST API for data management.
Performance: Native rendering for smooth, platform-specific experience.

Tech Stack
Web Demo

HTML5: Page structure for all pages.
CSS3: Styling with CSS variables, RTL support, and Google Fonts (Cairo for Arabic, Arial fallback).
JavaScript: Handles language toggle, burger menu, and clinic details navigation.
Assets: Images (png, jpg, webp) and SVGs for UI elements.

.NET MAUI App (Reference)

Framework: .NET MAUI (.NET 8)
Language: C#
UI: XAML with MVVM architecture
Dependencies: (TBD, e.g., CommunityToolkit.Mvvm)
Platforms: iOS, Android, Windows, macOS

Project Structure
ersona-dental-live-demo/
├── about.html              # About Dr. Mina Emad page
├── aboutdev.html           # About the developer (Mina Malak) page
├── appointments.html       # Clinic schedules page
├── beforeafter.html        # Before & After gallery page
├── clinicdetails.html      # Clinic details page (query-based)
├── contact.html            # Contact information page
├── index.html              # Homepage
└── rec/
    ├── css/
    │   └── styles.css      # Unified stylesheet with RTL support
    └── imgs/
        ├── bfaf.jpg        # Before & After placeholder
        ├── clinic.png      # Clinic card placeholder
        ├── clininder.jpg   # Appointments card placeholder
        ├── contact.webp    # Contact card placeholder
        ├── devlogo.svg     # Developer logo
        ├── drimg.png       # Dr. Mina Emad image
        ├── tooth-icon.svg  # Burger menu icon

File Details

HTML Files:
index.html: Homepage with welcome section, clinic cards (Maadi, El Ahram, Helwan), and links to other pages.
about.html: Details about Dr. Mina Emad (profile, contact, bio).
aboutdev.html: Developer info (Mina Malak) with portfolio/GitHub links.
appointments.html: Clinic schedules (hours for Maadi, El Ahram, Helwan).
beforeafter.html: Placeholder gallery for treatment results.
clinicdetails.html: Detailed clinic info (hours, contact, location) with query-based navigation.
contact.html: Contact details for clinics (assumed to mirror clinicdetails.html).


CSS:
rec/css/styles.css: Unified styling with mobile-first design, CSS variables, and RTL support for Arabic.


Images:
Placeholders (bfaf.jpg, clinic.png, clininder.jpg, contact.webp) for cards and gallery.
devlogo.svg: Developer logo in aboutdev.html.
drimg.png: Dr. Mina Emad’s image.
tooth-icon.svg: Burger menu icon.



Setup Instructions
Running the Web Demo

Clone the Repository:
git clone https://github.com/your-username/ersona-dental-live-demo.git
cd ersona-dental-live-demo


Serve the Demo:

Use a local server (e.g., Python’s http.server, VS Code Live Server):python -m http.server 8000


Open http://localhost:8000 in a browser.


Dependencies:

Google Fonts CDN (internet required for Cairo font).
No external JavaScript libraries.


Customization:

Update data-en/data-ar attributes in HTML for translations.
Modify rec/css/styles.css for styling changes.
Replace placeholder images in rec/imgs/ with real assets.



.NET MAUI App (Not Included)

The primary MAUI app is a separate project, not in this repository.
Requires:
.NET 8 SDK
Visual Studio 2022 with MAUI workload
Xcode (iOS/macOS) or Android SDK (Android)


Contact the developer for access to the MAUI codebase or build instructions.

Usage

Language Toggle: Click “العربية” or “English” in the header to switch languages. Text and layout (RTL/LTR) update dynamically, with preferences saved in localStorage.
Navigation:
Homepage (index.html): Access clinic cards and More section links.
Burger menu: Navigate to Share and About Developer (aboutdev.html).
Clinic details: Click clinic cards (e.g., clinicdetails.html?clinic=helwan).


Limitations: Static demo with placeholder images/maps, no backend functionality.

Contributing
Contributions to the web demo are welcome. To contribute:

Fork the repository.
Create a branch: git checkout -b feature-name.
Make changes in HTML/CSS/JS under ersona-dental-live-demo/.
Commit: git commit -m "Add feature-name".
Push: git push origin feature-name.
Open a pull request with a clear description.

Guidelines:

Use 2-space indentation for HTML/CSS/JS.
Test changes in English and Arabic (RTL) modes.
Preserve mobile-first design (375px width).
Document changes thoroughly.

For MAUI app contributions, contact the developer directly.
Issues
Report bugs or suggest features via the Issues tab. Include:

Issue description.
Steps to reproduce.
Browser/device details.
Screenshots or logs.

Roadmap
Web Demo

Replace placeholder images (bfaf.jpg, clinic.png, etc.) with real clinic photos.
Add a mock contact form in contact.html.
Integrate Google Maps API for location placeholders in clinicdetails.html.
Enhance transitions/animations for smoother UX.

.NET MAUI App (Reference)

Implement appointment booking with backend sync (e.g., REST API).
Add push notifications for appointment reminders.
Support offline data caching with SQLite.
Improve accessibility (e.g., VoiceOver, TalkBack support).

License
This project is licensed under the MIT License. See LICENSE for details.
Developer
Developed by Mina Malak.  

© 2025 Mina Malak. All Rights Reserved.
