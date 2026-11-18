Examine the code (but don't run it yet!). Predict the final printed value, then run it to see if your prediction was correct.

```py-cell
my_list = [[1, 3], [4, 6], [8, 1]]

result = 1

for inner in my_list:
    current = 0
    for number in inner:
        current = current + number
    result = result * current

print(result)
```

# Explanation

Click below to reveal an explanation of the behaviour of the code.

>[!HIDDEN]
> For this exercise, it is useful to start with understanding the inner loop, but in terms of what data it processes, and what operation it performs.
>
> ## Step 1: The Value of `inner`{.python}
> 
> In the outer iteration of the loop, `inner`{.python} takes on each value in `my_list`{.python}. This will be a list and is what the inner loop will iterate over.
>
> ## Step 2: Understand the Inner Sum
>
> For each inner list, the code computes its sum of `inner`{.python} values in `current`{.python}.
>
> * `[1, 3]`{.python} gives `4`{.python}
> * `[4, 6]`{.python} gives `10`{.python}
> * `[8, 1]`{.python} gives `9`{.python}
>
> ## Step 3: Multiply into the Result
>
> Each inner sum is multiplied into `result`{.python}:
>
> $$
> \mathrm{result} = 1 \times 4 \times 10 \times 9 = 360
> $$
