# MealMap — Indian Cooking Guide

A lightweight, responsive static web app that provides a visual guide and map to popular Indian recipes. Built with plain HTML/CSS/JavaScript and using localStorage to persist user-added recipes. The site ships with an initial curated database of 60 recipes (30 veg + 30 non-veg).

---

## Features
- Responsive recipe grid with thumbnails and tags (region, veg/non-veg)
- Search by dish name or ingredient
- Filter by region and category
- Recipe detail modal with:
  - Ingredients (checkable)
  - Step-by-step instructions
  - Built-in 5-minute kitchen timer
- Add custom recipes (saved to localStorage)
- No backend required — static and easy to host

---

## Tech / Files
- index.html — single-page static app (HTML/CSS/JS)
- Uses:
  - Vanilla JavaScript (no frameworks)
  - CSS variables and responsive grid
  - LocalStorage key: mealmap_recipes
- Images referenced from Unsplash (external URLs)

---

## Quick start (local)
1. Clone the repo:
   git clone https://github.com/appdev993-alt/cooking123.git
2. Open the site:
   - Option A: Open index.html directly in your browser
   - Option B (recommended for consistent behavior with fetch/local paths):
     - Python: python3 -m http.server 8000
     - Node: npx serve
     - Then open http://localhost:8000

---

## Usage
- Browse recipes on the main grid.
- Click a recipe card to open details, use the timer, or check off ingredients.
- Use the search input to find recipes by name or ingredient.
- Use filter buttons to narrow by category/region.
- Click "+ Add Custom Recipe" to add your own; it will be stored in your browser's localStorage and appear at the top of the list.

Local changes are stored only in the browser that created them. To share custom recipes across users, add a backend or export/import feature.

---

## Data
- initialRecipes array in index.html contains 60 initial recipe objects with fields:
  - id, title, category (e.g., ["North","Veg"]), time, image, ingredients[], steps[]
- localStorage key used: mealmap_recipes

---

## Contributing
- Suggestions, bug reports, and PRs welcome.
- If you want this to become a multi-user app:
  - Add an API for storing recipes and user authentication
  - Replace localStorage with server-side storage (database)
  - Add image upload handling and validation

---

## Possible improvements
- Create JSON data file and load dynamically
- Add recipe import/export (JSON)
- Persist user settings (theme, timer presets)
- Accessibility improvements (a11y labels, keyboard navigation)
- Offline support via Service Worker (PWA)
- Tests and CI for linting/build

---

## License
Add a license file as desired (MIT recommended). This repository does not include an explicit license—please add LICENSE.md or let me know which license you prefer and I can add it.

---

## Credits
- Unsplash (recipe images referenced via Unsplash URLs)
- Built as a simple static demo to explore Indian recipes and localStorage usage

---

Would you like me to create README.md in the repository with this content (I can commit it for you)?  

— GitHub Copilot Chat Assistant
