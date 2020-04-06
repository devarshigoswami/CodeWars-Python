Your goal in this kata is to implement a difference function, which subtracts one list from another and returns the result.

It should remove all values from list a, which are present in list b.

`array_diff([1,2],[1]) == [2]`

If a value is present in b, all of its occurrences must be removed from the other:

`array_diff([1,2,2,2,3],[2]) == [1,3]`

APPROACH:
conversion second list to set
filter function: The filter() method filters the given sequence with the help of a function that tests each element in the sequence to be true or not.


CODE:

```python
def array_diff(a, b):
  s = set(b)
  return list(filter(lambda x: x not in b, a))```
