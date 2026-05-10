
---

# Suggested `reflection.md`

```markdown
# Reflection

## What Copilot Generated

I used GitHub Copilot to help generate several functions in my project, including `load_data()`, `clean_column_names()`, and `handle_missing_values()`. I prompted Copilot by writing descriptive comments above each function explaining what the function should accomplish. For example, before writing `handle_missing_values()`, I added a comment saying the function should fill missing prices and quantities using median values.

Copilot quickly generated working starter code that used pandas functions like `fillna()` and `pd.to_numeric()`. It also suggested try/except handling for loading the CSV file, which improved the script’s reliability.

## What I Modified

Although Copilot generated useful starting points, I modified several parts of the code. I changed variable names to make them more readable and added additional comments explaining why each cleaning step matters. I also adjusted the text-cleaning logic to remove quotation marks and normalize spacing because the original Copilot suggestion did not fully handle inconsistent whitespace.

Additionally, I added separate functions for duplicate removal and date cleaning to keep the script more organized and easier to understand. I tested the script several times and adjusted the order of cleaning operations so that invalid rows were removed after missing values were handled.

## What I Learned

This project helped me better understand how pandas can be used for real-world data cleaning tasks. I learned how to standardize text fields, convert data types, handle missing values, and remove invalid records in a structured workflow.

I also learned that GitHub Copilot works best as a coding assistant rather than a complete solution. It saved time by generating boilerplate code and pandas syntax, but I still needed to review the logic carefully and make changes based on the dataset’s problems. One example was that Copilot initially suggested dropping missing values completely, but I decided filling them with median values was more appropriate for preserving data.

Overall, the project showed me how AI tools can improve productivity while still requiring human judgment and testing.
