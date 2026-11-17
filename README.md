# FridgeFeast

Turn what's in your fridge into a feast.

FridgeFeast is a React Native app we're building for our Mobile Application Development with React Native I course (SODV2205-02). The idea is simple: you type in an ingredient you already have at home, like chicken or eggs, and the app shows you recipes you can make with it. You can also search by meal name or browse categories, open a recipe to see the ingredients, instructions and a video, and save the ones you like to your favorites.

The app doesn't use a database or store anything locally. All recipe data comes live from TheMealDB API.

Team: Byte Kitchen (Bibek Panta and Nyein Chan Tun)

## API

We're using [TheMealDB](https://www.themealdb.com/api.php). It's free and doesn't need a sign-up, which made it a good fit for this project.

Base URL: `https://www.themealdb.com/api/json/v1/1/`

Endpoints we plan to use:

- `filter.php?i=chicken` - search meals by ingredient
- `search.php?s=pasta` - search meals by name
- `categories.php` - get all categories
- `filter.php?c=Seafood` - meals in a category
- `lookup.php?i=52772` - full details of one meal
- `random.php` - a random meal

## Screens

- **Home** - search bar (by ingredient or meal name), a random pick of the day, and a grid of categories
- **Meal List** - results shown in a FlatList
- **Meal Detail** - photo, ingredients, instructions and a YouTube link
- **Favorites** - meals saved during the session
- **About** - info about the app and team

## Built with

- React Native with Expo
- Axios with async/await
- React Navigation (bottom tabs and stack)
- useState, useEffect, useReducer and a custom useApiData hook
- FlatList and Flexbox for layout
- Expo Vector Icons

## How to run it

We're still building the app, so these steps might change a bit in Phase 2.

1. Install Node.js and the Expo Go app on your phone
2. Clone the repo
