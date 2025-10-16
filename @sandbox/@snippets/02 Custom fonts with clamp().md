---
title:
class: note
date:
tags:
---
##### Different way to right custom font with `clmap()` related

```css
@import 'tailwindcss';  
  
@theme {  
    --color-linear-gradient: linear-gradient(to right, #FF0000 0%, #FF8938 100%);  
    --color-dark1: #1C1C1C;  
    --color-dark2: #494949;  
    --color-dark3: #777777;  
    --font-manrop: "Manrope", sans-serif;  
  
    /* header-section heading custom fonts */  
    --text-heading: clamp(2rem, 5vw, 5rem);  
    --text-heading--line-height: 1.2;  
    --text-heading--font-weight: 800;  
  
    --space-right: clamp(5rem, 4vw, 12rem);  
}  
  
#header-section h1{  
    @apply font-manrop text-dark1 text-heading pr-[var(--space-right)];  
    /*padding-right: var(--space-right);*/  
}
```