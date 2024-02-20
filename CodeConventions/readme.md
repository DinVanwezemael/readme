
# Code conventions

Why?





## Method parameters

don't do

```
private void MethodName(string parameters1, string parameter2,
    int parameters3, bool parameter4)
{
    // logic
}
```

instead do

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

don't do

```
private Person MethodName()
{
    return new();
}
```

instead do

```
private Person MethodName()
{
    return new Person();
}
```