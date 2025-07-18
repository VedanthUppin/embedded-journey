# Header Guards vs `#pragma once`

Tested different methods of preventing double inclusion of header files.

### What I Did
- Created a `header.h` with a struct.
- Included it twice from another header.
- Observed redefinition error.
- Fixed it using:
  - `#ifndef/#define/#endif`
  - `#pragma once`

### What I Learned
- Header guards are portable and reliable.
- `#pragma once` is cleaner but compiler-specific (works in GCC, Clang).
