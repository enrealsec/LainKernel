# LainKernel

![Language](https://img.shields.io/badge/language-C-blue.svg)
![Architecture](https://img.shields.io/badge/arch-x86-orange.svg)
![License](https://img.shields.io/badge/license-Educational-green.svg)
![Status](https://img.shields.io/badge/status-In%20Development-yellow.svg)

A secure, educational operating system kernel written in C for x86 architecture.

> 🎯 **Educational Project**: This kernel is designed for learning OS development concepts, security features, and low-level programming.

## 📁 Project Structure

```
project/
├── src/                    # Source code
│   ├── kernel/            # Core kernel
│   ├── mm/                # Memory management
│   ├── arch/x86/          # Architecture-specific code
│   ├── interrupts/        # Interrupt handling
│   ├── drivers/           # Hardware drivers
│   ├── security/          # Security features
│   ├── process/           # Process management
│   ├── lib/               # Standard library
│   └── shell/             # Shell interface
├── include/kernel/        # Public headers
├── build/                 # Build artifacts
├── iso/boot/grub/         # Bootloader configuration
├── docs/                  # Documentation
└── scripts/               # Build and utility scripts
```

## 🚀 Quick Start

### Prerequisites
- GCC cross-compiler (i686-elf-gcc)
- NASM assembler
- GRUB bootloader
- QEMU emulator (for testing)

### Build

```bash
make clean
make
```

### Run

```bash
make run
```

## 📚 Documentation

- [README](docs/README.md) - Full documentation
- [Security Enhancements](docs/SECURITY_ENHANCEMENTS.md) - Security features and roadmap
- [Suggestions](docs/SUGGESTIONS.md) - Future improvements
- [Reorganization Guide](docs/REORGANIZATION.md) - Project structure details

## 🔒 Security Features

- Ring-based protection (Ring 0/3)
- Memory isolation with paging
- Cryptographically secure random number generator (CSPRNG)
- Stack canaries
- Input validation
- Audit logging
- Rate limiting

## 🛠️ Components

### Core (`src/kernel/`)
- Kernel initialization
- GDT/IDT setup
- System panic handler

### Memory Management (`src/mm/`)
- Physical memory manager
- Virtual memory (paging)
- Kernel heap allocator

### Drivers (`src/drivers/`)
- VGA text mode driver
- PS/2 keyboard driver

### Security (`src/security/`)
- Security validation
- CSPRNG (Xorshift128+)
- Audit logging system

### Process Management (`src/process/`)
- Process control blocks
- Round-robin scheduler
- System call interface

## 📝 License

Educational project - feel free to learn from and modify.

## 👤 Author

Enreal

## 🙏 Acknowledgments

- OSDev Wiki
- Intel Software Developer Manuals
- Linux kernel source code
