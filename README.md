# File Compression and Decompression

This repository contains a simple C++ program for file compression and decompression using run-length encoding (RLE). The program compresses a text file by encoding sequences of the same character with the character followed by its count and can also decompress files encoded with this method.

## Overview

- **Compression**: Reads a text file, compresses it using run-length encoding, and writes the compressed data to a new file.
- **Decompression**: Reads a compressed file and reconstructs the original text by decoding the run-length encoded data.

## Files

- `compressFile(const string &inputFile, const string &outputFile)`: Compresses the specified input file and writes the result to the output file.
- `decompressFile(const string &inputFile, const string &outputFile)`: Decompresses the specified input file and writes the result to the output file.
- `main()`: Demonstrates the usage of the compression and decompression functions.

## Requirements

- A C++ compiler that supports C++11 or later.

## Usage

1. **Prepare Your Files**

   Create a text file named `input.txt` with the content you want to compress.

2. **Compile the Code**

   Use a C++ compiler to compile the source code. For example, with `g++`, you can run:

   ```sh
   g++ -o file_compression file_compression.cpp
   ```

3. **Run the Program**

   Execute the compiled program:

   ```sh
   ./file_compression
   ```

   This will generate two files:
   - `compressed.txt`: The compressed version of `input.txt`.
   - `decompressed.txt`: The decompressed version of `compressed.txt`.

4. **Check Results**

   Verify the output files:
   - `compressed.txt` should contain the run-length encoded data.
   - `decompressed.txt` should match the original `input.txt` file.

## Example

Assume `input.txt` contains the following text:

```
aaaabbbccdaa
```

After running the program, `compressed.txt` will contain:

```
a4b3c2d2a2
```

And `decompressed.txt` will revert back to:

```
aaaabbbccdaa
```

## Troubleshooting

- Ensure that `input.txt` exists in the same directory as the executable.
- Verify file permissions if you encounter issues with opening or writing files.
Your README file looks well-organized and informative. Here’s a slightly refined version with minor improvements for clarity and completeness:

---

# File Compression and Decompression

This repository contains a simple C++ program for file compression and decompression using run-length encoding (RLE). The program compresses a text file by encoding sequences of the same character with the character followed by its count and can also decompress files encoded with this method.

## Overview

- **Compression**: Reads a text file, compresses it using run-length encoding, and writes the compressed data to a new file.
- **Decompression**: Reads a compressed file and reconstructs the original text by decoding the run-length encoded data.

## Files

- `compressFile(const string &inputFile, const string &outputFile)`: Compresses the specified input file and writes the result to the output file.
- `decompressFile(const string &inputFile, const string &outputFile)`: Decompresses the specified input file and writes the result to the output file.
- `main()`: Demonstrates the usage of the compression and decompression functions.

## Requirements

- A C++ compiler that supports C++11 or later.

## Usage

1. **Prepare Your Files**

   Create a text file named `input.txt` with the content you want to compress.

2. **Compile the Code**

   Use a C++ compiler to compile the source code. For example, with `g++`, you can run:

   ```sh
   g++ -o file_compression file_compression.cpp
   ```

3. **Run the Program**

   Execute the compiled program:

   ```sh
   ./file_compression
   ```

   This will generate two files:
   - `compressed.txt`: The compressed version of `input.txt`.
   - `decompressed.txt`: The decompressed version of `compressed.txt`.

4. **Check Results**

   Verify the output files:
   - `compressed.txt` should contain the run-length encoded data.
   - `decompressed.txt` should match the original `input.txt` file.

## Example

Assume `input.txt` contains the following text:

```
aaaabbbccdaa
```

After running the program, `compressed.txt` will contain:

```
a4b3c2d2a2
```

And `decompressed.txt` will revert back to:

```
aaaabbbccdaa
```

## Troubleshooting

- Ensure that `input.txt` exists in the same directory as the executable.
- Verify file permissions if you encounter issues with opening or writing files.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to open issues or submit pull requests for improvements and fixes.
