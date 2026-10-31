

Module Code: WEDES020  
Qualification: Diploma in Information Technology in Software Development  
Institution: Rosebank College Nelson Mandela Bay Campus  
Location: Gqeberha, South Africa  

---

# CRUMB STUDIO BAKERY - My Website
PART 1 WEBDEVELOPMENT ASSIGNMENT
## This is my final GitHub submission for Part 1
- I updated my proposal
- I added my 5 html pages
-  I have a navigation panel
-  Customers can view the gallery and find the location.
-  Customers can ask questions by using the enquiry form I created as well.
### Goal Achieved
- My website does not have any errors, and it is neatly organized for customers to view.
- ### I did insert an extra file, 
- This website was created for the goal, so that customers can easily view my pages and understand what this website is also about. The website has a option for users to ask extra questions using a message box that was created in the enquiry page.
  ### The five pages
  - Indexhtml
  - Contacthtml
  - AboutUshtml
  - Galleryhtml
  - Enquiryhtml


# Part 2 POE

For part 2, I focused on improving my website by adding css.styles inside my Assets folder, proving my website proposal and editing the readme.Md
---
## Changes
* Updated the proposal
* Added a Readme file on vscode
* Added css.styles
* Added a footer
* Added a hamburger
* Added more photos
## Features

* *Responsive Layout:* Designed with modern CSS for seamless display across mobile, tablet, and desktop screens.
* *Component-Based Styling:* Clean, reusable CSS structure for easy maintenance and scaling.
* *Custom Theming:* Utilizes CSS custom properties (variables) for fast and easy theme switching.

---

## Tech Stack

* *Structure:* HTML5
* *Styling:* Modern CSS (Flexbox, Grid, CSS Variables)

---

## File Structure

```text
├── index.html
├── assets/
│   └── images/
└── css/
    ├── style.css
    └── variables.css
```
* Color scheme: Primary Color (--primary-color): #5c3a21 

Warm Chocolate Brown — used for the main header bar, logo text title, primary buttons, and footer background. 

Secondary Color (--secondary-color): #f4e8d1 

Cream / Soft Warm Sand — used for the subtle container highlight. 

Accent Color (--accent-color): #d4a373 

Warm Golden Cookie / Warm Tan — used for hover highlights, active link colors, section dividers, and footer headings. 

Background Color (--bg-color): #fefae0 

Light Buttercream / Soft Off-White — applied to body.home-page 

Text Color (--text-color): #333333 

Dark Charcoal Gray — used for main body text. 

White (--white): #ffffff 

Pure White — used for container card backgrounds, form fields, and navigation link text. 

* Typography: Primary Font Family: Arial, sans-serif 

Clean and highly readable for operating systems and web browsers. 

Line Height: 1.6 

Applied globally to body.home-page for clear line spacing and easy readability.

## Update for an Ice task 4
- Added a form on my contact page
- Formatted my contact page again using style.css
## 1.SUMMARY

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



## 3. CORE FEATURES AND TECHNICAL IMPLEMENTATION

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

## 4. USER INTERFACE (UI) AND USER EXPERIENCE (UX) DESIGN

### Typography and Palette
- Primary Color: Deep Cocoa Brown (#4a2c11) for headers, borders, and main brand elements.
- Accent Color: Warm Bakery Gold (#c88d46) for interactive buttons, highlights, and subtle tags.
- Background Tones: Soft Warm Cream (#fdfaf6 / #f4ece1) to provide a cozy aesthetic.
- Typography: Clean sans-serif and system font stacks prioritizing legible rendering across screen resolutions.

### Header and Navigation Structure
- Text Branding: Employs a text-based brand title (CRUMB STUDIO) in place of generic logo graphics for clean alignment.
- Mobile Drawer Menu: Utilizes a CSS checkbox toggle (#menu-toggle) and CSS hamburger icon label for pure CSS responsive navigation on narrow mobile screens.

---

## 5. SEARCH ENGINE OPTIMIZATION (SEO) AND ACCESSIBILITY COMPLIANCE

- Meta Descriptions: Every HTML document features a custom <meta name="description" content="..."> tag summarizing page purpose.
- Alt Text Coverage: All <img> elements include meaningful alternative text attributes to support screen readers and enhance search indexation.
- Semantic HTML Structuring: Documents stick strictly to structural HTML5 tags (<header>, <main>, <section>, <article>, <nav>, <footer>) to facilitate automated DOM parsing.

---

## 6. QUALITY ASSURANCE AND TESTING FRAMEWORK

- Browser Verification: Tested on Google Chrome, Microsoft Edge, Mozilla Firefox, and Apple Safari.
- Viewport Testing: Validated across desktop monitors (1920x1080), laptop screens (1366x768), tablet interfaces (768x1024), and mobile viewports (375x667 and 414x896).
- DOM Script Validation: Script execution verified to prevent console syntax errors, unhandled promise rejections, or broken onclick event bindings.

---

## 7. INSTALLATION, DEPLOYMENT, AND LOCAL SETUP

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

## 8. COMPREHENSIVE CHANGELOG AND PROJECT HISTORY

- Version 1.0.0 (Initial Framework): Created multi-page file structure, linking base stylesheets and primary page skeletons.
- Version 1.1.0 (Header & Navigation Overhaul): Replaced static image logo with brand title text and added CSS checkbox hamburger drawer for mobile viewports.
- Version 1.2.0 (Gallery & Lightbox Integration): Implemented CSS Grid gallery layout and added full-screen modal lightbox functionality.
- Version 1.3.0 (Team Section Refinement): Upgraded team profiles to 3D flip-cards with dark brown back styling and white text for contrast.
- Version 1.4.0 (Form Processing Improvements): Separated feedback (contact.html) and catering (enquiry.html) forms with custom exit modals and Google Map integration.
- Version 2.0.0 (Smart Search & Multi-Step Ordering): Added universal hero search bar with live dropdown suggestions, updated gallery to 20 exact cookie items, and built the multi-step Add-to-Cart workflow modals with store pickup instructions.

---

## 9. PROJECT SUMMARY AND ACADEMIC ASSESSMENT METRICS

Evaluation Metric - Implementation Detail - Status

- Multi-Page Layout : 6 complete HTML5 pages (index, about, contact, enquiry, Gallery, team)
- Responsive Design : Custom CSS Grid and Flexbox models supporting desktop, tablet, and mobile 
- Product Portfolio : 20 individual cookie items with exact custom titles, prices, and high-res imagery 
- Interactive Modals : Full-screen image lightbox modal, quantity calculation modal, and store-pickup receipt confirmation modal 
- Smart Search : Cross-page search bar with auto-suggestion dropdowns and automatic parameter routing 
- Forms & Maps : Validated contact and enquiry forms paired with embedded location map 
- SEO & Accessibility : Unique meta descriptions, semantic HTML5 structure, and full image alt text coverage
- Documentation : Extensive, fully detailed README.md repository document 
# GRAPHICAL USER INTERFACE (GUI) DOCUMENTATION

## 10. NAVIGATION & HEADER LAYOUT
- Brand Title: Positioned prominently at the top left/center of every page as clean text ("CRUMB STUDIO") in deep cocoa brown, avoiding graphic clutter.
- Desktop Navigation Bar: Horizontal link list connecting all main views (HOME PAGE, OUR STORY, CONTACT, ENQUIRY, GALLERY, OUR TEAM) separated by clean vertical dividers.
- Mobile Drawer Menu: On screens smaller than 820px, the navigation bar converts into a 3-line hamburger icon. Tapping the icon smoothly slides open a vertical drawer menu.

---

## 11. HERO SECTION & SMART SEARCH BAR
- Greeting & Banner: Features a welcoming intro ("Hello there...") alongside a high-resolution hero display image showcasing stacked artisanal cookies.
- Centered Search Bar: Placed directly beneath the introductory copy with a prominent gold search button ("Search Gallery").
- Live Auto-Suggestions Dropdown: Typing into the input opens a floating dropdown listing matching site pages (Contact Us, Our Team, Enquiry) and cookie names (Macaron, Biscoff, Pig cookies). Clicking any item routes the user directly to that page or filters the gallery instantly.

---

## 12. PRODUCT GALLERY GRID (2-COLUMN LAYOUT)
- Balanced Grid Layout: Arranges all 20 cookie items across a spacious 2-column grid.
- Image Cards & Zoom Badges: Each card features a high-quality product photo with a semi-transparent "Click to zoom" badge overlay that highlights on hover.
- Price & Title Display: Displays the exact cookie name and price in South African Rands (e.g., "R 35.00").
- Call-to-Action Buttons: Includes a styled "Add to Cart" button on every card to launch the ordering workflow.

---

## 13. OVERLAY MODALS (INTERACTIVE POPUPS)
- Quantity Selection Modal (Step 1): Tapping "Add to Cart" brings up a centered popup window displaying the item title, a numeric quantity selector input, and a live auto-calculating total price.
- Receipt & Confirmation Modal (Step 2): Clicking "Next" transitions to a confirmation popup displaying the required store pickup message:
  "Your order has been submitted. Go to the nearest store and please show them your message and pay in front of the counter. Thank you for supporting our business."
- Email Handoff: Clicking "Proceed to Open Gmail" opens the user's email client with pre-formatted order details and receipt instructions.
- Image Lightbox Modal: Clicking any cookie image darkens the background and displays the photo in high resolution, equipped with previous (<) and next (>) navigation arrows and descriptive captions.

---

## 14. INTERACTIVE 3D TEAM FLIP CARDS
- Two-Sided Profile Cards: Presents bakery staff and leadership on the "Our Team" page.
- 3D Flip Animation: Hovering or tapping a card triggers a smooth 180-degree card flip animation.
- h-Contrast Backing: The back of each card uses a dark bakery-brown background with crisp white typography to ensure descriptions are easily readable.

---

## 15. FORMS & INTERACTIVE LOCATION MAP
- Form Styling: Styled input boxes and textareas with gold focus borders on both the general Feedback page (contact.html) and Catering Enquiry page (enquiry.html).
- Embedded Google Map: A responsive, framed location map integrated directly onto the contact page showing the bakery's location in Gqeberha.

---

## 16. FOOTER SECTION & QUICK LINKS
- 3-Block Footer Layout: Features organized columns for Contact Info (Phone/Email), Social Media links (Facebook/Instagram), and a full Quick Links list for instant 1-click navigation to any page.
-
# REFERENCES 
---

## References

1. World Wide Web Consortium (W3C). (2023). HTML5 Specification and Semantic Markup Guidelines. W3C Recommendation. Available at: https://www.w3.org/TR/html52/

2. World Wide Web Consortium (W3C). (2023). Cascading Style Sheets (CSS) Level 3 Specification: Grid Layout, Flexbox, and 3D Transforms. W3C Recommendation. Available at: https://www.w3.org/TR/css-grid-1/

3. Mozilla Developer Network (MDN). (2024). JavaScript (ES6+) Standard Reference: Event Handling, DOM Manipulation, and URLSearchParams API. MDN Web Docs. Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript

4. Web Content Accessibility Guidelines (WCAG). (2023). WCAG 2.1 Standard: Text Contrast, Keyboard Navigation, and Alternative Text (Alt Text) Requirements. Web Accessibility Initiative (WAI). Available at: https://www.w3.org/WAI/standards-guidelines/wcag/

5. Google Maps Platform. (2024). Embed API & Maps Integration Standards. Google Developers Documentation. Available at: https://developers.google.com/maps/documentation/embed

6. Visual Studio Code & Live Server Documentation. (2024). Local Development & Static Web Server Setup Guide. Available at: https://code.visualstudio.com/docs
7.
