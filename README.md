# Post-Interview Technical Assessment

Thank you for taking the time to interview with us. As the next step in our hiring process, we'd like to assess your practical coding skills with a short technical task.

## Technical Assessment Instructions

### Objective
Demonstrate your proficiency in Python by completing one of the two tasks provided below. Choose the task that best aligns with your strengths.

### Time Limit
You have 20 minutes to complete the task.

### Submission Instructions
1. Commit your solution to a public GitHub repository on your account.
2. Follow good GitHub practices:
   - Use clear and descriptive commit messages.
   - Organize your repository logically.
   - Include a `README.md` file explaining your solution and how to run it.
3. Share the repository link with us upon completion.

## Tasks (Choose One)

### Option 1: Flatten a Nested Dictionary

**Task Description:**
Implement a function `flatten_dict(d)` that takes a nested dictionary `d` and returns a new dictionary with all nested keys flattened into a single level. The keys in the flattened dictionary should represent the path to each value in the original dictionary, joined by dots (`.`).

**Constraints:**
- All keys are strings.
- Values can be integers, strings, or other dictionaries.
- Assume there are no lists or other data types in the values.

**Example:**

```python
def flatten_dict(d):
    # Your code here

# Example usage:
nested_dict = {
    'a': 1,
    'b': {
        'c': 2,
        'd': {
            'e': 3,
            'f': 4
        }
    },
    'g': {
        'h': 5
    }
}

flattened = flatten_dict(nested_dict)
print(flattened)
```

**Expected Output:**

```python
{
    'a': 1,
    'b.c': 2,
    'b.d.e': 3,
    'b.d.f': 4,
    'g.h': 5
}
```

**Requirements:**
- Your function should handle dictionaries nested to any depth.
- Include error handling for invalid inputs (e.g., non-dictionary inputs).
- Write clean, readable code with appropriate comments.
- Follow Python best practices (e.g., PEP 8).

**If You Have Extra Time:**
- Handle edge cases, such as empty dictionaries or keys with special characters.
- Write additional test cases to cover more scenarios.
- Optimize your code for efficiency.

---

### Option 2: Word Count in a Text File

**Task Description:**
Write a function `word_count(filepath)` that reads a text file specified by `filepath` and returns a dictionary where the keys are words, and the values are the number of times each word appears in the file.

**Constraints:**
- Ignore punctuation and special characters.
- Treat words as case-insensitive (e.g., 'Python' and 'python' are the same word).
- Assume the file exists and is readable.

**Example:**

```python
def word_count(filepath):
    # Your code here

# Example usage:
counts = word_count('sample.txt')
print(counts)
```

**Sample `sample.txt` Content:**

```
Hello world!
This is a sample text file.
Hello Python world.
```

**Expected Output:**

```python
{
    'hello': 2,
    'world': 2,
    'this': 1,
    'is': 1,
    'a': 1,
    'sample': 1,
    'text': 1,
    'file': 1,
    'python': 1
}
```

**Requirements:**
- Handle file I/O operations safely.
- Normalize words by converting them to lowercase.
- Remove punctuation and special characters.
- Write clean, readable code with appropriate comments.
- Follow Python best practices (e.g., PEP 8).

**If You Have Extra Time:**
- Implement error handling for scenarios like file not found or unreadable files.
- Optimize your code for large files.
- Extend the function to accept command-line arguments for file path input.

---

## Additional Guidelines

### Testing
- Include any test cases or examples you used to verify your solution.
- Demonstrate that your code works as expected.

### Code Style
- Use meaningful variable and function names.
- Keep your code organized and modular.
- Comment your code where necessary to explain complex logic.

### GitHub Practices
- **Commit Messages:** Use descriptive messages that explain what changes were made and why.
- **Repository Structure:** Organize your files logically; for example, place your code in a `src` directory and tests in a `tests` directory.
- **README.md:** Provide instructions on how to run your code and any dependencies required.
- **LICENSE (Optional):** Include a license if you prefer.

### What to Ensure
- **Functionality:** Your code should run without errors and meet the task requirements.
- **Efficiency:** While not the primary focus, efficient code is appreciated.
- **Error Handling:** Gracefully handle unexpected inputs or errors where applicable.
- **Adherence to Instructions:** Make sure you have followed all the guidelines provided.

---

## Submission Checklist
- [ ] Complete one of the two tasks within 20 minutes.
- [ ] Commit your code to a public GitHub repository.
- [ ] Follow good GitHub practices (clear commits, proper structure, README).
- [ ] Include test cases or examples demonstrating your code works.
- [ ] Share the GitHub repository link with us.

---

## Final Notes

- **Time Management:** Focus on delivering a working solution first. If you have extra time, you can refine and optimize your code.
- **Communication:** If you encounter any issues or need clarifications, feel free to reach out.
- **Good Luck:** We look forward to seeing your coding skills in action!

Please send the link to your GitHub repository to Jason once you're done.