# Data
This folder contains the data used in my research articles, saved in Python's pickle format for easy access and reproducibility.

## What is Pickle?
Pickle is a module in Python used for serializing and deserializing objects. Serialization is the process of converting a Python object into a byte stream so it can be saved to a file or transferred over a network. Deserialization is the reverse process, converting a byte stream back into a Python object.

In this repository, the data files are stored in **Pickle format** (`.pkl`). These files can be loaded directly into Python programs.

---

## How to Load Pickle Data in Python

To load the data stored in a Pickle file, you can use the following code:

```python
import pickle

# Specify the path to your pickle file
file_path = "your_file_name.pkl"

# Open the file in binary read mode
with open(file_path, "rb") as file:
    data = pickle.load(file)

# Now, 'data' contains the Python object stored in the Pickle file
print(data)
