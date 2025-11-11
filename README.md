# Modern Portfolio Website Template

**Live Demo:** [https://portfolio-template-omega-peach.vercel.app/](https://portfolio-template-omega-peach.vercel.app/)

A sleek, modern, and fully responsive personal portfolio website template built with HTML, CSS, and vanilla JavaScript. It includes beautiful animations, a project filter, a skills section, and a dark/light mode toggle.
<img width="1440" height="812" alt="Screenshot 2025-11-11 at 6 11 43 PM" src="https://github.com/user-attachments/assets/1963b160-5f7d-4349-8c8c-ef9ef23907d9" />


## Features

* **Responsive Design:** Looks great on all devices, from mobile phones to desktops.
* **Dark/Light Mode:** A theme toggle that saves the user's preference in `localStorage`.
* **Custom Cursor:** An interactive custom cursor (dot and outline) for an enhanced user experience on desktop.
* **Smooth Scrolling:** Seamless navigation between sections.
* **Sticky Navbar:** A navigation bar that sticks to the top and highlights the active section on scroll.
* **Animations:**
    * **AOS (Animate On Scroll):** Subtle fade and slide animations as you scroll.
    * **Typing Effect:** A dynamic typing effect in the hero section.
    * **Animated Stats:** Numbers in the "About" section count up when they become visible.
    * **Skill Bars:** Animated progress bars for the "Skills" section.
    * **Animated Background:** Floating gradient orbs in the hero section.
* **Project Filtering:** A filterable gallery to categorize and display your projects (e.g., "All", "Web", "Design", "Mobile").
* **Contact Form:** A functional contact form (currently logs to the console, ready to be connected to a backend).
* **Mobile Menu:** A clean, full-screen mobile menu.

## Technologies Used

* **HTML5:** Semantic HTML for structure.
* **CSS3:**
    * CSS Variables (for easy theme customization)
    * Flexbox & Grid
    * Media Queries (for responsiveness)
    * Keyframe Animations
* **Vanilla JavaScript (ES6+):**
    * DOM Manipulation
    * Event Listeners
    * `localStorage` for theme persistence
    * `IntersectionObserver` for scroll-based animations (stats and skills)
* **Libraries:**
    * **Font Awesome:** For icons.
    * **Google Fonts:** Using 'Inter' and 'Space Grotesk' fonts.

## How to Use

1.  **Download or Clone:**
    ```bash
    git clone [https://github.com/niranjan2411/portfolio-template.git](https://github.com/niranjan2411/portfolio-template.git)
    ```
2.  **Navigate to the directory:**
    ```bash
    cd portfolio-template
    ```
3.  **Open the website:**
    * Simply open the `index.html` file in your favorite web browser.

## Customization

This template is designed to be easily customized.

### 1. Change Text and Content:

* Open `index.html`.
* **Hero Section:** Change the name in `.typing-text` and the subtitle in `.hero-subtitle`.
* **Social Links:** Update the `href` attribute in the `<a>` tags within `.social-links` and `.contact-social`.
* **About Me:** Edit the text in `.about-description` and update the `data-target` attributes in `.stat-number` to your stats.
* **Skills:** Update skill names, percentages, and the `--progress` custom property in `.skill-progress` for each skill.
* **Projects:**
    * Update the `data-category` attribute for each `.project-card` to match your filter buttons.
    * Change the project images (`<img>` src).
    * Update project links, tags, titles, and descriptions.
* **Contact Info:** Change the email, phone, and location in the `.contact-detail` elements.
* **Footer:** Update the copyright text.

### 2. Change Styling (Colors & Fonts):

* Open `styles.css`.
* **Colors:** All colors are defined as CSS variables inside the `:root` selector at the top of the file. You can change these to match your personal brand. The dark mode colors are defined in `[data-theme="dark"]`.

    ```css
    :root {
        --primary-color: #6366f1;
        --secondary-color: #8b5cf6;
        --text-primary: #1f2937;
        --bg-primary: #ffffff;
        /* ...and so on */
    }
    ```

* **Fonts:** Fonts are imported in `index.html` from Google Fonts. You can change the `<link>` tags and update the `font-family` property in the `body` selector in `styles.css`.
