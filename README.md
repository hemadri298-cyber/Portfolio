# Hemadri — Cosmic Gaming Portfolio

A personal developer portfolio built for **Class 11 — Builders Day** using **pure HTML and CSS**.

## 🪐 Theme & Design Concept
- **Cosmic Saturn Gaming Aesthetic**: Built with a 3D tilted Saturn gas-giant sphere and concentric orbital rings (with Cassini division), rendered completely in pure CSS gradients and 3D transforms.
- **Orbital Data Spine**: Section cards and waypoints are docked along an orbital track, creating a smooth visual illusion of data gliding through Saturn's rings as you scroll.
- **Glassmorphism HUD**: Translucent dark panels with cyan and violet neon borders (`backdrop-filter: blur(16px)`).
- **Zero JavaScript**: 100% compliant with the course requirement. All smooth scrolling, hover physics, 3D tilts, keyframe animations, and back-to-top actions are accomplished strictly in HTML and CSS.

---

## 🛠️ Technologies Used
- **HTML5**: Semantic tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<form>`)
- **CSS3**:
  - CSS Custom Properties (`:root` variables)
  - CSS Grid (2D layouts for skills categories, project galleries, and hero grid)
  - CSS Flexbox (1D layouts for navigation bar, buttons, pills, tags, and timeline)
  - 3D Transforms (`perspective`, `rotateX`, `rotateY`, `rotateZ`)
  - CSS Keyframe Animations (`@keyframes saturnFloat`, `@keyframes ringPulse`, etc.)
  - Media Queries for mobile and tablet responsiveness

---

## 📂 Project Structure
```text
portfolio/
│
├── index.html                  # Main portfolio document
├── style.css                   # Complete stylesheet with 3D Saturn & animations
├── Portfolio Profile Image.jpeg # Profile picture
├── images/
│   ├── project1.png            # Flexbox Arena preview graphic
│   ├── project2.png            # Responsive Cyber Portal preview graphic
│   └── project3.png            # Saturn Orbital Experience preview graphic
└── README.md                   # Documentation for TA Evaluation
```

---

## 🚀 Key Sections
1. **Sticky Navbar**: Brand logo, status indicator, section jump links (`#home`, `#about`, `#skills`, `#projects`, `#education`, `#contact`), and transmit CTA.
2. **Hero Section**: Profile avatar with orbital dot animation, title, subtitle, quote, and quick stat counters.
3. **About Me**: Narrative on frontend engineering passion, technical focus, and feature cards.
4. **Skills**: Categorized grids (Frontend Core, Motion & Visuals, Tools & Workflow, Currently Exploring).
5. **Projects**: 3 featured projects with preview mockups, tech badges, live demo, and GitHub links.
6. **Education & Milestones**: Chronological timeline featuring Scaler School of Technology and frontend engineering foundations.
7. **Contact**: Communication channels (Email, GitHub, LinkedIn) plus a frontend-only contact form.
8. **Footer & Back to Top**: Smooth scroll-to-top button with hovering pulse animation.

---

## 🧑‍🏫 TA Evaluation Cheat-Sheet
- **Why Grid?** Used for two-dimensional layouts like the projects showcase, skills categories, and about cards where both rows and columns need alignment.
- **Why Flexbox?** Used for one-dimensional components like the sticky navbar, button groups, tag pills, and form fields where items align in a row or stack.
- **How does the 3D Saturn ring work?** 
  - The planet sphere has `border-radius: 50%` with realistic linear and radial gradients.
  - The ring is tilted using `transform: rotateX(75deg) rotateY(-14deg) rotateZ(-22deg)`.
  - Realistic depth is created using two clipped layers: `.ring-back` (clipped to the top half with `clip-path`, `z-index: 1`) passes behind the planet, while `.ring-front` (clipped to the bottom half, `z-index: 3`) passes in front of the planet.
- **How does the back-to-top work without JavaScript?** The `html` element has `scroll-behavior: smooth`, and the floating anchor `<a href="#top">` smoothly returns the viewport to `<body id="top">`.

---

## 👤 Author
**Hemadri**  
CS & AI Student | Frontend Developer | Builder
