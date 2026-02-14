Dump OS:
1) Install the os into nspire-emu/firebird
2) Enter debugger, type "k 10000000", then "c"
3) Reset emulation
4) When progress bar is at end it will hit a breakpoint
5) In debugger type "wm os.bin 10000000 2000000"
6) OS ram will be dumped in the emulator's root folder

Trim OS Dump (ONLY TRIMMED DUMPS SHOULD BE USED FOR ANALYSIS):
1) Rename OS dump to "os.bin"
2) Copy the renamed file inside same directory of "CutOS.exe"
3) Run the program
4) Trimmed OS will be written to "cutos.bin"

When loading a dump inside IDA Pro or other software for static analysis,
remember to load the dump at offset 0x10000000.