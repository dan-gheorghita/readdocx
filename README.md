# readDocx.py

**Code Analysis: Extracting Text from a Microsoft Word Document**

The provided Python code is designed to extract the text from a Microsoft Word document (.docx file) and return it as a single string. Here's a breakdown of the code:

### Importing the Required Library

```python
import docx
```

The code starts by importing the `docx` library, which is used to read and manipulate Microsoft Word document files.

### Defining a Function to Extract Text

```python
def getText(filename):
```

The `getText` function takes a single argument `filename`, which is the path to the Microsoft Word document file.

### Loading the Document

```python
doc = docx.Document(filename)
```

Inside the function, the `docx.Document` class is instantiated with the specified `filename`, loading the Microsoft Word document into memory.

### Iterating through Paragraphs and Extracting Text

```python
fullText = []
for para in doc.paragraphs: