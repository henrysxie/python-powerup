# Objective
- get comfortable with writing functions

# Exercises
Problem 1: Create a function `multiply` that takes two parameters and returns their product.

Problem 2: Create a function `subtract` that takes two parameters and returns their difference.

Problem 3: Let's write a function that takes a variable, which is a list of numbers, and then returns just the ones that are divisible by 33.

Problem 4:. Write a function that takes prints all the even numbers between 1 and 10,000. Use list comprehensions.

Problem 5: Write a function `get_max` that takes a list of numbers and returns the max of those numbers, don't use the builtin `max()` function. Afterward,  try using `max()`

Problem 6: Write a function `is_odd_or_div_by_7` that returns True if a number is odd or divisble by 7 and False otherwise. Then write it using a `lambda` function.

Problem 7:. Use `is_odd_or_div_by_7` and list comprehensions to write a function `get_sublist_of_numbers_odd_or_div_by_7` that takes in a list and returns a sublist of those numbers that are either odd or divisible by 7.

Problem 8. Given a list of food orders, e.g. ```["burger", "fries", "burger", "tenders", "apple pie"]```, write a function `get_aggregate_order_counts` that takes the list and returns a dictionary with the different dishes as keys and the number of times they appear in the list as the values. For example, it takes ```["burger", "fries", "burger", "tenders", "apple pie"]``` and outputs ```
{
   "burger": 2,
   "fries": 1,
   "tenders": 1,
   "apple pie": 1
}```

Problem 9: Use collections.Counter to achieve the same functionality as in Problem 8.

Problem 10: Write a function `get_most_popular_order_data` that takes a list of orders but instead of returning a dictionary with the counts, it just outputs a tuple: the dish that appears the most in the list and the number of times it appears in the list. So the output given the example would be ```("burger", 2)```
