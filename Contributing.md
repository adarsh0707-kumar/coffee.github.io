# Contributing to Coffee Shop Web Application (`coffee.github.io`)

First off, thank you for considering contributing to the **coffee.github.io** repository! 🎉 

Whether you are fixing a visual glitch, refining the JavaScript interactive components, improving performance, or enhancing accessibility, your contributions are welcome.

This document provides guidelines and best practices for contributing to this project.

---

## 📋 Table of Contents

- [Code of Conduct](#-code-of-conduct)
- [How Can I Contribute?](#-how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Features](#suggesting-features)
  - [Submitting Pull Requests](#submitting-pull-requests)
- [Development Workflow](#-development-workflow)
  - [1. Fork & Clone](#1-fork--clone)
  - [2. Branching Naming Strategy](#2-branching-naming-strategy)
  - [3. Local Development](#3-local-development)
  - [4. Code Style & Standards](#4-code-style--standards)
- [Commit Message Guidelines](#-commit-message-guidelines)
- [Pull Request Checklist](#-pull-request-checklist)

---

## 📜 Code of Conduct

Please maintain a respectful, supportive, and inclusive environment. Avoid inappropriate, offensive, or discriminatory language in issues, discussions, and pull requests.

---

## 🤝 How Can I Contribute?

### Reporting Bugs
Before creating a bug report, please check existing issues to make sure it hasn't already been reported.

When creating a bug report, include as much context as possible:
- **Title**: A clear, concise summary of the issue.
- **Description**: Detailed steps to reproduce the bug.
- **Environment**: Operating System, Browser type and version, Device (Desktop/Mobile).
- **Screenshots / GIFs**: Visual evidence of the issue if applicable.

### Suggesting Features
Enhancements to the site are always welcome! When opening a feature request:
- Explain **why** the feature is valuable to users.
- Describe **how** you envision the feature working or looking.
- Check the project [Roadmap in README.md](README.md#-roadmap--future-enhancements) to see if it is already planned.

### Submitting Pull Requests
1. Search active Pull Requests to ensure your work does not duplicate existing efforts.
2. Keep your PRs focused: a single PR should address a single feature or bug fix.
3. Follow the repository structure and coding standards detailed below.

---

## 🛠️ Development Workflow

### 1. Fork & Clone
1. Fork the repository on GitHub by clicking the **Fork** button at the top right of the page.
2. Clone your fork to your local machine:
   ```bash
   git clone https://github.com/<your-username>/coffee.github.io.git
   cd coffee.github.io
   ```
3. Add the original repository as an `upstream` remote:
   ```bash
   git remote add upstream https://github.com/adarsh0707-kumar/coffee.github.io.git
   ```

### 2. Branching Naming Strategy
Create a descriptive branch for your changes:
```bash
git checkout -b feature/add-dark-light-toggle
# or
git checkout -b fix/cart-sidebar-scroll-bug
```

Use prefixes like:
- `feature/` for new functionality.
- `fix/` for bug fixes.
- `docs/` for documentation improvements.
- `style/` for pure visual UI updates or code formatting.

### 3. Local Development
Since this project uses vanilla frontend technologies without build tools:
- Simply launch `index.html` in your browser.
- Alternatively, use the **Live Server** extension in Visual Studio Code for real-time reload on saving changes.

### 4. Code Style & Standards

#### 🌐 HTML5
- Use semantic HTML tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
- Maintain clean 4-space or 2-space indentation.
- Ensure all interactive elements have accessible attributes (`alt` tags for images, `aria-label` for icons/buttons).

#### 🎨 CSS3 (`css/style.css`)
- Utilize CSS Custom Variables (`:root`) for colors, fonts, and reused measurements.
- Write responsive styles using mobile-first or desktop-down `@media` queries consistently.
- Avoid inline styling (`style="..."`) inside HTML files.

#### ⚡ JavaScript (`js/script.js`)
- Use modern ES6+ syntax (`const`, `let`, arrow functions, DOM `querySelector`).
- Ensure code is lightweight and zero-dependency.
- Write explanatory comments for non-trivial DOM manipulation or state management logic.

---

## 💬 Commit Message Guidelines

Clear commit messages help maintain clean repository history. Use imperative phrasing in your subject lines:

```text
Format: <type>(<scope>): <short description>

Examples:
feat(cart): add localstorage persistence for cart items
fix(nav): resolve mobile drawer overlap issue on scroll
docs(readme): add contribution guidelines link
```

Common types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`.

---

## 📋 Pull Request Checklist

Before submitting your PR, verify the following:

- [ ] My code follows the established coding style of this repository.
- [ ] Visual updates have been tested across multiple screen sizes (Mobile, Tablet, Desktop).
- [ ] JavaScript changes do not throw console errors.
- [ ] I have updated relevant documentation (`README.md`) if introducing new features or modifying workflows.
- [ ] My commit history is clean and contains descriptive messages.

---

Thank you for helping make this coffee shop project better! ☕