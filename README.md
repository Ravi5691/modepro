Here’s a well-structured `README.md` for your project using **GSAP**, **ScrollTrigger**, **Locomotive Scroll**, and **Canvas-based image sequence animation**:

---

# 🚀 Scroll Animation Project with GSAP, Locomotive Scroll & Canvas

This project demonstrates a **high-performance scroll animation** using `GSAP`, `ScrollTrigger`, and `Locomotive Scroll`. It features a **canvas-based frame-by-frame animation** synced with scrolling, combined with **pinned full-page sections** for immersive storytelling or creative showcases.

---

## 🔧 Features

* Smooth scrolling using **Locomotive Scroll**
* Scroll-synced canvas animation with **GSAP ScrollTrigger**
* Frame-by-frame image sequencing for high-fidelity visuals
* Responsive canvas rendering
* Scroll-triggered pinning for multiple sections (`#page1`, `#page2`, `#page3`)

---

## 📁 Folder Structure

```
project-root/
│
├── index.html
├── script.js           // (Your JavaScript code)
├── frames/             // (Contains all animation frames: male0001.png → male0300.png)
│   ├── male0001.png
│   └── ...
└── styles.css          // (Optional CSS styles)
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/scroll-animation-project.git
cd scroll-animation-project
```

### 2. Install dependencies

Include the following in your `index.html` or install via NPM:

```html
<!-- GSAP and ScrollTrigger -->
<script src="https://unpkg.com/gsap@3/dist/gsap.min.js"></script>
<script src="https://unpkg.com/gsap@3/dist/ScrollTrigger.min.js"></script>

<!-- Locomotive Scroll -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/locomotive-scroll/dist/locomotive-scroll.min.css">
<script src="https://cdn.jsdelivr.net/npm/locomotive-scroll/dist/locomotive-scroll.min.js"></script>
```

### 3. Setup Image Frames

Place all frame images inside the `./frames` directory and ensure they follow this naming convention:

```
male0001.png
male0002.png
...
male0300.png
```

> You can modify the `files(index)` function in `script.js` to change the folder or naming pattern.

---

## ✨ How It Works

* `LocomotiveScroll` smooths the page scroll and links with `GSAP ScrollTrigger`.
* A canvas element displays a sequence of 300 images as you scroll.
* `GSAP.to()` animates the `imageSeq.frame` and updates the canvas accordingly.
* Individual sections like `#page1`, `#page2`, `#page3` are pinned during scroll for storytelling.

---

## 📱 Responsive Design

The canvas resizes on window resize:

```js
window.addEventListener("resize", () => {
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
  render();
});
```

---

## 🧩 Dependencies

* [GSAP](https://greensock.com/gsap/)
* [ScrollTrigger](https://greensock.com/scrolltrigger/)
* [Locomotive Scroll](https://locomotivemtl.github.io/locomotive-scroll/)

---

## 🛠 Customization Tips

* To change frame count, update `const frameCount = 300;`
* To adjust scroll length, modify the `end` value in ScrollTrigger (`600% top`)
* You can add more pinned sections with `gsap.to()` and `ScrollTrigger`

---

## 📷 Preview

> Add a screenshot or screen recording here for visual reference.

---

## 📝 License

This project is open-source and available under the MIT License.

---

Let me know if you want this readme in Hindi or styled in Markdown with emojis, badges, or GitHub project links.
