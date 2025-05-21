# Recipe Rating System

This project is a simple JavaScript-based program that manages recipes by calculating and displaying key information such as average ratings, total ingredients, and difficulty levels for each recipe.

## Table of Contents

* [Features](#features)
* [How It Works](#how-it-works)
* [Usage](#usage)
* [Technologies Used](#technologies-used)
* [Example Output](#example-output)
* [Contributing](#contributing)

## Features

* **Recipe Management**: Stores recipes with details like ingredients, cooking time, and ratings.
* **Average Rating Calculation**: Computes the average rating for each recipe.
* **Ingredient Count**: Determines the total number of ingredients in a recipe.
* **Difficulty Level Assessment**: Assigns a difficulty level (easy, medium, or hard) based on cooking time.

## How It Works

1. **Recipe Objects**: Recipes are defined as JavaScript objects with properties such as `name`, `ingredients`, `cookingTime`, and `ratings`.
2. **Utility Functions**:

   * `getAverageRating(ratings)`: Calculates the average rating from an array of ratings.
   * `getTotalIngredients(ingredients)`: Counts the total number of ingredients in a recipe.
   * `getDifficultyLevel(cookingTime)`: Determines the difficulty level based on cooking time.
3. **Dynamic Updates**: Recipe objects are updated dynamically to include `averageRating`, `totalIngredients`, and `difficultyLevel`.

## Usage

1. Clone the repository or copy the code.
2. Run the program in any JavaScript environment (e.g., browser console or Node.js).
3. View the output in the console to see the recipe information, including calculated properties.

### Code Snippet

```javascript
const recipes = [];
const recipe1 = {
  name: 'Spaghetti Carbonara',
  ingredients: ['spaghetti', 'Parmesan cheese', 'pancetta', 'black pepper'],
  cookingTime: 22,
  totalIngredients: null,
  difficultyLevel: '',
  ratings: [4, 5, 4, 5],
  averageRating: null,
};
// Additional recipes and logic here...
recipes.push(recipe1);
console.log(recipes);
```

## Technologies Used

* JavaScript (ES6+)

## Example Output

```plaintext
Average Rating for Spaghetti Carbonara: 4.5
Total Ingredients for Spaghetti Carbonara: 4
Difficulty Level for Spaghetti Carbonara: easy
[
  {
    name: 'Spaghetti Carbonara',
    ingredients: ['spaghetti', 'Parmesan cheese', 'pancetta', 'black pepper'],
    cookingTime: 22,
    totalIngredients: 4,
    difficultyLevel: 'easy',
    ratings: [4, 5, 4, 5],
    averageRating: 4.5
  },
  // Other recipes...
]
```

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request with your enhancements.
