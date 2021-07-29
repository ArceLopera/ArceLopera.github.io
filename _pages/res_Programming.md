---
permalink: /res_Prog/
title: "Resources - Python vs C#"
---

## Variables

Python:

```python
foo = 1
bar = "hi"
something_that_varies = 2 # Though strict immutability in Python isn't common.
something_that_varies += 1
```

C#:

```csharp
var foo = 1; // Equivalent to: int foo
var bar = "hi"; // Equivalent to: String bar
var somethingThatVaries = 2; // Equivalent to: int somethingThatVaries
somethingThatVaries++;
```



## Functions


Python:

```python
# Function definition: takes an argument
def do_domething(some_argument):
  return some_argument + 1


# Function use
results = do_something(3)
```

C#:

```csharp
// Function definition: takes an integer argument, returns an integer
static int DoSomething(int some_argument)
{
  return some_argument + 1;
}

// Function use
var results = DoSomething(3);
```

## Conditionals

Python:

```python
if x == 3:
    # ...
elif x == 0:
    # ...
else:
    # ...
```

C#:

```csharp
if (x == 3)
{
  // ...
}
else if (x == 0)
{
  // ...
}
else
{
  // ...
}
```

```csharp
// Or using a switch:
switch(x) {
  case 3:
    // ...
    break;
  case 0:
    // ...
    break;
  default:
    // ...
    break;
}
```

## Output to the screen


Python:

```python
x = 5
print("x has the value %s" % x);
```

C#:

```csharp
var x = 5;
Debug.Log("x has the value {0}", x);
```

## Lists of variable size

Python:

```python
i = ["a", "b", "c"];
i.append("d"); 
print(i[1]); # outputs b
```

C#:

```csharp
var i = new List<String>() { "a", "b", "c" };
i.Add("d");
Debug.Log(i[1]); // outputs b
```

## Iterating over the elements in a list

Python:

```python
i = ["a", "b", "c"];
for j in i:
    print(j):
```

C#:

```csharp
var i = new List<String>() { "a", "b", "c" };

foreach(var j in i) {
  Debug.Log(j);
}

i.ForEach((j) => Debug.Log(j));
```