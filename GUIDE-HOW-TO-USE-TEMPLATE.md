> 📚 **Navigation:** [README](README.md) | [PLANNING](PLANNING.md) | [TODO](TODO.md) | [How to Use Guide](GUIDE-HOW-TO-USE-TEMPLATE.md) | [Todo Tree Guide](GUIDE-TODO-TREE.md)  

# 📖 How to Use This Template
> **Open in preview**  
`Shift + Command + V on Mac`  
`Shift + Control + V on Windows`

Welcome! This guide will help you understand how to use these project documentation templates for your school projects.

## 📋 Table of Contents
- [What's Included?](#1)
- [Getting Started](#2)
  - [Step 1: Copy the Template](#s1)
  - [Step 2: Start with PLANNING.md](#s2)
  - [Step 3: Convert Plan to Tasks (TODO.md)](#s3)
  - [Step 4: Code & Track Progress](#s4)
  - [Step 5: Document in README.md](#s5)
- [The Complete Workflow](#3)
- [Helpful Tools](#4)
- [Next Steps](#5)

<a id="1"></a>
## 🎯 What's Included?
This template contains three interconnected files:

1. **[README.md](README.md)** - The main documentation for your finished project
2. **[PLANNING.md](PLANNING.md)** - Your planning document before you start coding
3. **[TODO.md](TODO.md)** - Your active task list during development

<a id="2"></a>
## 🚀 Getting Started
<a id="s1"></a>
### Step 1: Copy the Template
1. Copy all template files to your project folder
2. Keep all three files at the root of your project

---

<a id="s2"></a>
### Step 2: Start with PLANNING.md
Before writing any code, fill out the PLANNING document.

---

<a id="s3"></a>
### Step 3: Convert Plan to Tasks (TODO.md)
Once your plan is ready, break it down into small, actionable tasks in TODO.md.

**Example workflow:**  
From PLANNING:
```
Tech Stack: React, Vite, React Router
```

To TODO:
```markdown
## 🔴 High Priority
- [ ] Setup Vite project
- [ ] Install React Router
- [ ] Create basic folder structure
```

**Tips:**
- Break big features into smaller tasks
- Use priorities (🔴 High, 🟡 Medium, 🟢 Low)
- Add deadlines for important tasks: `(Due: 2025-01-15)`
- Move tasks to "In Progress" when you start 
- Move to "Completed" when done ✅

**Update frequency:** Daily or whenever you work on the project

---

<a id="s4"></a>
### 💻 Step 4: Code & Track Progress

As you work on your project:

#### Update TODO.md regularly:
```markdown
## 🚧 In Progress
- [x] Setup Vite project ← Move to Completed when done
- [ ] Install React Router ← Currently working on this

## ✅ Completed  
- [x] Created folder structure
- [x] Added color palette to CSS
```

> TIP  
Optional: Use code comments  
Link your code to TODO items:
```javascript
// TODO: Add error handling for API calls
// See TODO.md - Medium Priority #2

const fetchData () => {
  // your code here
}
```

---

<a id="s5"></a>
### 📝 Step 5: Document in README.md

As features get completed, update your README:

**During development:**
- Update "Features" section when you complete a feature
- Add screenshots as you build the UI
- Keep tech stack accurate

**After completion:**
- Fill in "Execution" section (how you built it)
- Write "Retrospect" (what you learned)
- Add live demo link
- Make sure all sections are complete

<a id="3"></a>
## 🔄 The Complete Workflow

```
1. PLAN (PLANNING.md)
   ↓
   Decide what to build and how
   
2. BREAK DOWN (TODO.md)
   ↓
   Create small, actionable tasks
   
3. EXECUTE (TODO.md + Code)
   ↓
   Work through tasks, update status
   
4. DOCUMENT (README.md)
   ↓
   Document completed features and learnings
```


<a id="4"></a>
## 🛠️ Helpful Tools
### VS Code Extensions:
1. **Todo Tree** - Shows all TODO comments from your code
   - Install: Search "Todo Tree" in VS Code Extensions
   - Usage: Write `// TODO: task description` in your code
   
2. **Markdown All in One** - Makes editing these files easier
   - Quick checkbox toggling: `Cmd/Ctrl + Shift + X`

### GitHub:
- Commit with meaningful messages: `git commit -m "feat: add search bar component"`
- Reference tasks: `git commit -m "fix: navbar bug (TODO.md #5)"`

<a id="5"></a>
## 📚 Next Steps
Ready to start? Here's your checklist:

- [ ] Copy these template files to your project
- [ ] Read through PLANNING.md and start filling it out
- [ ] Break your plan into TODO items
- [ ] Start coding and tracking progress
- [ ] Update README as you complete features
- [ ] (Optional) Install Todo Tree extension  

**Remember:** These templates are tools to help you, not rules to restrict you. Adapt them to fit your workflow and project!

Good luck! 🎉
