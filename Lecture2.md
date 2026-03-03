Data structures

## Dynamic sequest operations

### Static Arrays

- Array access is constant time because data is stored in contigous
memory

so array[i] = memory[address(array)+i]

O(1) per get per set
O(n) per build per iteration

Memory allocation model: allocate a size of an array n take O(n)
Space = O(n)

Characteristics
- Insert and delete anywhere cost Theta(n) time
-- Because if we are near the front, we need shiffting
-- To insert at the end, we have to do allocation, by copying from
an array of n to an array of n+1

Dynamic sequences

### Linked Lists

Solves the insertion / deletion problem encountered
in arrays

Characteristics
- Insertion and delete first cost O(1) time
- Get and set at need Theta (i) time, in worst case its Theta (n)

### Dynamic arrays

- Have no enforcing of the size of items
Add to the end takes constant time (O(1)) unless n == size
Size should always be more than n unless space is depleted

If n == size, allocate a new array of constant factor larger 2.Size