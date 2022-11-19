| [Home](README.md) | [Bits & Bytes](page1.md) | [Prefixes](page2.md) | [Efficiency](page3.md) | [**Compression**](page4.md) |

# Compression

**Compression:** _reduces_ resources required to store and transmit data
- encoding information using fewer bits than the original representation
- either lossy or lossless
- **Lossless:**
    - reduces bits by identifying and eliminating statistical redundancy
    - no information is lost
    - Ex. run-length encoding is a form of lossless compression
        - Let’s say we have a string of 30 characters:
            - AAAAAAAAAAABBBBBCCCCCCCCDDDDDD
        - If each character requires 1 byte to represent it, then the string - of characters takes 30 bytes to represent it.
        - With run-length encoding we can represent the same 30 characters like this:
            - 11A5B8C6D
            - The above could be represented using 8 bytes. 1 byte for each number (quantity) and 1 byte for each letter.
        - 30 bytes of information can be represented by 8 bytes.
            - 8 bytes is 3.75 times smaller than 30 bytes so the information will be transferred 3.75 times faster over the network
- **Lossy**: reduces bits by removing unnecessary or less important information