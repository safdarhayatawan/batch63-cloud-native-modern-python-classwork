- If you want to store multiple items, you would need to create a separate variable for each one.

```
student1 = "Rehan"
student2 = "Muzhar"
student3 = "Ibtisam"
```

This approach works fine if you have just a few items. But what if you have 10, 100, or even more? It quickly becomes unmanageable.

- If you want to add or remove an item, you have to manually shift the data around or create new variables.

```
student4 = "Usman"
```

- Accessing an item requires you to remember the exact variable name associated with it.

```
print(student1)
print(student2)
```

# What is List?

A list in Python is like a container that can hold multiple items, one after another. Imagine you have a shopping list where you write down everything you need to buy. A Python list is very similar, but instead of just groceries, it can hold all kinds of things like numbers, words, or even other lists!

### Store Multiple Items Together:

A list allows you to keep multiple items in one place. For example, if you want to keep track of all your students' names, you can store them in a list.

```
students = ["Rehan", "Muzhar", "Ibtisam"]
```

### Access Items by Position:

Lists keep items in the order you put them in. You can access any item by telling Python where it is in the list (starting from 0).

```
print(students[0])
print(students[1])
```

### Change Items:

You can easily change an item in the list if you need to update it.

```
students[0] = "Ahmad"
```

### Adding or Removing elements from list

```
students = ["Rehan", "Muzhar", "Ibtisam"]

# Append a new student
students.append("Usman")
print(students)  # Output: ["Rehan", "Muzhar", "Ibtisam", "Usman"]

# Pop the last student
last_student = students.pop()
print(last_student)  # Output: "Usman"
print(students)      # Output: ["Rehan", "Muzhar", "Ibtisam"]

# Remove a specific student by name
students.remove("Rehan")
print(students)  # Output: ["Muzhar", "Ibtisam"]
```

---

## Indexing

Indexing is how you access individual elements in a list using their position in the list. In Python, lists are zero-indexed, meaning that the first element in a list is at index 0, the second element is at index 1, and so on.

```
               0        1          2
students = ["Rehan", "Muzhar", "Ibtisam"]   # length-1 
             -3         -2        -1
```

## Slicing with Indexes

```
phrase = list("LongLivePakistan!")

```

#### Positive Indexing

```
part1 = phrase[0:4]
print(part1)  # Output: "Long"


part2 = phrase[4:8]
print(part2)  # Output: "Live"


part3 = phrase[8:16]
print(part3)  # Output: "Pakistan"

```

#### Negative Indexing

```
part4 = phrase[-9:-1]
print(part4)  # Output: "Pakistan"


part5 = phrase[-14:-10]
print(part5)  # Output: "Live"


part6 = phrase[:-1]
print(part6)  # Output: "LongLivePakistan"

```

#### Slicing with Steps

```
part7 = phrase[::2]
print(part7)  # Output: "LnLvPksa!"



part8 = phrase[0:8:2]
print(part8)  # Output: "LnLv"

```

Reversing the entire string
```
reversed_phrase = phrase[::-1]
print(reversed_phrase)  # Output: "!natsikaPevignoL"
```

Combining Positive and Negative Indexing with Steps
 
```
part10 = phrase[6:-2:2]
print(part10)  # Output: "vekaP"
```