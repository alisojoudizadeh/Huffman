# Huffman Coding by Ali Sojoudizadeh

This Python program implements Huffman coding, a compression algorithm that assigns variable-length codes to input characters based on their frequencies. Huffman coding is widely used in data compression applications.

## Overview

The program includes the following components:

- `Node` class: Represents a node in the Huffman tree. Each node has a probability, a symbol, and pointers to the left and right children.

- `Calculate_Codes` function: Recursively calculates Huffman codes for each symbol in the tree.

- `Calculate_Probability` function: Computes the frequency of each symbol in the input data.

- `Output_Encoded` function: Generates the encoded output based on the calculated Huffman codes.

- `Total_Gain` function: Calculates the space usage before and after compression in bits.

- `Huffman_Encoding` function: Creates a Huffman tree and computes the encoded output.

- `Huffman_Decoding` function: Decodes the encoded data using the Huffman tree.

## How to Use

1. **Run the Program:**
   ```bash
   python huffman_coding.py
   ```

2. **Input Data:**
   Modify the `data` variable with the desired input string.

3. **Output:**
   The program will display the original data, the encoded output, and the decoded output. Additionally, it will print the space usage before and after compression.

## Example

```python
data = "Ostad DOOOOOset DAREIM"
print("Original Data:", data)

encoding, tree = Huffman_Encoding(data)
print("Encoded Output:", encoding)

decoded_output = Huffman_Decoding(encoding, tree)
print("Decoded Output:", decoded_output)
```

## Notes

- The program is case-sensitive, treating uppercase and lowercase characters as distinct symbols.

- The output includes information about the symbols, their probabilities, and the Huffman codes assigned to each symbol.

Feel free to experiment with different input data to observe the compression achieved by Huffman coding.
