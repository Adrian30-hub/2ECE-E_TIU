<img width="687" height="407" alt="image" src="https://github.com/user-attachments/assets/8dce8e1f-2aa5-4290-bf8d-82f8074a15a8" /> 

### 1) Word Rotation Problem - Creates a function that shifts the first letter of a word to the end.

`python

def rotate_word(text):
    # Check if the input string is not empty to avoid error
    if len(text) != 0:
        # Extract First Character
        a = text[0]
        # Extract remaining elements from 1 to end
        b = text[1:]
        # Concatenate a and b
        c = b + a
        # Return value
        return c


print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))

`

#### Step-by-step procedure
`def rotate_word(text)` → Defines a function that accepts a string parameter
-`if len(text) != 0:` → Checks whether the input string is non-empty before proceeding
-`a = text[0]` → Extracts the first character of the string
-`b = text[1:]` → Slices the string starting from the first index to the end
-`c = b + a` → Concatenates the values of a and b
-`return c` → Returns the newly formed string back to the function call


`→
