## **ISA DB** (Instruction Set Architechture Database)
------------------------------------------------------

This is a database of instruction sets that is used by AsmJIT to generate it's internal database and also Assembler implementations. This project started initially as `AsmDB`, but was merged to The same `AsmJIT` repo / project later in order to make the maintenance easier. The database was created in a way so that each instruction definition would only need a single line in a `*.json` data file. The data is then processed by architecture-specific data readers that make the data canonical and ready for processing.

AsmJIT's database currentyly provides the following ISA (Instruction Set Architecture's):

  * `isa_x86.json` - provides x86 instruction-set data (both 32-bit and 64-bit)
  * `isa_aarch32.json` - provides AArch32 instruction-set data (A32 / T16/ T32 encoding)
  * `isa_aarch64.json` - provides AArch64 instruction-set data (A64 encoding)
  * `isa_aarch64_sme.json` - provides AArch64 SME instruction-set data (work-in-progress)

### To Be Documented
----------------

This project will be refactored and documented in the future.

## The ISA DB's Official UN-"License" Status & Free Usage
----------------------------------------------------------

The AsmJIT's ISA database is dual-licensed under ***Zlib (AsmJIT's license)*** **and** ***Public Domain***. The database can be used by *anyone* for *any purpose* AsmJIT*_

* Read more about it in the [`./db/LICENSE.md`](./db/LICENSE.md) file and consider checking out the [unlicense.org](https://unlicense.org) organization's website for a long list of other (unrelated to this project, by widely known & popular tools including
*  `SQLite`
*  `youtube-dl`
*  `MinGW`
*  `jQuery JSON-RPC`
*  `JSched`
*  `jStorage`
*  `yt-dlp`
*  `Postgres`
*   `Bitcoin` released under this the Unlicense), further information about it.
