---
title: "RAISIN - FILE COMPRESSION TOOL"
description: "A Python CLI tool designed to compress text files using a unique layered Huffman encoding algorithm, achieving a higher compression ratio than standard Huffman. | Tech Stack: Python"
#dateString: 
draft: false
tags: ["File compression", "Python", "Algorithms", "Data Structures", "CLI"]
showToc: false
weight: 110
cover:
    image: "projects/raisin/cover.jpg"
--- 
### 🔗 [Github Repository](https://github.com/NehalH/raisin)

## Description
**Raisin** is a Python-based command-line tool created to compress text files using a layered Huffman encoding algorithm. It employs a multi-tiered approach where data is successively compressed across multiple layers, achieving higher compression ratios than standard single-pass Huffman encoding while preserving complete data integrity.

## Features

- **Layered Huffman Compression**: Successively compresses text data across multi-stage Huffman trees for improved compression ratios over standard implementations.
- **Lossless Decompression**: Guarantees bit-exact reconstruction of the original text content.
- **Efficient Binary Representation**: Utilizes packed binary byte streams for compact file footprint and reduced disk overhead.
- **Intuitive CLI**: Simple command-line interface for rapid compression and decompression of files.

## Why "Raisin"?

Just like plump grapes transform into tiny raisins without losing their essential nutrition, Raisin shrinks your data while preserving every bit of real information. It's compression without compromise!

## Architecture & Modules

- **level_1**: Huffman tree generation, bit-code dictionary mapping, and encoding (`huffman_L1()`) / decoding (`decode_L1()`) at tier 1.
- **level_2**: Successive layered Huffman encoding (`huffman_L2()`) and decoding (`decode_L2()`) at tier 2.
- **pack_unpack**: Bit-packing (`pack()`) and unpacking (`unpack()`) routines translating variable-length binary strings into compact byte streams.
- **read_write**: File I/O utilities for handling raw and compressed binary archives (`write_to_compressed_file()`, `read_from_compressed_file()`).
- **manipulation**: High-level orchestration for executing layered compression (`compress()`) and decompression pipelines (`decompress()`).
- **main**: CLI entry point and argument parsing.
