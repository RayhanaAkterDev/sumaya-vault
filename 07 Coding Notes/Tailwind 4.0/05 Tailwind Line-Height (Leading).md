---
title: Tailwind Line-Height (Leading)
class: note
date: 2025-10-05
tags:
  - code
  - tailwind
---
# 🌸 Tailwind CSS — Line Height (Leading) Tips, Tricks & Quick Recap

*(For Beginners — Tailwind v4 Explained Clearly)*
(F)

---

## 🧠 What is Line Height?

**Line height** controls **the vertical space between lines of text.**

Think of each line of text as sitting on an invisible “line box.”  
Line-height decides **how tall** that box is.

---

## 📏 How Line Height Works in CSS

When you write:
```css
line-height: 1;
```
it means:
> Each line’s height = **1 × the font size**

So if:
- Font size = 24px → line-height = 24px  
- Font size = 16px → line-height = 16px  
- Font size = 40px → line-height = 40px  

✅ In short:  
> `line-height: 1` = same height as text, no extra vertical space.

---

### 🪶 Visual Feel

| Font Size | Line Height | Look | Feel |
|------------|--------------|------|------|
| 24px | `1` | Tight | Lines almost touch |
| 24px | `1.5` | Normal | Comfortable reading |
| 24px | `2` | Loose | Spacious layout |

🧩 So, **smaller numbers** make text tighter,  
and **larger numbers** make it airier and easier to read.

---

## 💬 Tailwind v4 — Basic Line Height Utilities

Tailwind gives you quick classes for controlling line-height:

| Class                        | Result                                   | Meaning                |
| ---------------------------- | ---------------------------------------- | ---------------------- |
| `leading-none`               | `line-height: 1;`                        | Tight lines            |
| `leading-6`                  | `line-height: calc(var(--spacing) * 6);` | Standard spacing       |
| `leading-7`                  | `line-height: calc(var(--spacing) * 7);` | Readable paragraphs    |
| `leading-8`                  | `line-height: calc(var(--spacing) * 8);` | Spacious blocks        |
| `leading-[1.5]`              | `line-height: 1.5;`                      | Custom numeric spacing |
| `leading-(--my-line-height)` | `line-height: var(--my-line-height);`    | Use CSS variable       |

---

## 🪄 Combine Font Size + Line Height (New in v4)

Tailwind v4 lets you **set both font-size and line-height in one class** 🎉

Example:
```html
<p class="text-lg/7">Hello World</p>
```

That means:
```css
font-size: var(--text-lg);
line-height: calc(var(--spacing) * 7);
```

or use a custom value:
```html
<p class="text-2xl/[1.2]">Tighter Heading</p>
```
Here:
- Font size = `2xl`
- Line height = `1.2`

✅ This “slash syntax” (`text-size/line`) is **new and smarter in v4**.

---

## 💡 Simple Tips for Beginners

1. 🩵 **Use `leading-none`** for big bold headings.  
2. 💚 **Use `leading-7` or `8`** for paragraphs — it’s easy to read.  
3. 💛 **Use `text-size/line`** (like `text-xl/[1.2]`) for control in one place.  
4. 🩷 **Custom spacing?** Add brackets → `leading-[1.5]`.  
5. 💙 **Responsive control?** → `md:leading-8`.  
6. 🧡 **Variable-based line height?** → `leading-(--my-line-height)`.

---

## ⚙️ How Tailwind Calculates It (v4 logic)

In Tailwind v4, numeric leading classes like `leading-6` or `leading-7` are built on a global variable:
```css
line-height: calc(var(--spacing) * 6);
```

You can redefine that:
```css
@theme {
  --spacing: 1px;
}
```

So:
- `leading-6` → `6px`
- `leading-7` → `7px`
- `leading-8` → `8px`

---

## ⚔️ Tailwind v3 vs v4 — Easy Comparison Table

| Feature | Tailwind v3 | Tailwind v4 |
|----------|--------------|-------------|
| Basic syntax | `leading-tight`, `leading-loose`, etc. | `leading-6`, `leading-7`, etc. |
| Combine font-size + line-height | ❌ Not possible | ✅ `text-lg/7` |
| Custom numeric value | ✅ `leading-[1.8]` | ✅ Still works |
| CSS variable use | ❌ Not supported | ✅ `leading-(--my-line-height)` |
| Based on spacing scale | Yes (`theme.lineHeight`) | Yes (`--spacing` variable) |
| Responsive prefixes | ✅ Supported | ✅ Supported |
| Default per font size | Yes | Yes |
| Code simplicity | ❌ Needed two classes | ✅ One class does both |

---

## 🌼 Quick Memory Trick

> “**v3 needed 2 classes — v4 does it in 1!** 🎯”

Example:
```html
<!-- Old way (v3) -->
<p class="text-lg leading-7">Hello</p>

<!-- New way (v4) -->
<p class="text-lg/7">Hello</p>
```
Same look, shorter code ✅

---

## 📘 Quick Recap Table

| Purpose | Recommended Class |
|----------|------------------|
| Big title / hero heading | `text-5xl/[1.1]` or `leading-none` |
| Normal paragraph | `text-base/7` |
| Subheading | `text-xl/[1.2]` |
| Custom spacing | `leading-[1.6]` |
| Responsive line height | `md:leading-8` |

---

✅ **Tailwind Version:** `v4.0+`  
📚 **Docs:** [https://tailwindcss.com/docs/line-height](https://tailwindcss.com/docs/line-height)

---

💡 **Super Simple Recap:**
- `leading-*` → controls line height only  
- `text-size/line` → controls font + line height in one  
- `leading-[1.5]` → custom number  
- `leading-(--variable)` → CSS variable  
- `line-height: 1` → equals the font size (tightest possible)  
- Bigger number = more spacing ✨
