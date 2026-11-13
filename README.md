# The Silk Launge 💇‍♀️✨

> **A luxury, modern, and responsive unisex salon & spa web application.**

Welcome to the official repository for **The Silk Launge**. Designed with sophistication and modern web standards, this website delivers a seamless digital experience for salon clients to discover premium hair styling, body treatments, beauty therapies, view transparent pricing, explore photo galleries, and book appointments online.

---

## 🌟 Key Features

- **💎 Elegant Luxury Aesthetics:** Tailored dark & golden theme with sleek typography (`Oswald` & `Rubik`) and smooth transitions.
- **📱 Fully Responsive Design:** Mobile-first architecture that scales smoothly across mobile devices, tablets, laptops, and ultra-wide screens.
- **🧭 Dynamic Interactive Navigation:**
  - Sticky header that transitions smoothly on scroll.
  - Smooth in-page anchor scrolling to any section.
  - Mobile hamburger navigation drawer with backdrop transitions.
  - Floating "Back to Top" button that appears on scroll.
- **✨ Service Showcase:** Six core salon offerings featuring custom Flaticon iconography:
  - Hair Cutting Style
  - Hair Washing & Conditioning
  - Body & Stone Treatments
  - Beauty & Spa
  - Stylist Shaving & Grooming
  - Multi Hair Coloring
- **🏷️ Interactive Pricing Filter:** Real-time JavaScript-driven category filter for service pricing:
  - *All Pricing*
  - *Beauty & Spa*
  - *Body Treatments*
  - *Face Washing*
  - *Meditations*
  - *Shaving*
- **📸 Visual Photo Gallery:** Responsive image grid highlighting professional salon results and styling portfolio.
- **📅 Appointment Booking Form:** Ready-to-connect reservation form collecting:
  - Client Full Name & Email
  - Phone Number
  - Service Category Selector
  - Preferred Date
  - Special Notes & Requests
- **📬 Newsletter Subscription:** Integrated footer subscription input for promotions and news.
- **📞 Comprehensive Contact Integration:**
  - Top header hotline & opening hours.
  - Dual contact lines: **Primary** and **Alternative** contact numbers.
  - Dual email channels: General inquiries & Booking desk.
  - Operating hours and physical location address.
  - Direct social media links and WhatsApp chat integration.

---

## 📞 Contact Information & Configuration

The contact details configured in the project:

| Detail | Primary | Alternative |
|---|---|---|
| **Brand Name** | The Silk Launge | — |
| **Phone** | `+94 11 234 5678` | `+94 77 123 4567` |
| **Email** | `info@thesilklaunge.com` | `booking@thesilklaunge.com` |
| **Address** | No. 45, Silk Boulevard, Colombo 07, Sri Lanka | — |
| **Opening Hours** | Sunday – Friday: 08:00 AM – 10:00 PM | Saturday: By Appointment |
| **Social Links** | Facebook, Twitter/X, YouTube | WhatsApp Chat (`+94 77 123 4567`) |

---

## 📁 Project Structure

```text
The-Silk-Launge/
│
├── index.html                   # Main single-page website template
├── README.md                    # Project documentation & setup guide
├── favi1.png                    # Favicon icon
│
└── assets/
    ├── css/
    │   ├── style.css            # Custom CSS stylesheets, variables & responsive queries
    │   └── flaticon.min.css     # Flaticon salon icon font styles
    │
    ├── js/
    │   └── script.js            # Interactive behaviors (nav toggle, filters, smooth scroll)
    │
    └── images/                  # Media assets & photo galleries
        ├── hero-banner.jpg      # Hero section background banner
        ├── pricing-bg.jpg       # Pricing section background
        ├── pricing-1.jpg...8    # Pricing menu item thumbnails
        ├── gallery-1.jpg...4    # Portfolio gallery images
        ├── appoin-banner-1.jpg  # Appointment card left banner
        ├── appoin-banner-2.jpg  # Appointment card right banner
        ├── footer-bg.png        # Footer decorative background
        └── footer-blog-1.jpg...2# Footer blog preview thumbnails
```

---

## 🛠️ Built With

- **HTML5:** Semantic, accessible markup for optimal SEO and screen-reader support.
- **CSS3:** Custom properties (CSS variables), CSS Grid, Flexbox, keyframe animations, and custom media queries.
- **JavaScript (ES6+):** Vanilla JavaScript for zero-dependency performance:
  - Navbar open/close toggling.
  - Header scroll detection.
  - Real-time pricing tab filtering with data attributes (`data-filter-btn`, `data-filter`).
  - Smooth scrolling for internal anchor links.
- **Ionicons:** Modern SVG icon pack ([ionicons.com](https://ionic.io/ionicons)).
- **Flaticon:** Salon, spa, and beauty glyph icon set.
- **Google Fonts:**
  - `Oswald` (Weights: 400, 500, 600, 700)
  - `Rubik` (Weights: 300, 400, 700)

---

## 🚀 Quick Start & Local Preview

No heavy dependencies or build tools are required. You can launch and preview the website instantly using any of the following methods:

### Method 1: Direct File Launch
Simply double-click [`index.html`](index.html) or open it directly in Google Chrome, Mozilla Firefox, Microsoft Edge, or Apple Safari.

### Method 2: VS Code Live Server
1. Open the project folder in **Visual Studio Code**.
2. Install the **Live Server** extension (by *Ritwick Dey*).
3. Right-click [`index.html`](index.html) and select **"Open with Live Server"**.

### Method 3: Python Local Server
If Python is installed on your machine:
```bash
# Python 3
python -m http.server 8000
```
Then visit `http://localhost:8000` in your web browser.

### Method 4: Node.js (npx serve)
```bash
npx serve .
```

---

## 🎨 Customization Guide

### 1. Changing Brand Name or Logo
Open [`index.html`](index.html):
- Update the `<title>` and `<meta name="title">` in the `<head>` section.
- Search for the `.logo` class in both the **header** (around line 106) and **footer** (around line 790):
  ```html
  <a href="#" class="logo">
    The Silk
    <span class="span">Launge</span>
  </a>
  ```

### 2. Updating Contact Numbers & Emails
- **Header Contact Bar:** Around line 50 in [`index.html`](index.html).
- **Footer Contact List:** Around line 920 in [`index.html`](index.html).
- Modify the `href="tel:..."` and `href="mailto:..."` attributes to match your actual phone and email links.

### 3. Adjusting Theme Colors & Fonts
Open [`assets/css/style.css`](assets/css/style.css) and edit the root variables:
```css
:root {
  --indian-yellow: hsl(36, 61%, 58%);   /* Primary Accent / Gold */
  --harvest-gold: hsl(36, 66%, 53%);    /* Hover & Button Accent */
  --rich-black-fogra-39: hsl(0, 0%, 5%);/* Background Dark */
  --eerie-black-1: hsl(0, 0%, 14%);     /* Card Background */
  --white: hsl(0, 0%, 100%);            /* Primary Text */
}
```

### 4. Updating Pricing & Service Items
In [`index.html`](index.html), find `<section class="section pricing" id="pricing">`:
- Add or modify `<li data-filter="<category-name>">` elements.
- Ensure the `data-filter` value matches one of the filter buttons in `<ul class="tab-filter">`.

---

## 🌐 Browser Compatibility

Tested and optimized for all modern browsers:
- Google Chrome (Latest)
- Mozilla Firefox (Latest)
- Microsoft Edge (Latest)
- Apple Safari (Latest)
- Opera (Latest)

---

## 📄 License & Attribution

- **Project:** The Silk Launge
- **Design & Layout:** Licensed for use by The Silk Launge.
- **Icons:** Ionicons (MIT License) and Flaticon.
- All rights reserved &copy; 2025 **The Silk Launge**.

