# Answers

Problem 1:
```python
def multiply(a, b):
    return a * b
```

Problem 2:
```python
def subrtact(a, b):
    return a - b
```

Problem 3:
```python
# I use list comprehensions since they are quite compact and clean.
def div_by_33(numbers):
    return [
        i for i in numbers
        if i % 33 == 0
    ]
```

Problem 4:
```python
def print_evens_to_10000():
    for k in range(1, 10001):
        if k % 2 == 0:
            print k
```

Problem 5:
```python
def get_max(numbers):
    max = numbers[0]
    for i in numbers:
        if i > max:
            max = i
    return max
```

Problem 6:
```
def is_odd_or_div_by_7(num):
    return num % 2 == 1 or num % 7 == 0

# Lambda function implementation

is_odd_or_divisible_by_7 = lambda num: num % 2 == 1 or num % 7 == 0
```

Problem 7:
```python
# I use `dog` as a dummy variable just to show you
# it doesnt matter what we name that dummy variable
def get_sublist_of_numbers_odd_or_div_by_7(nums):
    return [
        dog for dog in nums if is_odd_or_div_by_7(dog)
    ]
```


Problem 8:
```
def aggregate_counts(order_list):
    orders_by_count = {}
    for order in order_list:
        # if we've already seen this order, increment the count
        if order in orders_by_count:
           orders_by_count[order] += 1
        # otherwise, this is the first time we're seeing it, so set its count to 1
        else:
           orders_by_count[order] = 1
    return orders_by_count
```

Problem 9:
```
from collections import Counter

def aggregate_counts(order_list):
    return Counter(order_list)
```
Problem 10:
```
def get_most_popular_order_data(order_list):
    agg_counts = aggregate_counts(order_list)
    # the key is a function that tells `max` what to sort by
    # in this case, it's the second element of the tuple, e.g. 2 in ("burger", 2)
    # which is just the number of times it appears in the list of orders
    return max(agg_accounts.iteritems(), key=lambda: agg_count[1])
```
