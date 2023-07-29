---
title: "RAISIN - FILE COMPRESSION ALGORITHM/TOOL"
description: "Raisin is a command-line tool designed to compress text files using a unique layered Huffman encoding algorithm."
#dateString: Jan 2021 - May 2021
draft: false
tags: ["File compression","Python", "File Structures"]
showToc: false
weight: 110
cover:
    image: "projects/raisin/cover.jpg"
--- 
### 🔗 [Github Repository](https://github.com/NehalH/raisin)

## Description
Raisin is a command-line tool designed to compress text files using layered Huffman encoding techniques. It employs a layered approach, where the data is successively compressed at each layer, resulting in further reduction in size. Python is used as the programming language for the backend implementation.

## Features

- Compresses text files using layered Huffman encoding.
- Reduces the size of data while retaining the original content.
- Utilizes a binary string representation for efficient compression.
- Easy to use as a command-line tool.

### Modules/Functions:

- **level_1**: Contains functions for Huffman encoding (`huffman_L1()`) and decoding (`decode_L1()`) at level 1.
- **level_2**: Contains functions for Huffman encoding (`huffman_L2()`) and decoding (`decode_L2()`) at level 2.
- **pack_unpack**: Contains functions for packing (`pack()`) and unpacking (`unpack()`) data for compression and decompression.
- **read_write**: Contains functions for writing the compressed data to a file (`write_to_compressed_file()`), reading from a compressed file (`read_from_compressed_file()`), reading from a regular file (`read_from_file()`), and writing to a regular file (`write_to_file()`).
- **manipulation**: Contains the main compression (`compress()`) and decompression (`decompress()`) functions, which utilize the functions from other modules to perform the necessary operations.
- **main**: Contains the main function (`main()`) that serves as the entry point for the program.

## Why "Raisin"?

Wondering why this compression tool is named "Raisin" ?

Just like plump grapes transform into tiny raisins without loosing their nutrition, Raisin shrinks your data while preserving the real information. It's compression without compromise!

So, Raisin takes your files, gives them a little squeeze, and voilà! They become compact, travel-friendly, and ready to be stored or transmitted with ease.

Next time you use Raisin, remember the grape-to-raisin transformation. It's a small change that makes a big difference!

Happy compressing, and raisin up your data game! 🍇✨

