# NumPy Summary

A quick revision guide for the NumPy topics covered in notebooks **2–14**.

> ⭐ **ML IMPORTANT** = functions/concepts that you are likely to use frequently while learning Machine Learning.

---

## 1. Array Attributes

| Function / Attribute | Syntax | One-line description |
|---|---|---|
| ⭐ `ndim` | `a.ndim` | Tells the number of dimensions of an array. |
| ⭐ `shape` | `a.shape` | Tells the size of the array along each dimension. |
| `size` | `a.size` | Gives the total number of elements in an array. |
| `itemsize` | `a.itemsize` | Gives the number of bytes used by each element. |
| ⭐ `dtype` | `a.dtype` | Tells the data type of elements in the array. |
| ⭐ `astype()` | `a.astype(dtype)` | Converts an array from one data type to another. |

---

## 2. Array Creation

| Function | Syntax | One-line description |
|---|---|---|
| ⭐ `np.array()` | `np.array([1,2,3])` | Creates a NumPy array from a Python sequence. |
| ⭐ `np.arange()` | `np.arange(start, stop, step)` | Creates evenly spaced values using a fixed step. |
| ⭐ `reshape()` | `a.reshape(rows, cols)` | Changes the shape of an array without changing its elements. |
| `np.ones()` | `np.ones(shape)` | Creates an array filled with `1`. |

### Common example

```python
a1 = np.arange(10)
a2 = np.arange(12, dtype=float).reshape(3,4)
a3 = np.arange(8).reshape(2,2,2)
```

---

# 3. Array Operations ⭐

| Operation | Syntax | One-line description |
|---|---|---|
| Addition ⭐ | `a + b` | Adds corresponding elements of arrays. |
| Subtraction ⭐ | `a - b` | Subtracts corresponding elements. |
| Multiplication ⭐ | `a * b` | Multiplies corresponding elements. |
| Division ⭐ | `a / b` | Divides corresponding elements. |
| Power | `a ** 2` | Raises every element to a power. |
| Greater than ⭐ | `a > x` | Checks which elements are greater than `x`. |
| Less than | `a < x` | Checks which elements are less than `x`. |
| Greater/equal | `a >= x` | Checks which elements are greater than or equal to `x`. |
| Less/equal | `a <= x` | Checks which elements are less than or equal to `x`. |
| Equal | `a == x` | Checks equality element-wise. |
| Not equal | `a != x` | Checks inequality element-wise. |
| AND ⭐ | `(condition1) & (condition2)` | Combines conditions where both must be true. |
| OR ⭐ | `(condition1) \| (condition2)` | Combines conditions where either condition can be true. |

---

# 4. Array Functions ⭐

| Function | Syntax | One-line description |
|---|---|---|
| ⭐ `max()` | `a.max()` / `np.max(a)` | Returns the maximum value. |
| ⭐ `min()` | `a.min()` / `np.min(a)` | Returns the minimum value. |
| ⭐ `sum()` | `a.sum()` / `np.sum(a)` | Adds all elements. |
| `prod()` | `a.prod()` / `np.prod(a)` | Multiplies all elements. |
| ⭐ `max(axis=1)` | `a.max(axis=1)` | Finds maximum value row-wise in a 2D array. |
| ⭐ `max(axis=0)` | `a.max(axis=0)` | Finds maximum value column-wise in a 2D array. |
| ⭐ `sum(axis=1)` | `a.sum(axis=1)` | Calculates the sum of each row. |
| ⭐ `sum(axis=0)` | `a.sum(axis=0)` | Calculates the sum of each column. |

---

# 5. Statistical Functions ⭐

| Function | Syntax | One-line description |
|---|---|---|
| ⭐ `mean()` | `np.mean(a)` / `a.mean()` | Calculates the average of values. |
| ⭐ `median()` | `np.median(a)` | Returns the middle value after ordering the data. |
| ⭐ `std()` | `np.std(a)` / `a.std()` | Measures the spread of values using standard deviation. |
| ⭐ `var()` | `np.var(a)` / `a.var()` | Measures variance, which is the squared spread from the mean. |
| ⭐ `np.dot()` | `np.dot(a, b)` | Calculates the dot product of arrays/vectors. |
| `np.round()` | `np.round(a)` | Rounds values to the nearest number. |
| `np.floor()` | `np.floor(a)` | Rounds values down to the nearest integer. |
| `np.ceil()` | `np.ceil(a)` | Rounds values up to the nearest integer. |

### ⭐ ML connection

`np.mean()`, `np.std()`, `np.var()` and `np.dot()` are especially important for ML.

---

# 6. Indexing and Slicing ⭐

| Concept | Syntax | One-line description |
|---|---|---|
| 1D indexing ⭐ | `a[2]` | Accesses one element using its index. |
| 2D indexing ⭐ | `a[1,2]` | Accesses an element using row and column. |
| 3D indexing | `a[1,0,1]` | Accesses an element using layer, row and column. |
| Negative indexing | `a[-1]` | Accesses elements from the end. |
| Basic slicing ⭐ | `a[start:stop]` | Selects a range of elements; stop is not included. |
| Step slicing | `a[start:stop:step]` | Selects elements using a step. |
| Reverse | `a[::-1]` | Reverses an array. |
| 2D row slicing ⭐ | `a[0:2, :]` | Selects specific rows and all columns. |
| 2D column slicing ⭐ | `a[:, 0:3]` | Selects all rows and specific columns. |

---

# 7. Array Iteration

| Function / Concept | Syntax | One-line description |
|---|---|---|
| Normal iteration | `for i in a:` | Iterates through elements/rows of an array. |
| Nested iteration | `for i in a: for j in i:` | Used to access individual elements of a 2D array. |
| 3D iteration | Nested loops | Uses three levels of loops to access a 3D array. |
| `np.nditer()` | `for i in np.nditer(a):` | Iterates over every element regardless of array dimensions. |

---

# 8. Array Reshaping ⭐

| Function / Attribute | Syntax | One-line description |
|---|---|---|
| ⭐ `reshape()` | `a.reshape(rows, cols)` | Changes array shape while keeping the same elements. |
| ⭐ Transpose | `a.T` | Converts rows into columns and columns into rows. |
| `np.hstack()` | `np.hstack((a,b))` | Joins arrays horizontally, side by side. |
| `np.vstack()` | `np.vstack((a,b))` | Joins arrays vertically, one below another. |
| `np.hsplit()` | `np.hsplit(a, parts)` | Splits an array horizontally into parts. |
| `np.vsplit()` | `np.vsplit(a, parts)` | Splits an array vertically into parts. |

---

# 9. Advanced Indexing ⭐

## Fancy Indexing

| Syntax | One-line description |
|---|---|
| ⭐ `a2[[0,2,1]]` | Selects multiple specific rows in the given order. |
| ⭐ `a2[:,[0,2,3]]` | Selects all rows but only specific columns. |

## Boolean Indexing ⭐⭐⭐⭐⭐

| Syntax | One-line description |
|---|---|
| ⭐ `a[a > 5]` | Filters values greater than `5`. |
| ⭐ `a[a % 2 == 0]` | Filters even numbers. |
| `a[a % 2 != 0]` | Filters odd numbers. |
| ⭐ `a[(a > 2) & (a < 8)]` | Filters values satisfying both conditions. |
| ⭐ `a[(a > 5) & (a % 2 == 0)]` | Filters values that are both greater than `5` and even. |
| `a[(a < 2) \| (a > 7)]` | Filters values satisfying either condition. |

**Very important ML concept:** Boolean indexing is frequently used for filtering and preprocessing data.

---

# 10. Broadcasting ⭐⭐⭐⭐⭐

| Concept | Syntax / Example | One-line description |
|---|---|---|
| Scalar broadcasting ⭐ | `a + 10` | Applies one scalar value to every element. |
| Array broadcasting ⭐ | `a + b` | Performs operations on arrays with compatible shapes. |
| Shape comparison | `(2,3)` vs `(3,)` | Shapes are compared from right to left. |
| Broadcasting rule | Equal dimensions | Matching dimensions are compatible. |
| Broadcasting rule | One dimension is `1` | A dimension of `1` can be expanded to match. |
| Missing dimension | `(3,)` → `(1,3)` | Missing dimensions are treated as `1`. |

**Main rule:** Compare dimensions from **right to left**. They must either be equal or one of them must be `1`.

---

# 11. Mathematical Functions for ML ⭐

## Sigmoid

| Function / Expression | Syntax | One-line description |
|---|---|---|
| ⭐ `np.exp()` | `np.exp(x)` | Calculates the exponential value `e^x`. |
| ⭐ Sigmoid | `1 / (1 + np.exp(-x))` | Converts any real input into a value between `0` and `1`. |

### Formula

```text
σ(x) = 1 / (1 + e^(-x))
```

Main use: **binary classification**.

## Mean Squared Error

```python
mse = np.mean((actual - predicted) ** 2)
```

Used to measure the average squared difference between actual and predicted values.

---

# 12. Missing Values ⭐⭐⭐⭐⭐

| Function / Syntax | One-line description |
|---|---|
| ⭐ `np.nan` | Represents a missing numerical value. |
| ⭐ `np.isnan(a)` | Checks every element and returns `True` where the value is NaN. |
| ⭐ `a[np.isnan(a)]` | Extracts only the missing values. |
| ⭐ `~np.isnan(a)` | Reverses the Boolean mask to identify non-missing values. |
| ⭐ `a[~np.isnan(a)]` | Extracts only non-missing values. |
| ⭐ `np.sum(np.isnan(a))` | Counts the number of missing values. |

### Remember this pattern

```python
np.isnan(a)          # find missing
a[np.isnan(a)]       # get missing
a[~np.isnan(a)]      # get non-missing
```

---

# 13. Plotting Graphs

For graph plotting, NumPy is generally used together with Matplotlib.

| Function | Syntax | One-line description |
|---|---|---|
| `np.linspace()` ⭐ | `np.linspace(start, stop, num)` | Creates evenly spaced values. |
| `np.sin()` | `np.sin(x)` | Calculates sine values. |
| `plt.plot()` ⭐ | `plt.plot(x, y)` | Plots lines and continuous curves. |
| `plt.scatter()` ⭐ | `plt.scatter(x, y)` | Plots individual data points. |
| `plt.xlabel()` | `plt.xlabel("x")` | Sets the x-axis label. |
| `plt.ylabel()` | `plt.ylabel("y")` | Sets the y-axis label. |
| `plt.title()` | `plt.title("Title")` | Sets the graph title. |
| `plt.show()` | `plt.show()` | Displays the graph. |

### Graph examples

```python
y = 2*x + 3       # straight line
y = x**2          # parabola
y = np.sin(x)     # sin wave
plt.scatter(x, y) # scatter plot
```

---

# 14. NumPy Tricks ⭐

| Function | Syntax | One-line description |
|---|---|---|
| ⭐ `np.sort()` | `np.sort(a)` | Returns sorted values. |
| ⭐ `np.append()` | `np.append(a, values)` | Adds values to an array and returns a new array. |
| ⭐ `np.concatenate()` | `np.concatenate((a,b), axis=0)` | Joins arrays along an existing axis. |
| ⭐ `np.unique()` | `np.unique(a)` | Returns unique values and removes duplicates. |
| ⭐ `np.expand_dims()` | `np.expand_dims(a, axis)` | Adds a new dimension to an array. |
| ⭐ `np.where()` | `np.where(condition)` | Finds positions where a condition is true. |
| ⭐ `np.argmax()` | `np.argmax(a)` | Returns the index of the maximum value. |
| ⭐ `np.argmin()` | `np.argmin(a)` | Returns the index of the minimum value. |
| ⭐ `np.cumsum()` | `np.cumsum(a)` | Returns the cumulative/running sum. |
| `np.percentile()` | `np.percentile(a, p)` | Returns the value below which a given percentage of observations fall. |
| `np.histogram()` | `np.histogram(a, bins)` | Calculates frequency distribution using bins. |
| ⭐ `np.corrcoef()` | `np.corrcoef(a,b)` | Measures the linear correlation between variables. |
| ⭐ `np.isin()` | `np.isin(a, values)` | Checks whether each element exists in another collection. |
| `np.flip()` | `np.flip(a)` | Reverses the elements of an array. |
| `np.put()` | `np.put(a, indices, values)` | Replaces values at specified indices. |
| `np.delete()` | `np.delete(a, indices)` | Removes elements at specified indices and returns a new array. |

---

# 15. Set Functions

| Function | Syntax | One-line description |
|---|---|---|
| `np.union1d()` | `np.union1d(a,b)` | Returns all unique values present in either array. |
| `np.intersect1d()` | `np.intersect1d(a,b)` | Returns values common to both arrays. |
| `np.setdiff1d()` | `np.setdiff1d(a,b)` | Returns values present in `a` but not in `b`. |
| `np.setxor1d()` | `np.setxor1d(a,b)` | Returns values present in only one of the two arrays. |

---

# ⭐⭐⭐ ML Priority List

These are the NumPy concepts/functions from these notebooks that I should be able to use comfortably for ML:

### Must Know ⭐⭐⭐⭐⭐

```text
np.array()
np.arange()
reshape()
a.shape
a.ndim
a.dtype
astype()
```

```text
+  -  *  /  **
```

```text
mean()
std()
var()
sum()
max()
min()
np.dot()
```

```text
Indexing
Slicing
Boolean Indexing
Fancy Indexing
Broadcasting
```

```text
np.isnan()
np.where()
np.concatenate()
np.unique()
np.expand_dims()
np.argmax()
np.argmin()
```

### Very Useful ⭐⭐⭐⭐

```text
np.median()
np.percentile()
np.cumsum()
np.histogram()
np.corrcoef()
np.isin()
np.sort()
np.append()
np.delete()
np.flip()
```

### ML Mathematical Concepts ⭐⭐⭐⭐⭐

```text
np.exp()
Sigmoid
Mean Squared Error
```

---

# 🧠 NumPy → ML Connection

A simple way to remember where NumPy fits into ML:

```text
Raw Dataset
     ↓
NumPy Arrays
     ↓
Inspect shape / dtype
     ↓
Indexing + Slicing
     ↓
Boolean Filtering
     ↓
Handle Missing Values
     ↓
Reshape + Broadcasting
     ↓
Statistics / Scaling calculations
     ↓
Mathematical Operations
     ↓
ML Model
```

The most important NumPy skills for ML are **arrays, shapes, indexing, Boolean indexing, broadcasting, vectorized operations, statistics and mathematical operations**.

---

## Files Covered

This README summarizes the functions and concepts that could be verified from the available notebooks:

- `2_Array_Attributes.ipynb`
- `3_Array_Operations.ipynb`
- `4_Array_Functions.ipynb`
- `5_Statistical_Functions.ipynb`
- `6_Array_Indexing_and_Slicing.ipynb`
- `7_Array_Iteration.ipynb`
- `8_Array_Reshaping.ipynb`
- `9_Advance_Indexing.ipynb`
- `10_Broadcasting.ipynb`
- `11_Mathematical_Functions_in_NumPy.ipynb`
- `12_Working_with_Missing_Values.ipynb`
- `13_Plotting_Graphs.ipynb`
- `14_NumPy_Tricks.ipynb`

**Note:** `1` is not present in the available file set, so its contents have not been guessed or added. Once that notebook is available, its functions can be added to make this a complete **1–14 NumPy README**.
