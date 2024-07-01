# T2A1-B



# Quick Sort and Merge Sort are two sorting algorithms

Let's examine **Quick Sort** and **Merge Sort**, two well-known sorting algorithms. Consider them as several approaches to organising a disorganised space; each has a unique strategy and degree of effectiveness.

## Quick Sort

**Quick Sort** is similar to an algorithmic speedster. It completes the task by employing a tactic known as "divide and conquer." This is how it operates:

1. **Select a Pivot:** Assume that you are organising books. One book is chosen as the pivot.
2. **Partition the Books:** Place the books in such a way that the taller books are on the right and the shorter books are on the left of the pivot.
3. **Repeat the Process:** Next, select a new pivot, divide, and so forth for each of the left and right groups, repeating the process until everything is organised.

### Showcase

- **Optimal and Mean Case:** O(n log n) - In this scenario, the pivot performs exceptionally well in dividing the books equally.
- **Worst Case:** O(n²) - If you consistently choose the lowest or largest book, the splits will be incredibly unequal.

### Effectiveness

- **Space Complexity:** O(log n), as it requires additional space only for the steps it is recalling.
- Because Quick Sort makes efficient use of your computer's memory (cache), it typically completes tasks more quickly in practice.

### Big O Explanation
The O(n log n) average case arises because each step divides the data set into two parts, and the depth of the recursion is log n. The O(n²) worst case happens when the pivot selections result in highly unbalanced partitions, like always picking the smallest element as the pivot.

## Merge Sort

The dependable and steady one is **Merge Sort**. It employs divide and conquer tactics as well, but more methodically:

1. **Divide the Books**: Make two divisions in your stack of books.
2. **Sort Each Half:** Assign individual labels to each half.
3. **Merge Them Back:** In the end, combine the two separated parts once more.

### Showcase

- O(n log n) is the **best**, average, and worst case scenario. No matter how disorganised the pile was initially, it always takes the same length of time.

### Effectiveness

- **Space Complexity:** O(n) due to the necessity for additional space to keep the halves during the merger. Although it requires more memory, it is quite dependable, which may be a drawback for those with a lot of books.

### Big O Explanation
Merge Sort consistently divides the list in half, resulting in a time complexity of O(n log n) for all cases. The merging process requires additional space proportional to the size of the input, hence O(n) space complexity.

## Comparative

### Understanding Algorithms
- While Quick Sort and Merge Sort employ distinct techniques, they both divide the problem into smaller parts.
- While Merge Sort consistently divides the data in half, Quick Sort's effectiveness can vary depending on how well the pivot splits the data.

### Big O Notation

- **Quick Sort:**
  - O(n log n) is the best and average case.
  - The worst case is O(n²).
  - O(log n) for space complexity.
- **Merge Sort:**
  - O(n log n) is the best, average, and worst case.
  - O(n) for space complexity.

### Effectiveness and Relevance

- **Quick Sort:** 
  - Effectively uses memory and sorts in place, making it ideal for large datasets. 
  - If you choose a better pivot, you can adjust it to prevent the worst-case scenario.
- **Merge Sort:**
  - It maintains the order of equal things since it is steady.
  - Ideal for circumstances requiring reliable performance.
  - For very large datasets, the additional space it requires may be a disadvantage.

### Realistic Use Cases

- **Quick Sort** is the method of choice if you wish to use memory effectively and require a quick, all-purpose sort.
- **Merge Sort** is the best option if you can tolerate the additional memory usage and require a consistent sort when working with linked lists.

In conclusion, Quick Sort and Merge Sort are both superior algorithms, each with their own advantages. Because Quick Sort uses memory efficiently, it is frequently faster in real-world applications; however, Merge Sort offers reliable, steady performance, making it the best option for some jobs.



### Refernces

GeeksforGeeks. (n.d.). Quick Sort: https://www.geeksforgeeks.org/quick-sort/
GeeksforGeeks. (n.d.). Merge Sort: https://www.geeksforgeeks.org/merge-sort/
Khan Academy. (n.d.). Quick Sort: https://www.khanacademy.org/computing/computer-science/algorithms#quick-sort
Khan Academy. (n.d.). Merge Sort: https://www.khanacademy.org/computing/computer-science/algorithms#merge-sort
Wikipedia. (n.d.). Quicksort: https://en.wikipedia.org/wiki/Quicksort
Wikipedia. (n.d.). Merge Sort: https://en.wikipedia.org/wiki/Merge_sort
Programiz. (n.d.). Quick Sort: https://www.programiz.com/dsa/quick-sort
Programiz. (n.d.). Merge Sort: https://www.programiz.com/dsa/merge-sort



### Comprehending Linear Search and Binary Search

Searching for a specific element in a list by scanning each element in order.

#### Linear Search

##### How It Operates:
Let's say you're searching through an unkempt stack of books for a book. Starting at the top of the stack, you search through each book individually until you locate the one you're looking for when using a linear search strategy.

**Actions:**
1. **Commence at the outset**: Take the first book out.
2. **Examine the book**: Verify if it meets your requirements.
3. **If it's the right book**: Congratulations, you're done!
4. **If not**: Continue with the following book and go on.
5. **Finish**: Proceed until the book is located or you run out of books. It's not there if you get to the finish without finding it.

##### Performance:
- **Best Case**: O(1) 
  - You locate the book right away.
- **Average Case**: O(n) 
  - You will typically read through roughly half of the books.
- **Worst Case**: O(n) 
  - The book is either the final one on the stack or it isn't there at all.

Finding your book in a large stack can take some time, but linear search is easy to use and works well for tiny heaps.

#### Binary Search

##### How It Operates:
Imagine for a moment that your books are neatly placed alphabetically. By splitting and conquering, binary search facilitates a considerably faster book discovery.

**Actions:**
1. **Divide the Stack**: Examine the book in the centre of the stack first.
2. **Verify that the Middle Book** is the one you wish to use.
3. **If it's the correct book**: Great, you're done!
4. **If Not**: Select your book's position in the stack, placing it either at the top or bottom.
5. **Modify Your Search**: Go back and repeat with the other half, ignoring the part where your book isn't allowed to be.
6. **Repetition**: Continue halving the stack until the book is located or it is reduced to zero.

##### Performance:
- **Optimal Case**: O(1)
  - The book is located in the initial middle check.
- **Average Case**: O(log n) 
  - You reduce the remaining stack by half with each check.
- **Worst Case**: O(log n)
  - In the worst situation, you can locate the book or determine it isn't there with just a few checks.

For huge, well-organized book stacks, binary search is significantly faster. It closes in on the possible locations of the book quickly.

### Comparing the Two

**Effectiveness**:
- **Linear Search**: As the number of books increases, time does as well. You could check up to 100 times for 100 books.
- **Binary Search**: Time grows logarithmically. Because log2(100) = 7, you'll only need roughly 7 tests for 100 books.

**When to Apply It**:
- **Linear Search**: Ideal for small or unsorted stacks. It's simple and doesn't require that the books be read chronologically.
- **Binary Search**: Ideal for sorted stacks of considerable size. It only functions if the books have already been sorted, however it is really quick.

**Real-World Illustration**:
- **Linear Search**: Similar to searching a disorganised drawer for a certain item.
- **Binary Search**: Using the alphabetical order to navigate to a section, much like searching for a name in a phone book (if those are still in use!).

### References
GeeksforGeeks: Linear Search: https://www.geeksforgeeks.org/linear-search/
Khan Academy: Linear Search: https://www.khanacademy.org/computing/computer-science/algorithms/linear-search/a/implementing-linear-search-of-an-array
GeeksforGeeks: Binary Search: https://www.geeksforgeeks.org/binary-search/
Khan Academy: Binary Search: https://www.khanacademy.org/computing/computer-science/algorithms/binary-search/a/binary-search