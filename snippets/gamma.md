# `gamma.py`

A function to claculate the gamma function for "multiples of 1/2", i.e. x where {x} = 0.5 or 1.0.

```py
def gamma(n):
    """
        A Simplified Gamma Function for "powers" of 1/2
	Gamma Function for Integers are given by: Γ(n) = (n-1)!
	Gamma Function for Values ending with 1/2: Γ(n) = 0.5 * 1.5 * ... * (n-1) * √(π)
		    
	Gamma Function is generally given by the following expression as coded below.
	"""
	return np.arange(1 - (n%1), n).prod() * np.pi ** (n%1)
```
