# sort.js
[![Build Status](https://travis-ci.org/jongha/sort.js.png?branch=master)](https://travis-ci.org/jongha/sort.js)
[![Coverage Status](https://coveralls.io/repos/jongha/sort.js/badge.png)](https://coveralls.io/r/jongha/sort.js)
[![Dependency Status](https://gemnasium.com/jongha/sort.js.png)](https://gemnasium.com/jongha/sort.js)

Sort Library for Javascript

## `Test case`

* Case 1: Totally descending 2,000 data set to ascend.
* Case 2: Totally ascending 2,000 data set to descend.
* Case 3: Random 2,000 data set to ascend.
* Case 4: Random 2,000 data set to descend.

## `Usage`

This script is prototype of Javascript Array. First, includes the script block like below where you want. 

```
<script src="./dist/sort.min.js"></script>
```

And use it. It is simple.

```
var data = [1,2,3,4,5];
```


### `Bubble Sort`

The code is very simple But, slow.

Speed: 640 ms (Speed of test cases)

Time complexity: O(n^2)

```
data.bubble({ order: 'desc' }); // data == [5,4,3,2,1]
data.bubble({ order: 'asc' }); // data == [1,2,3,4,5]
```

### `Quick Sort`

Speed: 21 ms (Speed of test cases)

Time complexity: O(nlogn)

Faster then Bubble sort.

```
data.quick({ order: 'desc' }); // data == [5,4,3,2,1]
data.quick({ order: 'asc' }); // data == [1,2,3,4,5]
```

### `Merge Sort`

Speed: 15 ms (Speed of test cases)

Time complexity: O(nlogn)

Faster then Quick sort. Almost same speed with Quick Sort.

```
data.merge({ order: 'desc' }); // data == [5,4,3,2,1]
data.merge({ order: 'asc' }); // data == [1,2,3,4,5]
```

### `Heap Sort`

Speed: 18 ms (Speed of test cases)

Time complexity: O(nlogn)

Faster then Quick sort. (The code is not optimize yet.)

```
data.heap({ order: 'desc' }); // data == [5,4,3,2,1]
data.heap({ order: 'asc' }); // data == [1,2,3,4,5]
```

### `Insertion Sort`

Not Implemented

### `Selection Sort`

Not Implemented

### `Binary Sort`

Not Implemented