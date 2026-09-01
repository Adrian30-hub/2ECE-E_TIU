# 2ECE-E_TIU

def rotate_word(text):
    # Check if the input string is not empty to avoid error
    if len(text) != 0:
        # Extract First Character
        a = text[0]
        # Extract remaining elements from 1 to end
        b = text[1:]
        # Concatenate a and b
        c = b + a
        return c
        # Print output
        print(c)

print(rotate_word("python"))
print(rotate_word("logic"))
print(rotate_word("Code"))
print(rotate_word("A"))

ythonp
ogicl
odeC
A
