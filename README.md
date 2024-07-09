go-bitset
=========

A bit string is literally a fixed-length sequence of bits (0s and 1s) used as a compact way to represent a set of integers.

For example, the bitstring 1010 represents the set {1, 3}. The size of the string is 4 bits, and can represent a set of 4 integers.

Bit strings become efficient to use when the number of integers is large. ie. when we have a set of 1000 integers, we can represent it with:

- naively: 1000 * uint32 = 4000 bytes
- with a bitstring: 1000 bits = 125 bytes
