# Simple Shellcode Loader (Debug Harness)

A simple Windows shellcode loader harness that executes raw shellcode in memory using a suspended thread.  
It supports an optional entry-point offset and basic debugger-based controlled execution.

## ⚠️ Disclaimer
This tool is for **educational and malware analysis in controlled environments only**. Do not use on unauthorized systems.

---

## 📌 Description

Loads raw shellcode from a file into memory, allocates executable space, and executes it via a suspended thread.  
Supports an optional entry-point offset to control execution start location and waits for a debugger before running.

---

## ⚙️ Features

- Loads raw binary shellcode from file  
- Allocates executable memory using `VirtualAlloc`  
- Supports entry-point offset execution  
- Suspended thread execution (`CreateThread`)  
- Basic debugger check (`IsDebuggerPresent`)  
- Controlled execution under debugger  

---

## 🚀 Usage

```bash
shellcode_loader.exe <file> [entry_offset_hex]
