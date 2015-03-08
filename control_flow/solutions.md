# Answers

Problem 1:
```
x = "John Jameson"

if "John" in x:
    print "John is in x"
else:
    print "John is not in x"

if "roger" in x:
    print "Hi Roger!"
elif len(x) > 20:
    print "That's a long string!"
else:
    print "Oh well!"
```

Problem 2:
```python
numbers = range(1001)
div_by_33 = []
for i in numbers:
    if i % 33 == 0:
        div_by_33.append(i)

print div_by_33
```

Problem 3:
```python
characters = ["Donald Duck", "Mickey Mouse", "Daffy Duck", "Goofy", "Minnie Mouse", "Pluto"]

# First we get the sum of all the lengths of the strings
sum = 0
for char in characters:
    sum += len(char)
print "Sum is {}".format(sum)

# Now we will filter to just the list of elements that contain the letter d or m, case-INSENSITIVE
with_d_or_m = [
    char for char in characters
    if "m" in char.lower() or "d" in char.lower()
]
print with_d_or_m
```
