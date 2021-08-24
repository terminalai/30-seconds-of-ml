# `pearson_correlation.py`

Computes Pearson Correlation Coefficient, r, for a given x-y dataset pairing.

```py
def corr(data):
    norm = data - data.mean(axis=0)
    return norm.prod(axis=1).sum() / np.sqrt((norm**2).sum(axis=0).prod())
```
