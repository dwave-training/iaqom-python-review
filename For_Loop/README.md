# Use a For Loop
A business wants to pack a shipping container. The objective is to maximize the total monetary value of $N$ total objects that can fit in the container.

- The binary variable, $x_i$, represents whether the object is in the shipping container. If $x_i = 1$, item $i$ is in the container. If $x_i = 0$, item $i$ is not in the container.
  
- The coefficient $c_i$ represents the cost of each item $i$.
  
- The optimization objective is:

$$ \min - \sum_{i=1}^N c_i x_i $$


For this assignment, use a `for` loop to return the value of the optimization objective under the following conditions:

- The total number of items to select from is $N = 4$.	

- The cost of each item is $5, $10, $3, and $4, respectively.

- The second and fourth items are packed in the container.


## Exercise

Open `forloop_practice.py` and complete the following instructions:

1. Create two new lists:

- Name the first list `costs`. Add the following values, in order, to the list: 5, 10, 3, 4. This list represents the cost of each item.

- Name the second list `items`. Add the following values, in order, to the list: 0, 1, 0, 1. This list represents whether an item is packed in the shipping container. If the value is equal to 1, the item is included in the container; if the value is equal to 0, the item is not included in the container.
  
2. Initialize `value` by setting `value = 0`; this is where the final answer will be stored. Note that the value of `value` will change as the program runs.
   
3. On a separate line, use a `for` loop to calculate the following:
   
$$ - \sum_{i=1}^4 \texttt{costs}_i * \texttt{items}_i $$

 and then store the sum in `value`.
   
4. Print `value`, which is the optimization objective's value to your terminal.
