# Gameboy-logs
Emulation logs of common beginner ROMs for the Gameboy.
Currently contains a log of the boot ROM (DMG) as well as all of Blargg's ROMs

All these logs were generated with my own emulator which passes Blargg's CPU tests.

For the convenience of anyone who uses them, LY (MMIO register at 0xFF44) is stubbed to 0x90 permanently.

If you have any suggestions contact me on Discord: guccirodakino#1457

Or on Nintendo Switch Online: SW-8356-6970-6111

**Note**: All logs are zipped. The Blargg10 and Blargg11 one had to be zipped **twice** cause they're too :beeg:

**Side Note**: The bootrom log has one of the individual Blargg CPU tests loaded into memory, which is important when the bootrom computes the cart checksum. To ensure a matching log, load one of the Blargg 1-11 cpu_instrs ROMs (they all have the same checksum). If you load in any other ROM, the checksum will differ, so the log will also differ slightly (Checksum calculation happens at the end of the bootrom, starting from PC = 0x00F4)

Format: [registers] (mem[pc] mem[pc+1] mem[pc+2] mem[pc+3])
  
I log the state of the CPU BEFORE every instruction
  
