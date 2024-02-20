
# Code conventions

Why?





## Method parameters

❌ don't do

```
private void MethodName(string parameters1, string parameter2,
    int parameters3, bool parameter4)
{
    // logic
}
```

✅ instead do

```
private void MethodName(
    string parameters1,
    string parameter2,
    int parameter3,
    bool parameter4
)
{
    // logic
}
```
## Method return

❌ don't do

```
private Person MethodName()
{
    return new();
}
```

✅ instead do

```
private Person MethodName()
{
    return new Person();
}
```
## Spacing

### if statement

❌ don't do

```
if (data.Success) 
    persons.Add(new Person 
    {
        FirstName = "John",
        LastName = "Doe"
    });

```

✅ instead do

```
if (data.Success) 
{
    persons.Add(new Person 
    {
        FirstName = "John",
        LastName = "Doe"
    });
}

```

### if else statement

❌ don't do

```
if (data.Success) 
    //
else 
{
    persons.Add(new Person 
    {
        FirstName = "John",
        LastName = "Doe"
    });
}
```

✅ instead do

```
if (data.Success) 
{
    // logic
}
else 
{
    persons.Add(new Person 
    {
        FirstName = "John",
        LastName = "Doe"
    });
}
```