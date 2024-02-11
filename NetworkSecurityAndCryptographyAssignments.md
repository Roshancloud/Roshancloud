> Assignments with W are written assignments to be written by hand
> Assignments with C are to be coded assignments 

## W-1 Transport Layer Protocols (29/01/24)
- Study various protocols in the Transport Layer (4th in OSI 2nd in TCP/IP) 
- Headers format for various protocols (for better understanding)
- What is ICMP why is it used ?

## C-1 XOR Encryption Techniques (29/01/24)
### Technique 1
- Choose a prime Number b/w 64 and 128 (1 byte uint with MSB 0 and 2nd MSB 1) and use it XOR with each char in a INPUT text file and OUTPUT a binary file. (Also to implement the decryption of the bin to text again).
- Create a primarity.h for generating the prime numbers for the above code specifing an input and output range which keeps on generating the prime numbers until the range is exhausted 

### Technique 2
- Take 4 similar prime numbers and use them to repeatedly encrypt the txt chars using the order of the 4 prime numbers (Advanced : Implement a permutation logic in the order of the prime numbers so that every time the binary file changes even for the same INPUT txt !!)

### Technique 3
- Take 4 chars at a time consider them a block use a very huge uint32 to XOR the entire block at a time handle the backward edge case with 0 padding

### Technique 4 
- Take 8 chars at a time consider them a block use a very huge uint64 to XOR the entire block at a time handle the backward edge case with 0 padding


> Parameters of evaluation 
> 1. Program code should be as small as possible 
> 2. Command line interface
> 3. No limitation on the size of input file other than the OS limitations
> 4. Analysis of algo (for a given n characters how many XOR operations are used)

