# Sticky Glass Header Effect (Elementor)

A modern **glassmorphism sticky header effect** built with CSS for websites created with **Elementor**.

When the user scrolls, the header becomes sticky and applies a **blurred glass background**, soft shadows, and smooth transitions for a premium UI experience.

## ✨ Features

* Smooth header transition on scroll
* Glassmorphism effect using `backdrop-filter`
* Elegant gradient glossy overlay
* Sticky header optimization
* Compatible with Elementor sticky effects

## 💻 CSS Code

```css
/* HEADER TRANSITION */

selector{
transition: all 0.6s ease !important;
position: relative;
}

/* STICKY GLASS HEADER */

selector.elementor-sticky--effects{

background: rgba(25,45,75,0.82) !important;

backdrop-filter: blur(12px) saturate(160%);
-webkit-backdrop-filter: blur(12px) saturate(160%);

border-bottom: 1px solid rgba(255,255,255,0.15);

box-shadow: 0 12px 35px rgba(0,0,0,0.25);

}

/* GLOSSY OVERLAY */

selector.elementor-sticky--effects::before{

content:"";

background: linear-gradient(
120deg,
rgba(255,255,255,0.18),
rgba(255,255,255,0.05) 35%,
rgba(255,255,255,0) 70%
);

pointer-events:none;

}

/* HEIGHT */

selector > .elementor-container{
transition:min-height 0.8s ease !important;
}

#top-header {
display: none!important;
}

#main-header {
display: none!important;
}

.elementor-19462 .elementor-element.elementor-element-6163ab0a {
margin-top: 16px;
margin-bottom: 0px;
padding: 20px 0px 20px 0px;
z-index: 99;
}
```

## 🚀 How to Use

1. Open your **Elementor Header template**.
2. Go to **Advanced → Custom CSS**.
3. Paste the code above.
4. Enable **Sticky Header** in Elementor.
5. Save and publish.

## 🎨 Result

When scrolling:

* The header becomes sticky
* A **glass blur effect** appears
* Smooth transitions improve the visual experience
* The layout maintains a clean and modern UI

## 🧩 Perfect for

* Modern landing pages
* SaaS websites
* Agency websites
* Portfolio websites
* WordPress + Elementor projects
