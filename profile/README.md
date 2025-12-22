# IT4113: Computer Organization and Architecture – Practicals 🖥️⚙️

Welcome to the official repository for IT4113: Computer Organization and Architecture practicals and assignments. This repository is maintained for uploading daily practical sessions and coursework related to the IT4113 module. All tasks are assigned during lecture hours and focus on understanding computer architecture concepts and MIPS assembly language programming using QtSpim.

## 📘 Course Module Details

- **Course Code:** IT4113
- **Course Title:** Computer Organization and Architecture
- **University:** University of Vavuniya
- **Academic Year:** 2025
- **Student ID:** 2020/ICT/108

## ⚙️ How to Use This Repository

### 1. Clone the Repository

To get started, clone this repository using Git:

```bash
git clone https://github.com/IT4113-Computer-Organization-Practicals/
```

### 2. Navigate to the Specific Folder

Once cloned, navigate to the folder for the specific practical or assignment:

```bash
cd IT4113-Computer-Organization-Practicals
```

### 3. Follow the Instructions

Each folder contains setup instructions and task details. Follow them carefully to run the assembly programs using QtSpim.

## 🗂️ Practicals

Practical sessions will be uploaded periodically. Each task will have a dedicated folder containing:

- MIPS Assembly files (`.asm` or `.s`)
- Setup instructions
- Program descriptions and objectives
- Expected outputs and test cases
- Documentation of registers and memory usage

## 💻 Requirements

Before working on the practicals, ensure you have the following tools installed:

### QtSpim (MIPS Simulator)

**QtSpim** is a graphical simulator for the MIPS processor, allowing you to write, debug, and execute MIPS assembly programs.

#### Installation:

  - Download QtSpim from [SourceForge](https://sourceforge.net/projects/spimsimulator/)
  - Run the installer and follow the installation wizard
  - Launch QtSpim from the Start menu

### Alternative MIPS Simulators

- **MARS (MIPS Assembler and Runtime Simulator):** Java-based alternative
- **SPIM:** Command-line version of the simulator

## 🧪 How to Run Assembly Programs in QtSpim

### 1. Launch QtSpim
Open QtSpim from your applications menu or desktop shortcut.

### 2. Load an Assembly File
- Go to **File → Open** or press `Ctrl+O`
- Navigate to your `.asm` file and open it
- Alternatively, go to **File → Reinitialize and Load File**

### 3. Run the Program
- Click the **Run/Continue** button (▶️) or press `F5`
- For step-by-step execution, use the **Single Step** button or press `F10`
- View output in the **Console** window
- Monitor registers in the **Registers** panel

### 4. Debug Your Code
- Set breakpoints by clicking on line numbers
- Use **Single Step** to execute one instruction at a time
- Examine register values and memory contents during execution
- Check the **Text Segment** and **Data Segment** panels

## 📚 MIPS Assembly Basics

### Program Structure

```assembly
        .data           # Data segment
msg:    .asciiz "Hello, World!\n"

        .text           # Code segment
        .globl main
main:
        li $v0, 4       # System call for print string
        la $a0, msg     # Load address of string
        syscall         # Execute system call
        
        li $v0, 10      # System call for exit
        syscall
```

### Common System Calls

| Service | Code ($v0) | Arguments | Result |
|---------|-----------|-----------|--------|
| Print Integer | 1 | $a0 = integer | - |
| Print String | 4 | $a0 = string address | - |
| Read Integer | 5 | - | $v0 = integer read |
| Read String | 8 | $a0 = buffer, $a1 = length | - |
| Exit | 10 | - | - |

## 📁 Folder Structure

```
IT4113-Computer-Organization-Practicals/
│
├── Day01/
│   ├── README.md
│   ├── program1.asm
│   └── program2.asm
│
├── Day02/
│   ├── README.md
│   └── ...
│
└── Assignments/
    ├── Assignment01/
    └── Assignment02/
```

## 🎯 Learning Objectives

Through these practicals, you will:

- Understand fundamental computer organization concepts
- Master MIPS assembly language programming
- Learn about processor architecture and instruction sets
- Implement algorithms in low-level assembly code
- Debug and optimize assembly programs
- Understand memory hierarchy and addressing modes
- Work with registers, stack, and system calls

## 📝 Notes

- Always comment your code for better understanding
- Test your programs with multiple test cases
- Save your work frequently
- Follow naming conventions for labels and variables
- Document register usage in complex programs

## 📜 License

This repository is created as part of the **IT4113: Computer Organization and Architecture** course module and is intended for educational purposes only. All content belongs to the **University of Vavuniya** and its faculty.
