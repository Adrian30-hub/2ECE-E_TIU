#### 1) Word Rotation Problem - Creates a function that shifts the first letter of a word to the end.

```python

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

# Execute all test cases
print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))

```

##### Step-by-step procedure
- `def rotate_word(text)` → Defines a function that accepts a string parameter
- `if len(text) != 0:` → Checks whether the input string is non-empty before proceeding
- `a = text[0]` → Extracts the first character of the string
- `b = text[1:]` → Slices the string starting from the first index to the end
- `c = b + a` → Concatenates the values of a and b
- `return c` → Returns the newly formed string back to the function call

#### Outcome
```python
ythonp
ogicl
odeC
A
```

#### 2) Username Builder Problem - Creates a function that convert all letters to lowercase, remove all spaces from the first name, remove all spaces from the last name, and join the processed first and last names using one period (.).

```python

def make_username(first_name, last_name):
    # Make first name clean by converting to lowercase and removing spaces
    first = first_name.lower().replace(" ", "")
    # Make last name clean by converting to lowercase and removing spaces
    last = last_name.lower().replace(" ", "")
    # return concatenated values
    return first + "." + last

# Execute test cases
print(make_username("Ada", "Lovelace"))
print(make_username("Alan", "Turing"))
print(make_username("Ana Maria", "De Leon"))

```

#### Step-by-step procedure
- `def make-username(first_name, last_name)` → Defines a function that accepts two string parameter
- `first = first_name.lower().replace(" ", "")` → Cleans the first name by converting all characters to lowercase and removing spaces
- `last = last_name.lower().replace(" ", "")` → Cleans the last name by converting all characters to lowercase and removing spaces
- `return first + "." = last` → Returns and concatenates the cleaned string values

#### Outcome
```python
ada.lovelace
alan.turing
anamaria.deleon
```

#### 3) Bookend Swap Problem

```python

def swap_bookends(items):
    # Unpack into first element, middle list, and last element
    first, *middle, last = items
    # Return with the first and last elements swapped
    return (last,  *middle, first)

# Execute test cases
print(swap_bookends([1, 2, 3, 4, 5, 6]))
print(swap_bookends(["red", "green", "blue"]))
print(swap_bookends([8, 3]))

```

#### Step-by-step procedure
- `def swap_bookends(items)` → Defines a function that accepts any type of parameter
- `first, *middle, last = items` → Unpacks the sequence so the first item goes to first, the last item goes to last, and all items in between the first and last goes to middle
- `return (last, *middle, first)` → Returns the values handed in the function call but the first and last items swapped

#### Outcome
```python
(6, 2, 3, 4, 5, 1)
('blue', 'green', 'red')
(3, 8)
```

