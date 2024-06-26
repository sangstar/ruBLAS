## ruBLAS
Linear algebra implementations in Rust with bindings for Python.


```python
import rublas

mat_a = rublas.Matrix([
    [1,2],
    [4,5],
    [1,2],
])

mat_b = rublas.Matrix([
    [7, 8,  9, 46],
    [10,11, 3, 12],
])

if __name__ == "__main__":
    print(mat_a * mat_b)
# Outputs:
# [27 30 15 70 ]
# [78 87 51 244 ]
# [27 30 15 70 ]
```



## Installation
Make sure Rust and Python are installed on your machine, then clone the repository.

```bash
git clone https://github.com/sangstar/ruBLAS.git
```

Install `maturin` via pip.

```bash
pip install maturin
```

Finally, build the crate and install it as a Python module.

```bash
cd ruBLAS
maturin develop
```