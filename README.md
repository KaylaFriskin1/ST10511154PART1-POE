# CRUMB STUDIO BAKERY - My Website

Module Code: WEDES020  
Qualification: Diploma in Information Technology in Software Development  
Institution: Rosebank College Nelson Mandela Bay Campus  
Location: Gqeberha, South Africa  

---

## TABLE OF CONTENTS
1. Executive Summary
2. Comprehensive Project Requirements and Vision
3. System Architecture and Directory Layout
4. Core Features and Technical Implementation
5. User Interface (UI) and User Experience (UX) Design
6. Search Engine Optimization (SEO) and Accessibility Compliance
7. Quality Assurance and Testing Framework
8. Installation, Deployment, and Local Setup
9. Comprehensive Changelog and Project History
10. Project Summary and Academic Assessment Metrics

---

## 1. EXECUTIVE SUMMARY

Crumb Studio Bakery is an interactive, fully responsive multi-page web platform engineered for a boutique bakery located in Gqeberha, South Africa. Designed to satisfy all technical and structural guidelines of the WEDES020 Web Development module, this project delivers an engaging, accessible, and feature-rich digital storefront.

The application allows users to seamlessly navigate between specialized sections, perform instant cross-site and product-level searches with interactive dropdown suggestions, examine high-resolution product imagery through an interactive lightbox modal, execute multi-step cookie order requests with automated receipt confirmation modals, submit targeted catering and general enquiries, and view accurate location maps and interactive team profiles.

---

## 2. COMPREHENSIVE PROJECT REQUIREMENTS AND VISION

### Primary Business Goals
- Establish a unique online presence for Crumb Studio Bakery to attract local cookie enthusiasts, event coordinators, and party planners in Gqeberha.
- Provide a clear, transparent menu showcasing twenty distinct cookie varieties with unit prices, calculated order totals, and streamlined store-pickup instructions.
- Separate customer communication pathways into distinct contact and catering enquiry workflows to optimize customer service delivery.

### Key Academic and Technical Directives
- Multi-Page Architecture: Implement cleanly separated semantic HTML5 pages including Home, Our Story, Contact, Enquiry, Gallery, and Our Team.
- Responsive Layout Design: Utilize CSS Grid and Flexbox layouts to ensure optimal presentation across desktop monitors, laptops, tablets, and mobile smartphones without horizontal scrolling or UI breaking.
- Client-Side Interactivity: Employ vanilla JavaScript (ES6+) for live search filtering, URL parameter parsing, custom modal controllers, total calculations, and three-dimensional card rotations.
- Accessibility and SEO Standards: Incorporate structured meta tags, semantic content hierarchy, and descriptive alternative text for all media elements.

---

## 3. SYSTEM ARCHITECTURE AND DIRECTORY LAYOUT

The file structure follows a standardized, modular organization separating root index entry points, core CSS assets, visual media files, and sub-page views.

crumb-studio-bakery/
│
├── index.html                  # Main Home Page featuring Hero Search and Brand Overview
├── README.md                   # Comprehensive Project Technical Documentation
│
├── Assets/
│   ├── style.css               # Core Stylesheet (Variables, Grid, Modals, 3D Transforms)
│   └── images/                 # Optimized Visual Assets
│       ├── logo1.jpg           # Site Favicon Media
│       ├── picture1.jpg        # Hero Banner Display Graphic
│       ├── 2.jpg               # Macaron Cookie
│       ├── 3.jpg               # Pig Cookies
│       ├── 4.jpg               # M&M Cookies
│       ├── 5.jpg               # Hershey Cookies
│       ├── 6.jpg               # Lemon Surprise Cookie
│       ├── 7.jpg               # Biscoff Cookie
│       ├── 8.jpg               # Heart Cookies
│       ├── 9.jpg               # Pistachio Chip Cookie
│       ├── 10.jpg              # Cream Full Cookie
│       ├── 11.jpg              # Mint Choc Cookie
│       ├── 12.jpg              # Cute Flower Cookie
│       ├── 13.jpg              # Fun Cookies
│       ├── 14.jpg              # Fat Cookies
│       ├── 15.jpg              # Ice Cream Cookie
│       ├── 16.jpg              # Choc Chip Ice-Cream Cookie
│       ├── 17.jpg              # Oreo Surprise Cookie
│       ├── 18.jpg              # Oats Cookie
│       ├── 19.jpg              # Jam Full Cookie
│       ├── 20.jpg              # Pistachio White Cookie
│       └── 21.jpg              # Red Cookies
│
└── Pages/
    ├── about.html              # Brand Story, History, and Artisan Values Page
    ├── contact.html            # General Feedback Form and Embedded Google Map
    ├── enquiry.html            # Event Catering and Custom Bulk Order Form
    ├── Gallery.html            # 20-Item Product Gallery with Live Search and Lightbox
    └── team.html               # Interactive 3D Flip-Card Team Presentation

---

## 4. CORE FEATURES AND TECHNICAL IMPLEMENTATION

### Universal Smart Search Engine
- Hero-Integrated Search Box: Positioned centrally on the main home page (index.html), allowing users to input full or partial terms.
- Live Suggestions Dropdown: As the user types, a client-side JavaScript routine filters a pre-configured dictionary of pages (such as Contact Us, Our Team, Order Enquiry) and specific cookies (such as Macaron, Biscoff, Pig cookies, Oats). A structured dropdown updates instantly beneath the search input.
- Automatic Navigation and Parameter Passing: Selecting a dropdown suggestion or pressing Enter executes a routing action. Searching for pages opens the respective HTML document directly, while searching for cookies redirects to Pages/Gallery.html?search=KEYWORD, automatically triggering gallery filtering on load.

### Interactive 20-Item Product Gallery
- Spacious 2-Column Responsive Grid: Displays cards with uniform dimensions, pricing text, high-contrast typography, and a hover zoom badge (.gallery-zoom-badge).
- Complete 20-Cookie Roster:
  1. Macaron
  2. Pig cookies
  3. M&M cookies
  4. Hershey cookies
  5. Lemon surprise
  6. Biscoff
  7. Heart cookies
  8. Pistachio chip
  9. Cream full
  10. Mint choc
  11. Cute flower
  12. Fun cookies
  13. Fat cookies
  14. Ice cream cookie
  15. Choc chip ice-cream
  16. Oreo Surprise
  17. Oats
  18. Jam full
  19. Pistachio white
  20. Red cookies

### Multi-Step Add-to-Cart Modal Flow
- Step 1 (Quantity Selection): Clicking "Add to Cart" triggers startOrderFlow(), opening #qtyModal. Users specify their desired quantity, and JavaScript dynamically updates the calculated total (unitPrice * quantity).
- Step 2 (Order Submission Confirmation): Clicking "Next" closes the quantity modal and displays #confirmModal containing the required receipt instructions:
  "Your order has been submitted. Go to the nearest store and please show them your message and pay in front of the counter. Thank you for supporting our business."
- Step 3 (Gmail Handoff): Clicking "Proceed to Open Gmail" triggers a constructed mailto: URL containing the formatted item name, chosen quantity, calculated price, and pickup instructions.

### Full-Screen Lightbox Modal
- High-Resolution View: Clicking any gallery thumbnail triggers openLightbox(index), displaying a full-screen overlay containing the image and caption.
- Carousel Controls: Integrated controls allow users to cycle seamlessly forward or backward through all twenty cookie photos using array indexing.

### Interactive 3D Team Flip Cards
- Two-Sided Perspective Cards: Built using CSS 3D transforms (transform-style: preserve-3d; transition: transform 0.6s;).
- High-Contrast Dark Theme: The reverse face uses a dark bakery-brown background (.bg-bakery-darkCard) with white body text to maximize readability.

---

## 5. USER INTERFACE (UI) AND USER EXPERIENCE (UX) DESIGN

### Typography and Palette
- Primary Color: Deep Cocoa Brown (#4a2c11) for headers, borders, and main brand elements.
- Accent Color: Warm Bakery Gold (#c88d46) for interactive buttons, highlights, and subtle tags.
- Background Tones: Soft Warm Cream (#fdfaf6 / #f4ece1) to provide a cozy aesthetic.
- Typography: Clean sans-serif and system font stacks prioritizing legible rendering across screen resolutions.

### Header and Navigation Structure
- Text Branding: Employs a text-based brand title (CRUMB STUDIO) in place of generic logo graphics for clean alignment.
- Mobile Drawer Menu: Utilizes a CSS checkbox toggle (#menu-toggle) and CSS hamburger icon label for pure CSS responsive navigation on narrow mobile screens.

---

## 6. SEARCH ENGINE OPTIMIZATION (SEO) AND ACCESSIBILITY COMPLIANCE

- Meta Descriptions: Every HTML document features a custom <meta name="description" content="..."> tag summarizing page purpose.
- Alt Text Coverage: All <img> elements include meaningful alternative text attributes to support screen readers and enhance search indexation.
- Semantic HTML Structuring: Documents stick strictly to structural HTML5 tags (<header>, <main>, <section>, <article>, <nav>, <footer>) to facilitate automated DOM parsing.

---

## 7. QUALITY ASSURANCE AND TESTING FRAMEWORK

- Browser Verification: Tested on Google Chrome, Microsoft Edge, Mozilla Firefox, and Apple Safari.
- Viewport Testing: Validated across desktop monitors (1920x1080), laptop screens (1366x768), tablet interfaces (768x1024), and mobile viewports (375x667 and 414x896).
- DOM Script Validation: Script execution verified to prevent console syntax errors, unhandled promise rejections, or broken onclick event bindings.

---

## 8. INSTALLATION, DEPLOYMENT, AND LOCAL SETUP

### Prerequisites
- Any modern web browser (Google Chrome, Mozilla Firefox, Microsoft Edge, Safari).
- Visual Studio Code (recommended) with the Live Server extension.

### Step-by-Step Setup
1. Clone the project repository from GitHub:
   git clone https://github.com/your-username/crumb-studio-bakery.git

2. Change directory into the repository folder:
   cd crumb-studio-bakery

3. Open the project in your code editor or double-click index.html to open it in your browser.
4. If using VS Code Live Server, right-click index.html and select Open with Live Server to serve the site locally at http://127.0.0.1:5500/index.html.

---

## 9. COMPREHENSIVE CHANGELOG AND PROJECT HISTORY

- Version 1.0.0 (Initial Framework): Created multi-page file structure, linking base stylesheets and primary page skeletons.
- Version 1.1.0 (Header & Navigation Overhaul): Replaced static image logo with brand title text and added CSS checkbox hamburger drawer for mobile viewports.
- Version 1.2.0 (Gallery & Lightbox Integration): Implemented CSS Grid gallery layout and added full-screen modal lightbox functionality.
- Version 1.3.0 (Team Section Refinement): Upgraded team profiles to 3D flip-cards with dark brown back styling and white text for contrast.
- Version 1.4.0 (Form Processing Improvements): Separated feedback (contact.html) and catering (enquiry.html) forms with custom exit modals and Google Map integration.
- Version 2.0.0 (Smart Search & Multi-Step Ordering): Added universal hero search bar with live dropdown suggestions, updated gallery to 20 exact cookie items, and built the multi-step Add-to-Cart workflow modals with store pickup instructions.

---

## 10. PROJECT SUMMARY AND ACADEMIC ASSESSMENT METRICS

Evaluation Metric | Implementation Detail | Status
---|---|---
Multi-Page Layout | 6 complete HTML5 pages (index, about, contact, enquiry, Gallery, team) | Complete
Responsive Design | Custom CSS Grid and Flexbox models supporting desktop, tablet, and mobile | Complete
Product Portfolio | 20 individual cookie items with exact custom titles, prices, and high-res imagery | Complete
Interactive Modals | Full-screen image lightbox modal, quantity calculation modal, and store-pickup receipt confirmation modal | Complete
Smart Search | Cross-page search bar with auto-suggestion dropdowns and automatic parameter routing | Complete
Forms & Maps | Validated contact and enquiry forms paired with embedded location map | Complete
SEO & Accessibility | Unique meta descriptions, semantic HTML5 structure, and full image alt text coverage | Complete
Documentation | Extensive, fully detailed README.md repository document | Complete
