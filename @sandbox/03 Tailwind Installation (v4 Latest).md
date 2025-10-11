---
title: Tailwind Installation (v4 Latest)
class: note
date: 2025-10-03
tags:
  - code
  - tailwind
---
# Install Tailwind (v4):

**open `Git Bash` and run the following commands:**

1. Create a new `Vite` project:
	```bash
	npm create vite@latest my-project -- --template vanilla
	```
2. Navigate into the project folder:
	```bash
	cd my-project
	```
3. Install Tailwind CSS with the `Vite` plugin:
	```bash
	npm install tailwindcss @tailwindcss/vite
	```
4. Create `vite.config.js` and paste the following code:

	```js
	import { defineConfig } from 'vite'
	import tailwindcss from '@tailwindcss/vite'

	export default defineConfig({
	  plugins: [
	    tailwindcss(),
	  ],
	})
	```
5. Import `Tailwind` in your `CSS` file:
	```css
	@import "tailwindcss";
	```
6. Run the project:
	```bash
	npm run dev
	```

> **Note:** Make sure to link your `CSS` file in `index.html` for Tailwind styles to work.