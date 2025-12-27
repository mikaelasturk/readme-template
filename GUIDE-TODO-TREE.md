> 📚 **Navigation:** [README](README.md) | [PLANNING](PLANNING.md) | [TODO](TODO.md) | [How to Use Guide](GUIDE-HOW-TO-USE-TEMPLATE.md) | [Todo Tree Guide](GUIDE-TODO-TREE.md)  

# 🌲 Todo Tree Guide - Connect Your Code with TODO.md
> **Open in preview**  
`Shift + Command + V on Mac`  
`Shift + Control + V on Windows`

This guide explains how to use **Todo Tree** extension in VS Code to link your code comments with your TODO.md file.

## 📋 Table of Contents
- [What This Does](#1)
- [Writing TODO Comments in Your Code](#2)
- [Connecting TODO Comments to TODO.md](#3)
- [Using Todo Tree Sidebar](#4)
- [Customize Todo Tree](#5)
- [Complete Workflow Example](#6)
- [Why This System Works](#7)
- [Quick Start Checklist](#8)

<a id="1"></a>
## 🎯 What This Does
Instead of having TODOs scattered everywhere, Todo Tree:
- ✅ Collects ALL TODO comments from your code
- ✅ Shows them in one place (sidebar)
- ✅ Links them to your TODO.md file
- ✅ Helps you track what needs to be done WHERE in your code

<a id="2"></a>
## 📝 Writing TODO Comments in Your Code
Todo Tree automatically detects these keywords in your code:

### Basic Format:
```javascript
// TODO: Description of what needs to be done
// FIXME: Something that's broken and needs fixing
// HACK: Temporary solution that should be improved
// NOTE: Important information to remember
// [ ]: Unchecked task
// [x]: Completed task
```

<a id="3"></a>
## 🔗 Connecting TODO Comments to TODO.md
You can use a **reference system** to link code comments with your TODO.md:

### Method 1: ID System
**In TODO.md:**
```markdown
## 🔴 High Priority
- [ ] [BTN-001] Add loading state to Button component
- [ ] [BTN-002] Fix button disable functionality
```

**In your code:**
```javascript
// TODO [BTN-001]: Add loading state
// FIXME [BTN-002]: Button doesn't disable properly
```

### Method 2: Link to File Location
**In TODO.md:**
```markdown
## 🔴 High Priority
- [ ] Add loading state (src/components/Button.jsx:15)
- [ ] Fix navbar responsive (src/components/Nav.jsx:42)
```

**In your code:**
```javascript
// TODO: Add loading state - Tracked in TODO.md
```

<a id="4"></a>
## 🌲 Step 4: Using Todo Tree Sidebar
Once you have TODO comments in your code:

### View All TODOs:
1. Click the **Todo Tree icon** in sidebar
2. See all your TODOs organized by file
3. Click any TODO to jump to that line in code

### Filter by Type:
- Click `TODO` to see only TODOs
- Click `FIXME` to see only FIXMEs
- Click `NOTE` to see only notes

### Search TODOs:
- Use the search box at top of Todo Tree panel
- Filter by keyword, file, or tag

<a id="5"></a>
## ⚙️ Customize Todo Tree 
Add this to your VS Code `settings.json`:

```json
{
  "todo-tree.general.tags": [
    "TODO",
    "FIXME",
    "HACK",
    "NOTE",
    "[ ]",
    "[x]",
    "BUG",
    "REVIEW"
  ],
  "todo-tree.general.statusBar": "total",
  "todo-tree.highlights.defaultHighlight": {
    "icon": "check",
    "type": "text",
    "foreground": "#ffffff",
    "background": "#ff6b6b"
  },
  "todo-tree.highlights.customHighlight": {
    "TODO": {
      "icon": "check",
      "foreground": "#ffffff",
      "background": "#4CAF50"
    },
    "FIXME": {
      "icon": "alert",
      "foreground": "#ffffff", 
      "background": "#f44336"
    },
    "NOTE": {
      "icon": "note",
      "foreground": "#000000",
      "background": "#FFC107"
    }
  }
}
```

**To add this:**
1. Press `Cmd + Shift + P` / `Ctrl + Shift + P`
2. Type "Preferences: Open Settings (JSON)"
3. Paste the config above


<a id="6"></a>
## 🔄 Complete Workflow Example
### 1. Plan in TODO.md:
```markdown
## 🔴 High Priority
- [ ] [AUTH-001] Implement login form
- [ ] [AUTH-002] Add JWT token validation
```

### 2. Add comments while coding:
```javascript
// src/components/LoginForm.jsx
// TODO [AUTH-001]: Add form validation
// FIXME [AUTH-001]: Password field not hiding text

export function LoginForm() {
  // [AUTH-001] Implementation here
  return <form>...</form>;
}
```

### 3. Check Todo Tree:
- Open Todo Tree sidebar
- See all [AUTH-001] TODOs in one place
- Click to jump to each location

### 4. Complete and update:
```javascript
// ✅ [AUTH-001] Form validation completed
export function LoginForm() {
  // Validation implemented!
}
```

**In TODO.md:**
```markdown
## ✅ Completed
- [x] [AUTH-001] Implement login form
```

---

<a id="7"></a>
## 🎯 Why This System Works
✅ **Quick overview**: Todo Tree shows ALL tasks from code  
✅ **Context in code**: Comments remind you what needs work  
✅ **Easy navigation**: Click to jump to exact line  
✅ **No duplication**: ID system connects both places  
✅ **Track progress**: Move from TODO → done in both places


<a id="8"></a>
## 🚀 Quick Start Checklist
- [ ] Install Todo Tree extension
- [ ] Add a TODO comment in your code: `// TODO: Test comment`
- [ ] Open Todo Tree sidebar (tree icon)
- [ ] Click the TODO to jump to it
- [ ] Try adding an ID: `// TODO [TEST-001]: My first tagged todo`
- [ ] Create matching entry in TODO.md with same ID

--- 

**That's it!** Now you can keep your tasks organized both in your code and in TODO.md. Happy coding! 🎉
