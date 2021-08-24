# `sliding_window.py`

A piece of code for creating a sliding window in NumPy.

```py
def sliding_window(image, kernel_shape):
  return np.transpose(np.transpose(image[np.arange(kernel_shape[1]) + np.arange(image.shape[0] + 1 - kernel_shape[0])[:, np.newaxis]], (0, 2, 1))[:, np.arange(kernel_shape[0]) + np.arange(image.shape[1] + 1 - kernel_shape[1])[:, np.newaxis]], (0, 1, 3, 2))
```

