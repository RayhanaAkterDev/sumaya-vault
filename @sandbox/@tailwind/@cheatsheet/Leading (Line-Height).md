---
title: Tailwind Line-Height (Leading)
class: note
date: 2025-10-07
tags:
  - tailwind
  - cheatsheet
aliases:
  - tailwind_cheatsheet
---
🧭 Tailwind CSS v4 — Line-Height (`leading-*`) Quick Reference

| Class                        | Result                                                              | Meaning / When to Use                      |
| ---------------------------- | ------------------------------------------------------------------- | ------------------------------------------ |
| `leading-none`               | `line-height: 1;`                                                   | Lines are tight — good for big titles      |
| `leading-6`                  | `line-height: calc(var(--spacing) * 6);`                            | Standard, balanced spacing                 |
| `leading-7`                  | `line-height: calc(var(--spacing) * 7);`                            | Comfortable reading paragraphs             |
| `leading-8`                  | `line-height: calc(var(--spacing) * 8);`                            | Spacious text blocks                       |
| `leading-9`                  | `line-height: calc(var(--spacing) * 9);`                            | For long-form content                      |
| `leading-10`                 | `line-height: calc(var(--spacing) * 10);`                           | Very open, airy layout                     |
| `leading-[1.5]`              | `line-height: 1.5;`                                                 | Custom numeric value (unitless)            |
| `leading-[32px]`             | `line-height: 32px;`                                                | Custom pixel-based line-height             |
| `leading-(--my-line-height)` | `line-height: var(--my-line-height);`                               | Uses your CSS variable                     |
| `text-lg/6`                  | `font-size: var(--text-lg); line-height: calc(var(--spacing) * 6);` | Combined text size + line-height shorthand |
| `text-xl/[1.2]`              | `font-size: var(--text-xl); line-height: 1.2;`                      | Combine both in one class                  |
| `text-2xl/(--heading-line)`  | `font-size: var(--text-2xl); line-height: var(--heading-line);`     | Use custom property in combined shorthand  |

---

#### 💡 Quick Tips

1. `leading-*` = standalone control (line-height only).    
2. `text-size/line` = shorthand (font-size + line-height).    
3. `--spacing` = Tailwind’s internal spacing variable (default ~0.25rem or 4px per unit).    
4. `leading-none` locks line height to the font size (1:1 ratio).    
5. For responsive design:    
    - `sm:leading-7 md:leading-8` works perfectly in v4.