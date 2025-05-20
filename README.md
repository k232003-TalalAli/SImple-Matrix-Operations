# Matrix Operations in Assembly Language

This project implements basic matrix operations in **x86 Assembly Language** using the `Irvine32` library. It was developed as a course project for *Computer Organization and Assembly Language*.

---

## 📌 Features

The program allows users to perform the following operations on two matrices:

1. **Transpose Matrix 1**  
2. **Add Matrix 1 and Matrix 2**  
3. **Subtract Matrix 2 from Matrix 1**  
4. **Multiply Matrix 1 and Matrix 2**
5. **Divide Matrix 1 and Matrix 2**

It also includes:

- Input validation for dimension compatibility  
- Formatted matrix display with spacing  
- Support for matrix elements stored as signed integers  

An **additional section** handles **fractional matrix division using structures**, including:

- Custom fraction struct (`Array_element`)  
- Division and simplification of rational numbers  
- Sign handling and formatting  

---

## 🛠️ Technologies

- **Assembly Language (x86)**  
- **Irvine32 Library** (required for input/output functions)  
- Assembler: MASM (Microsoft Macro Assembler)  

---

### Main Matrix Program

- Takes dimensions and inputs for two matrices  
- Displays a menu for operations  
- Validates dimensions and performs selected operation  
- Supports dynamic sizes (up to 10x10 by default)

### Rational Number Matrix Division

- Uses custom `Array_element` structure to represent fractions  
- Performs division with simplification  
- Displays fractions cleanly with `/` separator  

---

## 📋 How to Run

1. **Requirements**
   - Windows OS  
   - MASM assembler  
   - `Irvine32.inc`, `Irvine32.lib`, and required `.obj` files  

2. **Compile and Link**

   ```bash
   ml /c /coff main.asm
   link /subsystem:console main.obj Irvine32.lib
   ```

3. **Run the Program**

   - Follow the prompts to input matrix dimensions and elements  
   - Choose an operation from the displayed menu  

---

## 👨‍💻 Authors

- **Talal Ali**  
- **Daniyal Ahmed**  
- **Muhammad Hammad**

  ---

## 📌 Notes

- This project focuses on learning low-level memory manipulation and logic implementation without high-level abstractions.  
- Fraction handling in matrix division is a bonus implementation to simulate rational arithmetic in assembly.
