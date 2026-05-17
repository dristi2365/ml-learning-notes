# Classification vs Regression

Both are types of supervised learning but predict different things.

## Classification
Predicts a category — the answer is one of a fixed set of options.

Examples:
- Is this email spam or not spam? → Spam / Not Spam
- What shot is this player doing? → Forehand / Backhand / Smash
- Will a student pass or fail? → Pass / Fail

Easy way to remember: "Which box does this belong to?"

### Binary vs Multiclass:
- Binary — only 2 outputs (Spam or Not Spam)
- Multiclass — more than 2 outputs (Forehand, Backhand, Smash)

## Regression
Predicts a number — the answer can be any value.

Examples:
- What will be the price of this house? → $250,000
- What will the temperature be tomorrow? → 28.5°C
- What will a student's exam score be? → 78.5

Easy way to remember: "What number will this be?"

## Important note — Recommendation Systems:
Recommendation systems don't fit neatly into either category.
They predict what a user would like based on patterns and similarities.
- Collaborative Filtering — finds patterns between users
- Content Based Filtering — finds patterns between items
They are their own category in ML.
