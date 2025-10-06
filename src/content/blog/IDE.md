---
title: "Integrated Development Environments (IDEs)"
description: "Software that consolidates all the tools a programmer needs!"
coverImage: "/What-is-IDE.gif"
category: "Language Development"
inDev: False
pubDate: "2025-10-06"
updatedDate: "2025-10-06"
publishDate: "October 10th"
---

# Integrated Development Environments
IDEs are pretty much the main tool in your belt for coding. They contain code editors, compilers, debuggers and more all within the same UI. Below are some common IDEs

# Integrated Development Environments

IDEs are pretty much the main tool in your belt for coding. They contain code editors, compilers, debuggers, and more—all within the same UI. Below are some common IDEs.

---

## Common IDEs:

- **Visual Studio Code (VS Code)**  
- **PyCharm**  
- **IntelliJ IDEA**  
- **Xcode**  
- **Android Studio**  


---

## VS Code

**Visual Studio Code (VS Code)** is one of the most popular code editors developed by Microsoft. It’s lightweight compared to something like Visual Studio (which is a different editor), but still highly useful.

### Key Features:
- **IntelliSense:** Smart autocompletion and syntax highlighting for many languages.  
- **Integrated Terminal:** Run commands and scripts without leaving the editor.  
- **Debugger:** Built-in debugging support for multiple languages.  
- **Extensions Marketplace:** Thousands of extensions to add new features, themes, and tools.  
- **Version Control:** Built-in Git integration for committing, branching, and pushing changes.  
- **Snippets & Emmet:** Quickly insert boilerplate code or HTML/CSS shortcuts.  
- **Multi-root Workspaces:** Manage multiple projects in one window.  
- **Live Share:** Real-time collaborative coding with others.  
- **Settings Sync:** Sync your extensions, settings, and themes across devices.

### Stuff You Can Do in VS Code:
- **Code in any language** — from Python and JavaScript to C++, Go, and Rust.  
- **Use Jupyter Notebooks directly in VS Code** for data science and experimentation.  
- **Run a local development server** and preview web apps live.  
- **Customize the UI** with themes, icons, and layout options.  
- **Automate tasks** using built-in terminals or tasks.json scripts.  
- **Use Remote Development** to code directly in containers, WSL, or remote servers.  
- **Pair program with Live Share** for instant collaboration.  
- **Integrate with AI tools** like GitHub Copilot for code suggestions.  

---

### Setup Guide

1. **Download and Install VS Code**
   - Go to [https://code.visualstudio.com/](https://code.visualstudio.com/)  
   - Download the installer for your operating system (Windows, macOS, or Linux).  
   - Follow the installation prompts.

2. **Install Language Extensions**
   - Open the **Extensions** panel (`Ctrl+Shift+X` or `Cmd+Shift+X` on Mac).  
   - Search for and install language packs:  
     - *Python*  
     - *C/C++*  
     - *JavaScript / TypeScript*  
     - *Java*  
     - *HTML / CSS*  

3. **Set Up Git Integration**
   - Install [Git](https://git-scm.com/) if you haven’t already.  
   - Open the Source Control panel (`Ctrl+Shift+G`).  
   - Initialize or clone a repository directly from VS Code.

4. **Customize Your Editor**
   - Go to **File → Preferences → Settings** to adjust fonts, themes, and behavior.  
   - Try popular themes like *One Dark Pro* or *Dracula Official*.  
   - Install an icon pack such as *Material Icon Theme* for better file visualization.

5. **Install Useful Extensions**
   - **Prettier**  
   - **ESLint** 
   - **GitLens** 
   - **Live Server** 
   - **Jupyter** 
   - **GitHub Copilot** 

6. **Test Your Setup**
   - Open a folder or create a new project.  
   - Write a small script (`print("Hello, VS Code!")`).  
   - Run it using the integrated terminal or debugger.



## Challenges

1. **Simply Install VS Code or another IDE** (100 pts)

2. **Do of the Following**
    - Change Theme (50 pts)
    - Add at least one extension (50 pts)
    - 

3. **Build Your Own VS Code Setup** (200 pts)
    - Set up VS Code to connect to a remote server, and run code from there (More on this next week, ENGR Servers).

    - Configure a tasks.json file to automate builds, tests, or scripts.

    - Build your own VS Code color theme or tweak an existing one.

    - Install and use GitHub Copilot (or another AI coding assistant) to write or refactor code.



## **Tips for Challenge 3:**
### Automate Tasks with `tasks.json`

1. In your project, open **Terminal → Configure Tasks → Create tasks.json file from template**.  
2. Choose a template (e.g., “Others”).  
3. Add your task configuration inside `.vscode/tasks.json`, like this:

   ```json
   {
     "version": "2.0.0",
     "tasks": [
       {
         "label": "Run Python Script",
         "type": "shell",
         "command": "python",
         "args": ["app.py"],
         "group": {
           "kind": "build",
           "isDefault": true
         },
         "problemMatcher": []
       }
     ]
   }
4. Run the task with Ctrl+Shift+B

### Create or Edit a Custom Color Theme

1. Press `F1` → **Developer: Generate Color Theme from Current Settings**.  
2. VS Code will create a `.json` theme file.  
3. Save it to your `.vscode/extensions` folder or a custom theme directory.  

#### To tweak an existing theme:
1. Open the theme’s `.json` file.  
2. Edit colors like `"editor.background"` or `"editorCursor.foreground"`.  
3. Reload VS Code and select your theme under **File → Preferences → Color Theme**.  

🖌️ **Pro tip:** Try the **Yo Code** extension generator to build a publishable theme extension:  
```bash
npm install -g yo generator-code
