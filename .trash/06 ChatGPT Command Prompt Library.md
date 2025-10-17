---
class: note
title: ChatGPT Command Prompt Library  
status: In Progress
date: 2025-08-03 09:56 am
---

⬆️:: [[@notes|NoteLab]]

[[2025-08-03]]

# 💬 ChatGPT Command Prompt Library  

**Purpose**: Reusable, standard prompt commands for interacting with ChatGPT or Soulbot professionally, efficiently, and with clear output.

---

## 🧭 Prompting Philosophy

✅ Always define:
- The **task** (what you want)
- The **context** (language, topic, format)
- The **style** (tone or structure you prefer)

🚫 Avoid:
- Vague commands like “help me” or “explain this”
- Asking multiple complex things at once
- Relying on one-shot prompts — iterate!

---

## 🧱 Prompt Command Structure

🟩 Action: [What you want AI to do]  
🟦 Context: [Topic, language, input]  
🟨 Format/Style: [Required format, output type, tone]

Example:

> 🟩 Action: Generate README  
> 🟦 Context: JavaScript topic: Arrays  
> 🟨 Format/Style: Use my standard learning-focused README format with sections: tags, overview, explanation, pro tip, file reference, navigation.

---

## 📁 Standard Prompt Templates (Grouped by Use Case)

### 📄 Documentation & Notes

```plaintext
Generate a README for the topic: [X]  
Use this format: [paste your format or describe sections briefly]  
Focus on clarity for beginner developers. Add one real-world insight or pro tip.
```

```plaintext
Create an Obsidian-style note on: [X]  
Structure it with headings, bullet points, and a learning checklist.
```

---

### 💻 Code Generation

```plaintext
Generate a basic [language] demo that shows: [topic/concept]  
Include comments and a short explanation at the bottom.
```

```plaintext
Create a reusable [function/class/component] in [language] that solves: [problem description]  
Follow clean code principles.
```

```plaintext
Convert this [plain JS code] to a React component.  
Use hooks where appropriate and modular structure.
```

---

### 🧪 Code Review & Debugging

```plaintext
Review the following code and point out errors or bad practices.  
Language: [X]  
Code: [paste code here]
```

```plaintext
This code throws an error: [error message]  
Here's the code: [paste code]  
Explain what's wrong and how to fix it.
```

```plaintext
Optimize this code for readability and performance:  
[paste code]  
Return only the improved version with short explanation.
```

---

### 🛠️ Project Planning & Structure

```plaintext
Suggest a folder structure for a [React + Laravel] full stack app.  
Include frontend, backend, API, and shared resources folders.
```

```plaintext
Create a checklist for building a [project type]  
Use phase-wise steps with deliverables for each.
```

```plaintext
Plan the database schema for a [project] in Laravel  
Include table names, relationships, and migration tips.
```

---

### ✍️ Commit Messages

```plaintext
Generate a conventional commit message for:  
Action: [what was added/fixed]  
Scope: [folder/topic]  
Follow this format:  
<type>(<scope>): <action> + short summary
<body with short line breaks>
```

---

### 📚 Learning & Practice Guidance 

```plaintext
Give me a practice plan for mastering [X] in [Y weeks]  
Include phases, resources, and project suggestions.
```

```plaintext
Break down this concept: [X] into small practice tasks  
Make it suitable for beginners building confidence.
```

---

### 🧠 Thinking Partner Prompts

```plaintext
I’m planning to build [project].  
Ask me 5 questions to clarify the purpose and structure before starting.
```

```plaintext
Help me brainstorm 3 ideas for this feature: [describe feature or goal]
```

```plaintext
Review my idea and give suggestions to make it more user-friendly:
[describe idea or app]
```

---

## ✨ Bonus: Your Signature Prompt Add-on

Use this tag at the end of any request to get clean, professional output:

```plaintext
Return the result in a well-formatted markdown block, with proper headings and comments. Keep the tone semi-formal and easy to follow.
```

---

## 🔁 Prompting Tips Checklist

- [ ] Did I define one clear action?
- [ ] Did I provide enough context (topic, language, structure)?
- [ ] Am I asking one task at a time?
- [ ] Did I try before asking AI to build it?
- [ ] Will this output improve my project or understanding?

✅ If all yes → Run prompt.  
❌ If no → Refactor or break down prompt.
