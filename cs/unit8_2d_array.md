# Unit 8: 2D Array

**Exam Weight:** 7.5-10% | **Suggested Time:** ~6-8 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 8.1: 2D Arrays

This section covers how to use a two-dimensional array to represent a collection of related primitive values or objects.

- A 2D array is essentially an array of arrays (organized as rows and columns)
- Declaration syntax: `type[][] name;`
- Creation syntax: `int[][] grid = new int[rows][cols];`
- Initializer list: `int[][] grid = {{1, 2}, {3, 4}, {5, 6}};`
- Accessing elements: `grid[row][col]`
- Number of rows: `grid.length`
- Number of columns in row r: `grid[r].length`
- In Java each row can have a different length (jagged array), but AP exams only cover rectangular arrays
- Default values are the same as for one-dimensional arrays

### Topic 8.2: Traversing 2D Arrays

This section covers how to visit every element in a two-dimensional array.

- **Row-major order:** outer loop over rows, inner loop over columns (most common)
- **Column-major order:** outer loop over columns, inner loop over rows
- The enhanced for loop can also traverse 2D arrays (the outer loop yields each row as a 1D array)
- A complete traversal requires nested loops
- Total elements = number of rows × number of columns

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| 2D array | An array whose elements are themselves arrays |
| Row | A horizontal group of elements (first index) |
| Column | A vertical group of elements (second index) |
| Row-major order | Traversal that goes left to right across each row, top to bottom |
| Column-major order | Traversal that goes top to bottom down each column, left to right |
| Rectangular array | A 2D array where every row has the same number of columns |
| Jagged array | A 2D array where rows can have different numbers of columns |

## Common Misconceptions

1. **`grid.length` is the total number of elements** — It is not. It returns only the number of rows. The total element count is `grid.length * grid[0].length`.
2. **Confusing row and column indices** — In `grid[row][col]`, the first index is the row and the second is the column. Think of it as [y][x], not [x][y].
3. **Using `grid.length` to get the column count** — Use `grid[0].length` (or `grid[r].length` for a specific row) to get the number of columns.
4. **Off-by-one in nested loops** — Both loop levels must use `<` with `.length`, not `<=`.
5. **Enhanced for loop over a 2D array** — The outer enhanced for loop yields a 1D array representing one row, not an individual element. A second inner enhanced for loop is needed to access individual values.
6. **Assuming the array is square** — Row count and column count can differ. Use `grid.length` for rows and `grid[0].length` for columns rather than assuming they are equal.

## Code Patterns and Examples

### 2D Array Creation
```java
// Declaration and creation
int[][] grid = new int[3][4];  // 3 rows, 4 columns, all zeros

// Initializer list
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

// Access
int val = matrix[1][2];  // 6 (row 1, col 2)
matrix[0][0] = 10;       // set top-left to 10

// Dimensions
int rows = matrix.length;        // 3
int cols = matrix[0].length;     // 3
```

### Row-Major Traversal
```java
int[][] grid = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};

// Row-major order (most common)
for (int row = 0; row < grid.length; row++) {
    for (int col = 0; col < grid[row].length; col++) {
        System.out.print(grid[row][col] + " ");
    }
    System.out.println();
}
// Output:
// 1 2 3
// 4 5 6
// 7 8 9
```

### Column-Major Traversal
```java
// Column-major order
for (int col = 0; col < grid[0].length; col++) {
    for (int row = 0; row < grid.length; row++) {
        System.out.print(grid[row][col] + " ");
    }
    System.out.println();
}
// Output:
// 1 4 7
// 2 5 8
// 3 6 9
```

### Enhanced For Loop with 2D Array
```java
// Enhanced for loop
for (int[] row : grid) {        // each row is a 1D array
    for (int val : row) {       // each val is an element
        System.out.print(val + " ");
    }
    System.out.println();
}
```

### Standard Algorithms

```java
// Sum all elements
int total = 0;
for (int[] row : grid) {
    for (int val : row) {
        total += val;
    }
}

// Find maximum
int max = grid[0][0];
for (int row = 0; row < grid.length; row++) {
    for (int col = 0; col < grid[row].length; col++) {
        if (grid[row][col] > max) {
            max = grid[row][col];
        }
    }
}

// Count occurrences of a value
int count = 0;
int target = 5;
for (int[] row : grid) {
    for (int val : row) {
        if (val == target) {
            count++;
        }
    }
}

// Sum each row
for (int row = 0; row < grid.length; row++) {
    int rowSum = 0;
    for (int col = 0; col < grid[row].length; col++) {
        rowSum += grid[row][col];
    }
    System.out.println("Row " + row + " sum: " + rowSum);
}

// Sum each column
for (int col = 0; col < grid[0].length; col++) {
    int colSum = 0;
    for (int row = 0; row < grid.length; row++) {
        colSum += grid[row][col];
    }
    System.out.println("Col " + col + " sum: " + colSum);
}
```

### Diagonal Traversal (Square Matrix)
```java
// Main diagonal (top-left to bottom-right)
for (int i = 0; i < grid.length; i++) {
    System.out.print(grid[i][i] + " ");
}

// Anti-diagonal (top-right to bottom-left)
int n = grid.length;
for (int i = 0; i < n; i++) {
    System.out.print(grid[i][n - 1 - i] + " ");
}
```

### Boundary Traversal
```java
// Check/process only edge elements
for (int row = 0; row < grid.length; row++) {
    for (int col = 0; col < grid[row].length; col++) {
        if (row == 0 || row == grid.length - 1 ||
            col == 0 || col == grid[row].length - 1) {
            // This is a boundary element
            System.out.print(grid[row][col] + " ");
        }
    }
}
```

### FRQ Pattern: Image Processing
```java
// Simulate pixel manipulation (common FRQ theme)
int[][] pixels = new int[100][100];

// Set all pixels to a value
for (int r = 0; r < pixels.length; r++) {
    for (int c = 0; c < pixels[r].length; c++) {
        pixels[r][c] = 255;
    }
}

// Mirror horizontally
for (int r = 0; r < pixels.length; r++) {
    for (int c = 0; c < pixels[r].length / 2; c++) {
        int temp = pixels[r][c];
        pixels[r][c] = pixels[r][pixels[r].length - 1 - c];
        pixels[r][pixels[r].length - 1 - c] = temp;
    }
}
```
