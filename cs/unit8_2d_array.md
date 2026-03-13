# Unit 8: 2D Array

**Exam Weight:** 7.5-10% | **Suggested Time:** ~6-8 class periods
**2025-26 Revision:** Merged into new Unit 4 "Data Collections" (30-40% of exam)

## Topics

### Topic 8.1: 2D Arrays
- **Learning Objective (VAR-2.N):** Represent collections of related primitive or object data using 2D arrays
- **Essential Knowledge:**
  - 2D array is an array of arrays (rows and columns)
  - Declaration: `type[][] name;`
  - Creation: `int[][] grid = new int[rows][cols];`
  - Initializer: `int[][] grid = {{1, 2}, {3, 4}, {5, 6}};`
  - Access: `grid[row][col]`
  - Number of rows: `grid.length`
  - Number of columns in row r: `grid[r].length`
  - Rows can have different lengths (jagged arrays), but AP exam uses rectangular arrays
  - Default values same as 1D arrays

### Topic 8.2: Traversing 2D Arrays
- **Learning Objective (CON-2.N):** Traverse elements in a 2D array
- **Essential Knowledge:**
  - **Row-major order:** Outer loop iterates rows, inner loop iterates columns (most common)
  - **Column-major order:** Outer loop iterates columns, inner loop iterates rows
  - Enhanced for loop can traverse 2D arrays (outer loop gives each row as a 1D array)
  - Nested loops required for full traversal
  - Total elements = rows x columns

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| 2D array | An array where each element is itself an array |
| Row | A horizontal line of elements (first index) |
| Column | A vertical line of elements (second index) |
| Row-major order | Traversing left to right, top to bottom |
| Column-major order | Traversing top to bottom, left to right |
| Rectangular array | All rows have the same number of columns |
| Jagged array | Rows can have different numbers of columns |

## Common Misconceptions

1. **`grid.length` gives total elements** - No! It gives the number of ROWS. Total elements = `grid.length * grid[0].length`.
2. **Confusing row and column indices** - `grid[row][col]` - first index is row, second is column. Think [y][x], not [x][y].
3. **Using `grid.length` for columns** - Must use `grid[0].length` (or `grid[r].length` for row r) for the number of columns.
4. **Off-by-one with nested loops** - Both loops must use `<` with `.length`, not `<=`.
5. **Enhanced for loop with 2D arrays** - The outer enhanced for gives 1D arrays (rows), not individual elements. Need a nested enhanced for for individual elements.
6. **Assuming square arrays** - Rows and columns can have different counts. Always use `grid.length` for rows and `grid[0].length` for columns separately.

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
