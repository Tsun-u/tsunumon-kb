# Big Idea 2: Data (DAT)

**Exam Weight:** 17-22%

## Overview

Data is central to computing. Programs receive input data, process it, and produce output. Data can be stored, copied, and manipulated, but the way data is represented affects the quality of information and knowledge that can be derived from it. This Big Idea includes the critically important topic of **Binary Numbers**.

## Enduring Understandings and Learning Objectives

### DAT-1: The way a computer represents data internally is different from the way the data is interpreted and displayed for the user

#### DAT-1.A: Explain how data can be represented using bits
- **Essential Knowledge:**
  - Data values can be stored in variables, lists of items, or standalone constants
  - Computing devices represent data digitally, meaning that the lowest-level components of any value are **bits** (binary digits: 0 or 1)
  - A **bit** is the smallest unit of data in computing
  - A **byte** is 8 bits
  - Bits are grouped to represent abstractions including numbers, characters, and colors
  - Everything in a computer is ultimately represented as sequences of bits

#### DAT-1.B: Explain the consequences of using bits to represent data
- **Essential Knowledge:**
  - In many programming languages, integers are represented by a fixed number of bits, which limits the range of values
  - **Overflow errors** occur when a calculated value exceeds the range that can be represented
  - **Round-off errors** occur when a calculated result is stored with less precision than the actual value
  - Some real numbers cannot be exactly represented in binary (e.g., 1/3, or even 0.1 in floating-point)
  - Using a fixed number of bits constrains both range and precision

#### DAT-1.C: For binary numbers: Calculate the binary (base 2) equivalent of a positive integer (base 10) and vice versa. Compare and order binary numbers.
- **Essential Knowledge:**
  - **Binary (base 2)** uses only digits 0 and 1
  - **Decimal (base 10)** uses digits 0-9
  - Number bases describe the number of unique digits used to represent numbers
  - Each position in binary represents a power of 2
  - The number of unique values representable with n bits is **2^n**

**Binary Place Values:**

| Position | 7 | 6 | 5 | 4 | 3 | 2 | 1 | 0 |
|----------|---|---|---|---|---|---|---|---|
| Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

**Decimal to Binary Conversion (Subtraction Method):**
1. Find the largest power of 2 that is less than or equal to the decimal number
2. Subtract it and mark that bit position as 1
3. Repeat with the remainder
4. All unused positions are 0

**Example: Convert 157 to binary**
- 157 >= 128 (2^7) → subtract: 157 - 128 = 29 → bit 7 = **1**
- 29 < 64 (2^6) → bit 6 = **0**
- 29 < 32 (2^5) → bit 5 = **0**
- 29 >= 16 (2^4) → subtract: 29 - 16 = 13 → bit 4 = **1**
- 13 >= 8 (2^3) → subtract: 13 - 8 = 5 → bit 3 = **1**
- 5 >= 4 (2^2) → subtract: 5 - 4 = 1 → bit 2 = **1**
- 1 < 2 (2^1) → bit 1 = **0**
- 1 >= 1 (2^0) → subtract: 1 - 1 = 0 → bit 0 = **1**
- Result: **10011101**

**Decimal to Binary Conversion (Repeated Division Method):**
- Divide by 2 repeatedly, recording the remainder at each step
- Read remainders from bottom to top

**Example: Convert 157 to binary**
- 157 / 2 = 78 remainder **1** (rightmost/least significant bit)
- 78 / 2 = 39 remainder **0**
- 39 / 2 = 19 remainder **1**
- 19 / 2 = 9 remainder **1**
- 9 / 2 = 4 remainder **1**
- 4 / 2 = 2 remainder **0**
- 2 / 2 = 1 remainder **0**
- 1 / 2 = 0 remainder **1** (leftmost/most significant bit)
- Read bottom to top: **10011101**

**Binary to Decimal Conversion:**
- Multiply each bit by its place value (power of 2) and sum all products

**Example: Convert 10110 to decimal**
- 1×16 + 0×8 + 1×4 + 1×2 + 0×1 = 16 + 4 + 2 = **22**

**Example: Convert 11001010 to decimal**
- 1×128 + 1×64 + 0×32 + 0×16 + 1×8 + 0×4 + 1×2 + 0×1
- = 128 + 64 + 8 + 2 = **202**

**Comparing Binary Numbers:**
- Compare from left (most significant bit) to right
- The first position where bits differ determines which is larger
- A number with more digits (and a leading 1) is always larger
- 1000 (8) > 0111 (7)

**Number of values representable with n bits:**

| n bits | 2^n values | Range (unsigned) |
|--------|-----------|-----------------|
| 1 | 2 | 0-1 |
| 2 | 4 | 0-3 |
| 3 | 8 | 0-7 |
| 4 | 16 | 0-15 |
| 8 (1 byte) | 256 | 0-255 |
| 10 | 1,024 | 0-1,023 |
| 16 | 65,536 | 0-65,535 |
| 32 | 4,294,967,296 | 0-4,294,967,295 |

#### DAT-1.D: Compare data compression algorithms to determine which is best in a particular context
- **Essential Knowledge:**
  - Data compression reduces the number of bits needed to represent data
  - **Lossless compression:** All original data can be perfectly reconstructed (ZIP, PNG, GIF)
  - **Lossy compression:** Some data is permanently removed to achieve smaller sizes (JPEG, MP3, MP4)
  - Lossless is preferred when data integrity is critical (text, code, medical images)
  - Lossy is preferred when some quality loss is acceptable for smaller files (streaming video, music)
  - The amount of size reduction varies by algorithm and data type

## Data Representation Beyond Numbers

### Text Representation
- **ASCII:** 7 bits per character, 128 characters total (letters, digits, punctuation, control characters)
- **Unicode:** Supports 100,000+ characters from most of the world's writing systems
- Each character maps to a unique number, which is stored in binary

### Image Representation
- Images are composed of **pixels** (picture elements)
- Each pixel's color can be represented by RGB values (Red, Green, Blue)
- Each color channel: 0-255 (8 bits), total 24 bits per pixel = 16.7 million colors
- Higher bit depth = more colors = larger file size
- Resolution (number of pixels) affects image quality and file size

### Sound Representation
- Sound is digitized by **sampling** at regular intervals
- **Sample rate:** How many times per second the sound is measured (e.g., 44,100 Hz for CD quality)
- **Bit depth:** Number of bits per sample (affects dynamic range, e.g., 16-bit for CD)
- Higher sample rate and bit depth = higher quality = larger file size

---

### DAT-2: Programs can be used to process data, which allows users to discover information and create new knowledge

#### DAT-2.A: Describe what information can be extracted from data
- **Essential Knowledge:**
  - Information is the collection of facts and patterns extracted from data
  - Data provide opportunities for identifying trends, making connections, and addressing problems
  - Digitally processed data may show correlation between variables
  - **Correlation does NOT necessarily indicate causation**
  - Often, combining data from different sources provides more insight than a single source

#### DAT-2.B: Describe what information can be extracted from metadata
- **Essential Knowledge:**
  - **Metadata** is data about data (e.g., author, date created, file size, GPS coordinates in photos)
  - Metadata can increase the effective use of data or collections of data
  - Metadata can reveal information about individuals or groups that was not intended to be shared
  - Changes and calculations performed on large data sets are more practical using programs than by hand

#### DAT-2.C: Identify the challenges associated with processing data
- **Essential Knowledge:**
  - The ability to process data depends on the capabilities of the users and their tools
  - Cleaning data is needed to ensure accuracy (removing duplicates, correcting errors, handling missing values)
  - Problems of bias, incomplete data, or inaccurate data can affect results
  - Bias is NOT eliminated just by using large data sets
  - Large data sets may require parallel computing or specialized software
  - The way data is collected, processed, and used can introduce bias

#### DAT-2.D: Extract information from data using a program
- **Essential Knowledge:**
  - Programs can be used to process, transform, filter, and clean data
  - Tables, charts, graphs, and other visualizations help identify patterns
  - Filtering and cleaning data helps identify relevant information
  - Combining data from different sources can provide additional insight

#### DAT-2.E: Explain how programs can be used to gain insight and knowledge from data
- **Essential Knowledge:**
  - Programs are used in iterative and interactive ways to process information
  - Insight and knowledge can be obtained from translating and transforming digitally represented information
  - Patterns and trends in data can be identified and used to make predictions
  - Programmers can use programs to filter and clean data; clean data provides more accurate results

## Key Concepts and Terminology

| Term | Definition |
|------|-----------|
| Bit | Binary digit (0 or 1); smallest unit of data |
| Byte | 8 bits |
| Binary (base 2) | Number system using only 0 and 1 |
| Decimal (base 10) | Standard number system using 0-9 |
| Hexadecimal (base 16) | Number system using 0-9 and A-F; shorthand for binary |
| Overflow error | When a value exceeds the maximum representable value |
| Round-off error | Loss of precision in numeric calculations |
| Metadata | Data about data |
| Pixel | Smallest addressable element in a digital image |
| RGB | Red-Green-Blue color model |
| Sampling | Converting analog signals to digital at regular intervals |
| Sample rate | Number of samples per second (Hz) |
| Bit depth | Number of bits per sample/channel |
| Lossless compression | Compression without data loss; fully reversible |
| Lossy compression | Compression with permanent data loss; not reversible |
| ASCII | 7-bit character encoding standard (128 characters) |
| Unicode | Universal character encoding standard (100K+ characters) |
| Correlation | Statistical relationship between variables |
| Causation | One event directly causing another |

## Common Misconceptions

1. **Binary is a code, not a number system** - Binary IS a positional number system, just like decimal. It's base 2 instead of base 10.
2. **Computers "understand" decimal** - Computers only work in binary internally. Decimal is converted to binary for processing and back for display.
3. **More bits always means a bigger number** - More bits means a wider RANGE of representable values. The number 5 is 5 regardless of whether stored in 8 or 32 bits.
4. **0.1 + 0.2 = 0.3 in a computer** - Due to floating-point representation, 0.1 + 0.2 may not exactly equal 0.3. This is a round-off error inherent to binary representation of certain decimals.
5. **Lossy compression can be reversed** - No! Once data is removed by lossy compression, it cannot be recovered.
6. **Correlation implies causation** - A correlation found in data does NOT necessarily mean one variable causes the other.
7. **Digital data is perfectly accurate** - Digital representations are approximations. Analog signals must be sampled, and precision is limited by bit depth.
8. **Metadata is always visible** - Metadata is often hidden and can reveal information people don't realize they're sharing (e.g., GPS coordinates in photos).
9. **Bigger data sets eliminate bias** - Bias can persist in large data sets if the data collection method itself is biased.

## Practice Problems: Binary Conversions

### Decimal to Binary
| Decimal | Binary |
|---------|--------|
| 0 | 0 |
| 1 | 1 |
| 5 | 101 |
| 10 | 1010 |
| 15 | 1111 |
| 25 | 11001 |
| 42 | 101010 |
| 100 | 1100100 |
| 127 | 1111111 |
| 128 | 10000000 |
| 200 | 11001000 |
| 255 | 11111111 |
| 256 | 100000000 |

### Binary to Decimal
| Binary | Calculation | Decimal |
|--------|-------------|---------|
| 1011 | 8+0+2+1 | 11 |
| 11100 | 16+8+4+0+0 | 28 |
| 101101 | 32+0+8+4+0+1 | 45 |
| 1000000 | 64 | 64 |
| 11111111 | 128+64+32+16+8+4+2+1 | 255 |

### Binary Ordering (smallest to largest)
Given: 1100, 101, 10001, 1010, 11111
- 101 = 5
- 1010 = 10
- 1100 = 12
- 10001 = 17
- 11111 = 31

### Hexadecimal Quick Reference

| Hex | Binary | Decimal |
|-----|--------|---------|
| 0 | 0000 | 0 |
| 1 | 0001 | 1 |
| 2 | 0010 | 2 |
| 3 | 0011 | 3 |
| 4 | 0100 | 4 |
| 5 | 0101 | 5 |
| 6 | 0110 | 6 |
| 7 | 0111 | 7 |
| 8 | 1000 | 8 |
| 9 | 1001 | 9 |
| A | 1010 | 10 |
| B | 1011 | 11 |
| C | 1100 | 12 |
| D | 1101 | 13 |
| E | 1110 | 14 |
| F | 1111 | 15 |

**Hex to Binary:** Replace each hex digit with its 4-bit binary equivalent.
- Example: 3F = 0011 1111 = 63 in decimal

**Binary to Hex:** Group binary digits into groups of 4 (from the right), convert each group.
- Example: 10011101 = 1001 1101 = 9D = 157 in decimal
