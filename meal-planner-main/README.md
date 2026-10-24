# MealMint Health Labs

**Plan Smart. Eat Well.**

MealMint is a responsive, frontend-only meal planning web application built to help react you weight and physical health goals. It uses HTML5, CSS3, Vanilla JavaScript, Fetch API CSV loading, and browser localStorage. There is no backend, no database, no login system, and no AI/API dependency.

## Entry Page

Open:

```text
mealmint-index.html
```

## Included Pages

1. `mealmint-index.html` - Corporate landing workspace
2. `mealmint-goals.html` - Health and fitness goal selection
3. `mealmint-library.html` - Meal library with search and filters
4. `mealmint-planner.html` - Seven-day weekly planner
5. `mealmint-dashboard.html` - Nutrition dashboard
6. `mealmint-grocery.html` - Consolidated grocery list

## Required Folder Structure

```text
mealmint/
├── css/
│   └── mealmint-styles.css
├── js/
│   ├── mealmint-app.js
│   ├── mealmint-planner.js
│   ├── mealmint-nutrition.js
│   └── mealmint-grocery.js
├── resources/
│   ├── mealmint_logo.png
│   ├── style_guide.png
│   ├── meals.csv
│   ├── nutrition_profiles.csv
│   ├── weekly_sample_plan.csv
│   └── grocery_items.csv
├── data/
│   ├── wireframe-landing.png
│   ├── wireframe-planner.png
│   └── wireframe-dashboard-grocery.png
├── mealmint-index.html
├── mealmint-goals.html
├── mealmint-library.html
├── mealmint-planner.html
├── mealmint-dashboard.html
├── mealmint-grocery.html
└── README.md
```

## Features

- Actual `mealmint_logo.png` used in the navbar and landing page
- Brand tagline restored: `Plan Smart. Eat Well.`
- CSV data loaded using the browser Fetch API
- Goal selection saved to localStorage
- Meal library search, meal type filter, cuisine filter, and Add to Plan flow
- Weekly planner with Breakfast, Lunch, Dinner, and Snack slots
- Planner auto-save using localStorage
- Remove meal and Clear All confirmation
- Daily calorie totals in the planner
- Nutrition dashboard with macro totals, daily breakdown, and goal comparison
- Success and warning indicators based on nutrition profile thresholds
- Grocery list generated from the active weekly plan
- Grocery categories, checkboxes, clear checked lines, reset list, and browser print support
- Fully responsive layout down to 320px with stacking below the 768px breakpoint

## CSV Files

The app loads these files from the `resources/` folder:

```text
resources/meals.csv
resources/nutrition_profiles.csv
resources/weekly_sample_plan.csv
resources/grocery_items.csv
```

## How to Run

Because the app uses Fetch API to load CSV files, run it through a local static server instead of opening the HTML file directly with `file://`.

### Option 1: Python

```bash
cd mealmint
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/mealmint-index.html
```

### Option 2: VS Code Live Server

Open the project folder in VS Code, right-click `mealmint-index.html`, and choose **Open with Live Server**.

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript ES6+
- Fetch API
- localStorage
- Static CSV files
