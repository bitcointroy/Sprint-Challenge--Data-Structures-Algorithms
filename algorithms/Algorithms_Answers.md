## Exercise I

a. This would be O(n). On the first pass, a is set to n squared, and in n-1 additional passes, a will equal n cubed.

b. O(log n). We're halving the elements we're searching through on each pass. This makes it log(2) of n. If we were able to cut the field to a tenth, it would be log(10) of n.

c. REALLY BAD O(64 \* (sqrt(n)/2)), which I think is in the red zone on the big-O cheatsheet http://bigocheatsheet.com/

## Exercise II

a. Pseudocode:

```
function max_difference(array):
  if length(array) <= 1:
    return 0 # 0 - 0 = 0 and x - x = 0
  max = array[0]
  min = array[0]
  for each x in array:
    if x < min: min = x
    if x >= max: max = x
  return max - min
```

b. I'd start on the 3rd floor. If the egg breaks, go to the second floor and try again. If it doesn't break, go to the 6th floor. Basically, if the egg doesn't break, go up 3 floors. If it does break, go down 1.

## Exercise III

a. Quicksort, pivot = array[0], presorted array

The running time of this would be linear - O(n). You still have to "touch" each element of the array, but you only do so once.

b. Quicksort, pivot = median

The running time of this would also be linear - O(n). You "touch" each element of the array only once.

Side note: technically, the time complexity would be O(n + 1) with the `+ 1` being added for concatenating the lists. However, this simplifies to simply O(n).
