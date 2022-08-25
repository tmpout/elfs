# ELFs

This is a collection of interesting ELF files for inspiration and testing.

> :warning: **WARNING**: Interact with these files at your own risk! They may contain malicious code, and malicious properties designed to break your analysis tools.

# File List

| File | Size | Author | Note |
|------|------|--------|------|
| 0xfftactics | 128 | netspooky | Maxed out fields in a 64 bit ELF |
| base.bin | 128 | netspooky | The smallest x86_64 ELF that doesn't violate the spec. |
| bigfilesz | 197 | netspooky | An ELF with a large p_filesz and some other issues that mess up a lot of parsers |
| bye | 84 | netspooky | A golfed ELF that shuts down the computer |
| f1ac5.bin | 106 | f1ac5 | Demonstrates a program header overlay at offset 0x31 |
| fourtytwo | 114 | subvisor | Demonstrations a program header overlay at offset 0x38 |
| myCoolBinary.elf | 40077 | netspooky | Contains ASCII art in the vernaux / verneeded entry and prints when you run it |
| p82.3 | 82 | netspooky | 82 byte x86_64 ELF, requires 5 level paging to work |
| phdr.0xFFFFprg.bin | 3670080 | netspooky | This ELF has 65,535 program headers, the maximum allowed in an ELF. |
| phdr.10kprgheaders.bin | 560120 | netspooky | This ELF has 10,000 program headers. |
| phdr.73prg.bin | 4152 | netspooky | This ELF contains 73 program headers, which is the maximum number that will run on most kernels |
| ptnote.oob.bin | 176 | netspooky | Has a PT_NOTE section that past the end of the file |
| retr0id.elf.so | 170 | retr0id | A small shared object. |
| rizin_free_acab_poc.bin | 39244 | netspooky | This caused a version of rizin to free(0xacabacabacabacab) due to bad offset in dynamic section |
| rqu.so | 136 | rqu | A small shared object used in the CVE-2021-3060 POC |
| sigbusser | 130 | netspooky | Causes a bus error |
| sigtrappin | 159 | netspooky | Was a challenge to enter a chat |

# Contributing

PRs are welcome. Please update the readme with a description of the files you added. 
