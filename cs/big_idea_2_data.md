# Big Idea 2: Data (DAT)

**Exam Weight:** 17-22%

## Overview

Data is at the heart of computing. Programs take in input data, process it, and produce output. Data can be stored, copied, and transformed, but how it is represented directly determines how much meaningful information we can extract from it. A central focus of this Big Idea is the **binary number system**.

## How Computers Represent Data Internally

### Bits and Digital Representation

How does a computer store anything at all? Everything reduces to sequences of 0s and 1s.

- Data values can be stored in variables, lists, or constants
- Computers represent data digitally — everything at the lowest level is a **bit**, a binary digit: 0 or 1
- A **bit** is the smallest unit of data in a computer
- A **byte** consists of 8 bits
- Bits are grouped together to represent abstract concepts including numbers, characters, and colors
- Everything inside a computer traces back to sequences of bits

### Limits and Errors in Bit Representation

Storing values with a fixed number of bits inevitably introduces some constraints:

- Most programming languages represent integers using a fixed number of bits, which limits the range of values that can be stored
- **Overflow error**: occurs when a calculation produces a result that exceeds the maximum value representable in the allotted bits
- **Round-off error**: occurs when a result's precision exceeds what can be stored, causing a loss of accuracy
- Some real numbers cannot be represented exactly in binary (for example, 1/3, and even 0.1 as a floating-point value)
- Using a fixed number of bits simultaneously limits both the range and the precision of stored values

---

### Binary Number System

#### Core Concepts

- **Binary (base 2)** uses only two digits: 0 and 1
- **Decimal (base 10)** uses ten digits: 0 through 9
- The "base" of a number system tells you how many distinct digit symbols it uses
- Each position in binary represents a power of 2
- With n bits, you can represent **2^n** distinct values

**Binary place values:**

| Position | 7 | 6 | 5 | 4 | 3 | 2 | 1 | 0 |
|----------|---|---|---|---|---|---|---|---|
| Value    | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

**Decimal to binary (subtraction method):**
1. Find the largest power of 2 that does not exceed the target
2. Subtract it and mark that bit position as 1
3. Repeat with the remainder
4. Fill unused positions with 0

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

**Decimal to binary (repeated division):**
- Divide by 2 repeatedly, recording each remainder
- Read the remainders from bottom to top to get the binary result

**Example: Convert 157 to binary**
- 157 / 2 = 78 remainder **1** (least significant bit)
- 78 / 2 = 39 remainder **0**
- 39 / 2 = 19 remainder **1**
- 19 / 2 = 9 remainder **1**
- 9 / 2 = 4 remainder **1**
- 4 / 2 = 2 remainder **0**
- 2 / 2 = 1 remainder **0**
- 1 / 2 = 0 remainder **1** (most significant bit)
- Read from bottom to top: **10011101**

**Binary to decimal:**
- Multiply each bit by its corresponding power of 2, then sum the results

**Example: Convert 10110 to decimal**
- 1×16 + 0×8 + 1×4 + 1×2 + 0×1 = 16 + 4 + 2 = **22**

**Example: Convert 11001010 to decimal**
- 1×128 + 1×64 + 0×32 + 0×16 + 1×8 + 0×4 + 1×2 + 0×1
- = 128 + 64 + 8 + 2 = **202**

**Comparing binary numbers:**
- Compare from left (most significant bit) to right
- The first position where they differ determines which number is larger
- A number with more digits (and a leading 1) is always larger
- 1000 (8) > 0111 (7)

**How many values can n bits represent:**

| Bits | 2^n values | Unsigned integer range |
|------|-----------|------------------------|
| 1 | 2 | 0–1 |
| 2 | 4 | 0–3 |
| 3 | 8 | 0–7 |
| 4 | 16 | 0–15 |
| 8 (1 byte) | 256 | 0–255 |
| 10 | 1,024 | 0–1,023 |
| 16 | 65,536 | 0–65,535 |
| 32 | 4,294,967,296 | 0–4,294,967,295 |

---

### Data Compression

Compression lets the same information be stored or transmitted using fewer bits:

- Data compression reduces the number of bits needed for storage or transmission
- **Lossless compression**: the original data can be perfectly reconstructed (ZIP, PNG, GIF)
- **Lossy compression**: permanently removes some data to achieve a smaller file size (JPEG, MP3, MP4)
- When data integrity is critical (text files, source code, medical images), lossless is the right choice
- When some quality loss is acceptable (streaming video, music), lossy compression delivers significant size savings
- Compression ratios vary depending on the algorithm and the type of data being compressed

---

## Representing Data Beyond Numbers

### Text Representation
- **ASCII**: represents each character using 7 bits, covering 128 characters (English letters, digits, punctuation, and control characters)
- **Unicode**: supports over 100,000 characters, covering most of the world's writing systems
- Each character maps to a unique number, which is then stored in binary

### Image Representation
- Images are made up of **pixels**
- Each pixel's color can be described by RGB values (Red, Green, Blue)
- Each color channel ranges from 0–255 (8 bits), giving 24 bits per pixel — about 16.7 million possible colors
- Higher bit depth means richer color, but also larger file sizes
- Resolution (number of pixels) affects both image quality and file size

### Sound Representation
- Sound is digitized through **sampling**
- **Sample rate**: how many times per second a measurement is taken (CD quality = 44,100 Hz)
- **Bit depth**: how many bits represent each sample (affects dynamic range; CD uses 16-bit)
- Higher sample rate and greater bit depth produce better audio quality but also larger files

---

## Extracting Meaning from Data

### What Data Can Tell Us

Data is raw material — it needs to be processed before it becomes meaningful information:

- Information is the facts and patterns extracted from data
- Data gives us the opportunity to discover trends, identify relationships, and solve problems
- Processed data can reveal **correlations** — statistical relationships between variables
- **Correlation does not imply causation**
- Combining multiple data sources typically yields deeper insight than relying on any single source alone

### Interpreting Data: Metadata

- **Metadata** is data about data (examples: author, creation date, file size, GPS coordinates embedded in a photo)
- Metadata can improve data usability and manageability
- Metadata can unintentionally reveal personal or group-level information

### Challenges of Working with Large Datasets

- What you can do with data depends on the capabilities of both the user and the tools available
- **Data cleaning** is a necessary step for ensuring accuracy (removing duplicates, correcting errors, handling missing values)
- Biased, incomplete, or inaccurate data skews analysis results
- Bias does not automatically disappear just because the dataset gets larger
- Very large datasets may require parallel computing or specialized software to process
- The way data is collected, processed, and used can itself introduce bias at every stage

### Using Programs to Extract Information

- Programs can process, transform, filter, and clean data
- Tables, charts, and visualizations help surface patterns that raw numbers hide
- Filtering and cleaning data helps focus analysis on what actually matters
- Merging multiple data sources typically leads to more complete and actionable insights

---

## Key Terms

| Term | Definition |
|------|------------|
| Bit | A binary digit (0 or 1); the smallest unit of data |
| Byte | 8 bits |
| Binary (base 2) | A number system that uses only 0 and 1 |
| Decimal (base 10) | The everyday number system using digits 0–9 |
| Hexadecimal (base 16) | A number system using 0–9 and A–F; often used as a compact representation of binary |
| Overflow error | An error that occurs when a calculation exceeds the maximum value that the available bits can store |
| Round-off error | Loss of precision in numeric computation due to limited bit depth |
| Metadata | Data that describes other data |
| Pixel | The smallest addressable element in a digital image |
| RGB | Red-Green-Blue color model |
| Sampling | The process of converting an analog signal to digital by taking measurements at fixed intervals |
| Sample rate | The number of samples taken per second (unit: Hz) |
| Bit depth | The number of bits used per sample or per color channel |
| Lossless compression | A compression method that allows perfect reconstruction of the original data |
| Lossy compression | A compression method that permanently discards some data to achieve a smaller file size |
| ASCII | A 7-bit character encoding standard covering 128 characters |
| Unicode | A universal character encoding standard supporting over 100,000 characters |
| Correlation | A statistical association between two variables |
| Causation | One event directly causing another to occur |

## Common Misconceptions

1. **Binary is a code, not a number system** — Binary is genuinely a positional numeral system, just like decimal, except it uses base 2 instead of base 10.
2. **Computers "understand" decimal** — Computers operate entirely in binary internally; decimal is converted to binary on input and converted back for display.
3. **More bits means a bigger number** — More bits means a wider **representable range**. The number 5 is still 5 whether stored in 8 bits or 32 bits.
4. **0.1 + 0.2 = 0.3 in a computer** — Because of how floating-point numbers are stored, 0.1 + 0.2 may not equal exactly 0.3. This is an inherent round-off error in binary representation of certain decimals.
5. **Lossy compression can be reversed** — No. Data removed by lossy compression is gone permanently and cannot be recovered.
6. **Correlation means causation** — A correlation found in data does not mean one variable causes the other.
7. **Digital data is perfectly precise** — Digital representation is approximate. Analog signals must be sampled, and precision is bounded by bit depth.
8. **Metadata is visible** — Metadata is typically hidden and can reveal personal information without the user being aware (for example, GPS coordinates embedded in a photo).
9. **Larger datasets eliminate bias** — If the data collection method is itself biased, no amount of additional data removes that bias.

## Practice: Binary Conversion

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

### Sorting Binary Numbers (Ascending)
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

**Hex to binary:** Replace each hex digit with its 4-bit binary equivalent.
- Example: 3F = 0011 1111 = decimal 63

**Binary to hex:** Group bits from the right in sets of 4; convert each group to its hex digit.
- Example: 10011101 = 1001 1101 = 9D = decimal 157
