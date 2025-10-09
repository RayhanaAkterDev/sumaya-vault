---
title: Tailwind (v4) Custom Styles & Reusability
class: note
date: 2025-10-04
tags:
  - code
  - tailwind
---

# Tailwind Custom Styles & Reusability

Tailwind provides multiple ways to extend, customize, and reuse styles efficiently. Below are the main approaches:

---

### 1. Adding Custom Values with Square Brackets

You can apply arbitrary values directly inside utility classes using square brackets:

```html
<p class="text-[#f1f1f1] p-[225px]">Custom styled text</p>
```

---

### 2. Using `@theme` for Custom Variables

Tailwind allows defining custom design tokens with the `@theme` directive:

```css
@theme {
  --color-offWhite: #f1f1f1;
}

body {
  background: var(--color-offWhite);
}
```

```html
@theme{
		--color-offWhite: #f1f1f1;
	}
	
	body{
		backgournd: offWhite;
	}
```

---

### 3. Applying Global Styles with `@layer base`

Use the `base` layer to apply global styles (similar to CSS resets or typography defaults):

```css
@layer base {
  h1 {
    color: blue;
  }

  p {
    @apply p-4 text-lg bg-red-400;
  }
}
```

---

### 4. Creating Reusable Components with `@layer components`

Define custom component classes using `@apply`:

```css
@layer components {
  .card {
    @apply p-10 w-3/6 rounded-lg bg-offWhite;
  }
}
```

---

### 5. Defining Utilities with `@utility`

Custom utilities can be created for frequently used patterns:

```css
@utility flex-center {
  @apply flex justify-center items-center;
}
```

---

📌 **Reference**:  

![[all the available tailwind directives name.png]]

---

## Tailwind Component Libraries

For a list of popular component libraries, see the next page:  
[[05 Tailwind Component Libraries]]