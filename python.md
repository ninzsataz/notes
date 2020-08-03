## Python basics

### Splitting strings

```python
s = ['Hi there Sam']
s.split()

>>> ['Hi', 'there', 'Sam!']
```

### Looping through multiple lists with zip()

```python
name = ['Pete', 'John', 'Elizabeth']
age = [6, 23, 44]

for n, a in zip(name, age):
    print('{} is {} years old'.format(n, a))

>>> Pete is 6 years old
>>> John is 23 years old
>>> Elizabeth is 44 years old
```

### The in and not in operators

```python
'howdy' in ['hello', 'hi', 'howdy', 'heyas']

>>> True
```

```python
'howdy' not in ['hello', 'hi', 'howdy', 'heyas']

>>> False
```

### Numpy Built-in Methods

#### arrange
returns evenly spaced values within a given interval

```python
np.arrange(0,10)

>>> array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
```

```python
np.arange(0,11,2)

>>> array([ 0,  2,  4,  6,  8, 10])
```

#### zeros and ones
generates arrays of zeros or ones

```python
np.zeros(3)

>>> array([ 0.,  0.,  0.])
```

```python
np.ones((3,3))

>>> array([[ 1.,  1.,  1.],
           [ 1.,  1.,  1.],
           [ 1.,  1.,  1.]])
```

#### linspace
returns evenly spaced numbers over a specified interval

```python
np.linspace(0,10,3) # three numbers from [0,10]

>>> array([  0.,   5.,  10.]) 
```

#### eye
creates an identity matrix

```python
np.eye(4)

>>> array([[ 1.,  0.,  0.,  0.],
           [ 0.,  1.,  0.,  0.],
           [ 0.,  0.,  1.,  0.],
           [ 0.,  0.,  0.,  1.]])
```

#### random.rand
creates an array of the given shape and populates it with random samples from a **uniform distribution over ```[0,1)```**

```python
np.random.rand(2,3)

>>> array([[ 0.66660768,  0.87589888,  0.60260888],
           [ 0.70027668,  0.85572434,  0.8464595 ]])
```

#### random.randn
returns a sample (or samples) from the **standard normal distribution**

```python
np.random.randn(2)

>>> array([-0.27954018,  0.90078368])
```

#### random.randint
returns random integers from ```(low, high]```

```python
np.random.randint(1,100, 3)

>>> array([8, 13, 96])
```

### Numpy Array Attributes & Methods

#### reshape
returns an array containing the same data with a new shape

```python
arr = np.arange(25)

arr.reshape(5,5)

>>> array([[ 0,  1,  2,  3,  4],
           [ 5,  6,  7,  8,  9],
           [10, 11, 12, 13, 14],
           [15, 16, 17, 18, 19],
           [20, 21, 22, 23, 24]])
```

#### max, min, argmax, argmin
returns max/min values *or* used to find their index locations via argmax/argmin

```python
ranarr = np.random.randint(0,50,5)
ranarr
>>> array([10, 12, 41, 17, 49])

ranarr.max()
>>> 41

ranarr.argmax()
>>> 2
```







