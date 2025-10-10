---
title: Common Comment Tags Used in IDEs
class: note
date: 2025-10-09
tags:
  - code
---
## 🧩 Common Comment Tags Used in IDEs

| 🔖 Keyword      | 💬 Meaning                           | 🧠 When to Use                                                 |
| --------------- | ------------------------------------ | -------------------------------------------------------------- |
| **TODO:**       | Task to be done later                | A reminder for incomplete or future work.                      |
| **FIXME:**      | There’s a bug that needs fixing      | Code behaves incorrectly or breaks something.                  |
| **BUG:**        | Known bug that must be addressed     | Similar to FIXME but often used for tracking confirmed issues. |
| **NOTE:**       | Important clarification or reminder  | Add context, tips, or reasoning behind code choices.           |
| **HACK:**       | Temporary or dirty workaround        | When code isn’t elegant but works for now.                     |
| **REVIEW:**     | Needs to be reviewed by someone      | Marks parts that require a second look or code review.         |
| **OPTIMIZE:**   | Could be made faster or cleaner      | For performance improvements or refactoring.                   |
| **DEPRECATED:** | This code will be removed soon       | Warns that the code or method is outdated.                     |
| **BUGFIX:**     | Marks the location of a bug fix      | Helps track where a fix was made.                              |
| **CHANGED:**    | Indicates recently modified code     | Useful for collaboration or version control notes.             |
| **QUESTION:**   | Uncertainty that needs clarification | Use when unsure about logic or design decisions.               |
| **WARNING:**    | Potential issue or risk area         | Alert to something fragile or unsafe.                          |
| **SECURITY:**   | Possible security concern            | For sensitive or vulnerable code sections.                     |
| **TEST:**       | Related to testing                   | Notes about test coverage or pending tests.                    |

---

### 🧱 Example Usage in Your Project

```css
/* FIXME: hero-section_title font-size not scaling correctly on mobile */
/* TODO: Add responsive line-height adjustments */
/* OPTIMIZE: Combine repetitive media queries for better maintainability */
/* NOTE: Using clamp() for fluid typography */
```

**Or in JS/React:**

```js
// TODO: Connect this button to the CTA handler
// FIXME: API data not loading correctly on refresh
// OPTIMIZE: Debounce input to reduce API calls
// NOTE: Using state to control modal visibility
```

---

## ## 💡 Bonus Tip for You (especially in WebStorm)

You can **customize recognized tags**:

1. Go to **Settings → Editor → TODO**.    
2. Add your own patterns (e.g., `@sumaya:` or `REFACTOR:`).    
3. Then you’ll see those tags show up in the **TODO panel** automatically!
