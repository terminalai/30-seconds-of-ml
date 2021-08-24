# `beta.py`

A function to claculate the beta function for "multiples of 1/2", i.e. x,y where {x}, {y} = 0.5 or 1.0.

```py
def beta(x, y):
    """
    Actual Beta Function based on the Simplified Gamma Function in gamma.md.
    """
    return gamma(x)*gamma(y)/gamma(x+y)
```
