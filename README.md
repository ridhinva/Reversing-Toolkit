# Reversing Toolkit 🔧

**3 reverse engineering & binary exploitation tools** — stack/heap exploitation, VM reversing, binary analysis.

## Tools

| Tool | Focus | Techniques |
|------|-------|------------|
| `binary_exploit.py` | Binary exploitation | Stack overflow, ROP, Shellcode, Format string |
| `heap_exploit.py` | Heap attacks | tcache, UAF, Double free, Fastbin, House of X |
| `vm_reverse.py` | VM reverse engineering | Bytecode analysis, Emulation, ISA recovery |

## Installation

```bash
git clone https://github.com/ridhinva/Reversing-Toolkit.git
cd Reversing-Toolkit
pip install pwntools unicorn capstone  # optional
```

## Usage

```bash
# Generate cyclic pattern for buffer overflow offset
python3 binary_exploit.py pattern 200

# Show ROP gadgets to search for
python3 binary_exploit.py rop

# Generate shellcode
python3 binary_exploit.py shellcode x64

# Analyze heap behavior
python3 heap_exploit.py --analyze vulnerable_binary

# Disassemble VM bytecode
python3 vm_reverse.py --disasm bytecode.bin
```

## Author

**Ridhin V A** ([@c_y_p_h3r](https://x.com/c_y_p_h3r))


## Disclaimer

For authorized security testing and educational purposes only.
