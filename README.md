# AsmJIT
------

AsmJIT is a lightweight library for Assembly machine code generation with JIT (Just-in-Time Compilation) written in C++ language.

  * [Official Home Page (asmjit.com)](https://asmjit.com)
  * [Official Repository (asmjit/asmjit)](https://github.com/asmjit/asmjit)
  * [Public Chat Channel](https://app.gitter.im/#/room/#asmjit:gitter.im)
    * [Zlib `LICENSE.md`](./LICENSE.md)

See [asmjit.com](https://asmjit.com) page for more details, examples, and documentation.

## Documentation
-------------

  * [Documentation Index](https://asmjit.com/doc/index.html)
  * [Build Instructions](https://asmjit.com/doc/group__asmjit__build.html)

### Contributing
------------

  * See [`CONTRIBUTING.md`](./CONTRIBUTING.md) page for more details

## Breaking Changes
----------------

Breaking the API is sometimes inevitable, what to do?

  * See [Breaking Changes Guide](https://asmjit.com/doc/group__asmjit__breaking__changes.html), which is now part of AsmJIT's documentation

  * Checkout under the the AsmJIT `test/` directory for implementation and use-case examples or testing whether the build / API **is** brokem. The following should always work, and they should always compile:
    
    * [`asmjit_test_emitters.cpp`](./test/asmjit_test_emitters.cpp) - Tests that demonstrate the purpose of emitters
    * [`asmjit_test_assembler_x86.cpp`](./test/asmjit_test_assembler_x86.cpp) - Tests targeting AsmJIT's Assembler (x86/x64)
    * [`asmjit_test_compiler_x86.cpp`](./test/asmjit_test_compiler_x86.cpp) - Tests targeting AsmJIT's Compiler (x86/x64)
    * [`asmjit_test_instinfo.cpp`](./test/asmjit_test_instinfo.cpp) - Tests that query instruction information
    * [`asmjit_test_x86_sections.cpp`](./test/asmjit_test_x86_sections.cpp) - Multiple sections test

    * Visit our [Gitter Chat](https://app.gitter.im/#/room/#asmjit:gitter.im) if you need quick help

## Project & Directory Organization:
--------------------

  * **`/`**        - Project root
    * **`db/`**       - AsmJIT's ISA DB Instruction Set Database

    * **`src/`**      - Source code
      * **`asmjit/`** - Source code and headers (always point `include` path in here)
        * **`core/`** - Core API, backend independent except relocations
        * **`arm/`**  - ARM specific API, used only by ARM and AArch64 backends
        * **`x86/`**  - x86 specific API, used only by x86 and x64 backends
    * **`test/`**     - Unit and integration tests (don't embed in your project)
    * **`tools/`**    - Tools used for configuring, documenting, and generating files

## Ports
-----

  * [ ] 32-bit ARM / Thumb port (work in progress)
  * [ ] RISC-V port (not in progress, help welcome)

### Support
-------

  * AsmJIT project has both community and commercial support, see [AsmJIT's Support Page](https://asmjit.com/support.html)
  * You can help the development and maintenance through Petr Kobalicek's [GitHub sponsors Profile](https://github.com/sponsors/kobalicek)
  
  
##**Original repository: [https://github.com/AsmJIT/AsmJIT](https://github.com/AsmJIT/AsmJIT)**
