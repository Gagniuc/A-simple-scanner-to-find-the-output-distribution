# A simple scanner to find the output distribution

Ex. (140) - A simple scanner to find the output distribution, is presented here in three programming languages: Python, MATLAB, and JavaScript. Although the implementations differ in syntax, the underlying concept remains identical across all three versions. Each code sample is reproduced from its respective volume of the series <i>Coding Examples from Simple to Complex</i> (Springer, 2024).
***

## Example in Python:

```python
def compute(x):
    return x + x / x - x * x

def distribution(start, stop):
    t = ""
    for i in range(start, stop):
        t += str(compute(i)) + "\n"
    return t

a = distribution(3, 21)
print(a)
``` 

```text
Python output:
-5.0
-11.0
-19.0
-29.0
-41.0
-55.0
-71.0
-89.0
-109.0
-131.0
-155.0
-181.0
-209.0
-239.0
-271.0
-305.0
-341.0
-379.0
```

## Example in Javascript:

```javascript
let a = distribution(3, 21);
print(a);

function distribution(start, stop){
    
    let t = "";
    
    for (let i = start; i < stop; i++) {
        t += compute(i) + "\n";
    }
    
    return t;
}

function compute(x){
    return x + x / x - x * x;
}
```

```text
Javascript output:
-5.0
-11.0
-19.0
-29.0
-41.0
-55.0
-71.0
-89.0
-109.0
-131.0
-155.0
-181.0
-209.0
-239.0
-271.0
-305.0
-341.0
-379.0
```

## Example in Matlab:

```matlab
a = distribution(3, 21);
disp(a);

function t = distribution(start, stop)
    t = "";
    for i = start:(stop-1)
        t = t + compute(i) + newline;
    end
end

function result = compute(x)
    result = x + x / x - x * x;
end
```

```text
Matlab output:
-5.0
-11.0
-19.0
-29.0
-41.0
-55.0
-71.0
-89.0
-109.0
-131.0
-155.0
-181.0
-209.0
-239.0
-271.0
-305.0
-341.0
-379.0
```

## References

- <i>Paul A. Gagniuc. Coding Examples from Simple to Complex - Applications in Python, Springer, 2024, pp. 1-245.</i>
- <i>Paul A. Gagniuc. Coding Examples from Simple to Complex - Applications in MATLAB, Springer, 2024, pp. 1-255.</i>
- <i>Paul A. Gagniuc. Coding Examples from Simple to Complex - Applications in Javascript, Springer, 2024, pp. 1-240.</i>

***
