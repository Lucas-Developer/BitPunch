BitPunch
========

Goal of project is to create standalone McEliece implemetation in C language.

Project is now only in *development version*.

### External dependencies:
  - there is now only dependency to openssl library, it uses hash function
  - library name: `libssl-dev`
  - see [lib/src/operations.c:28](lib/src/operations.c#L28) and [lib/src/operations.c:67](lib/src/operations.c#L67)
    - `#include <openssl/sha.h>`
    - `SHA512()`

### Build:
  - go to `cd lib` folder
  - type `make` to build static library with example of (keygen, enc, dec)
    - see [lib/src/main.c](lib/src/main.c) for details
  - see makefile help, type `make help` for further build options

### Example:
  - see [lib/src/main.c](lib/src/main.c) for example of usage keygen, encryption and decryption
