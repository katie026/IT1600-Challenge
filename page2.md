| [Home](README.md) | [Bits & Bytes](page1.md) | [**Prefixes**](page2.md) | [Efficiency](page3.md) | [Compression](page4.md) |

# Prefixes
Converting Bits and Bytes
- 8 bits = 1 byte
- 1,024 bytes = kilobyte
- 1,024 kilobytes = megabyte
- 1,024 megabytes = gigabyte
- 1,024 gigabytes = terabyte
- E.g.) to convert 4 kilobytes into bits
    - first convert kilobytes to bytes (4 x 1,024)
    - then use that total (4,096) to convert to bits (8 x 4,096) to - get 32,768 bits


[common prefixes](https://en.wikipedia.org/wiki/Metric_prefix): kilo, mega, giga, tera, peta, and exa
- Ex.
    - 1 mega = 106
    - 1 tera = 1012
    - 1 mega and 1 tera have a 106 = 1,000,000 difference
    Meaning 1 terabyte (the larger prefix) is 1,000,000 megabytes
- 1 kB = 1 kilobyte = 1024 bytes
    - Why 1024 instead of 1000?
    - 1024 is a power of 2: 210
- Mega = generally 1,000,000 (a million)
    - million = 1000 times 1000 → mega = 1000 kilo =  kilo kilo
    - If 1024 = kilo → mega = kilo x kilo = 1024 x 1024 = 1,048,576
        - 1 megabyte (MB) = 1,048,576 bytes
- [Sometimes](https://en.wikipedia.org/wiki/Megabyte), 1 megabyte = 1,048,576 bytes (220 B)
    - Less common: megabyte = 1000×1024 bytes = 1,024,000 bytes
    - From an order of magnitude standpoint, they are both the same

Speed examples of 3 kilobits over 1 kilobit/sec:
1. If k = 1000 
    - 3000 bits of data → transferred over a 1000 bit/second etwork → **3 seconds**
3. If k = 1024
    - 3072 bits (3 x 1024 bits) of data → transferred over a 024 bit/- second network → **3 seconds**  (3072 / 1024 = 3)
5. If k = 1024 (data) BUT k = 1000 (bandwidth)
    - 3072 bits (3 x 1024 bits) of data → transferred over a 000 bit/- second network → **3.072 seconds** (3072 / 1000 = 3.072)
7. If k = 1000 (data) BUT k = 1024 (bandwidth)
    - 3000 bits (3 x 1000 bits) of data → transferred over a 024 bit/- second network → **2.9296875 seconds** (3000 / 1024 = 2.9296875)