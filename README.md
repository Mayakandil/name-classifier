
# Name Classifier 📚

This project groups a list of names based on the first letter of each name.  
The program sorts the names alphabetically, creates a dictionary, and stores names under keys matching their starting letter.

---

## 🔧 Code Used

```python
name_list = ["ahmed", "fatma", "ibrahim"]
result = {}

names = sorted(name_list)

for item in names:
    key = item[0].lower()          # First letter of the name
    result.setdefault(key, []).append(item)

print(result)


# 📌 How It Works
- The list of names is sorted alphabetically.
- For each name:
     - A key is created using the first letter of the name.
     - The name is added to a dictionary under that key.
- The dictionary groups names by their starting letter.


# 🧪 Example Output
{
    'a': ['ahmed'],
    'f': ['fatma'],
    'i': ['ibrahim']
}


# 🚀 How to Run
- Install Python 3.x
- Save the script as:
    group_names.py
- Run it using:
    python group_names.py


# 📚 Features
- Groups names alphabetically.
- Automatically handles multiple names per letter.
- Uses dictionary + setdefault for efficient grouping.
- Easy to extend with larger datasets.


# 🔮 Possible Improvements
- Let the user input names manually.
- Load names from a text file.
- Export the grouped dictionary to JSON.
- Add input validation (ignore empty names, trim spaces, etc.).

