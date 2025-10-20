---
title: clamp() — Fluid Font Size
class: note
date: 2025-10-07
tags:
  - code
---
# 🧭 CSS `clamp()` — Fluid Font Size 

`clamp()` is a CSS function that makes a value smoothly scale between a **minimum**, a **preferred (fluid)**, and a **maximum** value.

### 📘 Syntax
```css
clamp(min, preferred, max)
```

---

### 💡 Example — Fluid Text
```css
font-size: clamp(24px, 5vw, 80px);
```

| Part | Meaning | Behavior |
|------|----------|-----------|
| `24px` | **Minimum size** | Text won’t go smaller than 24px, even on small screens |
| `5vw` | **Preferred (fluid) value** | Scales with 5% of the viewport width |
| `80px` | **Maximum size** | Text stops growing after 80px on large screens |

---

### 🧠 How It Works
- When screen width = **400px**, `5vw = 20px` → uses **24px** (min limit).  
- When screen width = **800px**, `5vw = 40px` → uses **40px** (fluid).  
- When screen width = **1600px**, `5vw = 80px` → uses **80px** (max limit).  

So the font size **grows fluidly** with the viewport — but never too small or too big.

---

### 🪄 In Tailwind CSS
You can use `clamp()` directly with arbitrary values:

```html
<p class="text-[clamp(24px,5vw,80px)] leading-[1.2]">
  Tea and Botanical Solutions
</p>
```

✅ Works in **Tailwind v3+ and v4**  
✅ Perfect for **hero titles**, **banners**, and **responsive headings**

---

### 🌼 Summary
- `clamp()` keeps text fluid and readable across all screens  
- Great for **modern responsive typography**  
- Combine with `leading-[value]` for balanced line-height
