---
title: Tailwind custom fonts working
class: note
date: 2025-10-07
tags:
  - code
  - snippets
  - tailwind
---

```css
@theme {  
    --color-linear-gradient: linear-gradient(to right, #FF0000 0%, #FF8938 100%);  
    --color-dark1: #1C1C1C;  
    --color-dark2: #494949;  
    --color-dark3: #777777;  
    --font-manrop: "Manrope", sans-serif;  
  
    /* how custom fonts works */  
    --text-heading: clamp(1.5rem, 5vw, 5rem);  
    --text-heading--line-height: 1.2;  
    --text-heading--font-weight: 800;  
}  
  
.heading{  
    @apply font-manrop text-dark1 text-[clamp(1.5rem,5vw,5rem)] leading-[1.2];  
}  
  
#test-clamp{  
    @apply text-heading text-blue-400;  
}
```