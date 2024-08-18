---
layout: page
title: AVR LCD I2C Interface
description: AVR implementation for interfacing with standard character LCD displays (16x2 or 20x4) using the I2C communication protocol.
img: assets/img/avr/thumb.png
importance: 5
category: hardware
tags : ['avr', 'i2c', 'LCD']
github: https://github.com/eshansurendra/liquid_crystal_i2c_avr
---

> For detailed documentation and source code, visit my [GitHub Repository](https://github.com/eshansurendra/liquid_crystal_i2c_avr).

### Project Overview

This project provides an AVR implementation for interfacing with standard character LCD displays (16x2 or 20x4) using the I2C communication protocol. The code is optimized for AVR microcontrollers, offering a lightweight and efficient way to control LCDs without relying on external libraries like the Arduino framework. By using I2C, you can significantly reduce the number of pins required for communication, simplifying wiring and freeing up valuable microcontroller resources.

### Features
* **I2C Communication:** Uses the AVR's Two-Wire Interface (TWI) for communication with I2C-enabled LCD modules.
* **Lightweight:** Designed to be compact and efficient, minimizing code size and resource usage.
* **Easy Integration:** Provides a simple API for sending commands and data to the LCD.
* **4-Bit Mode:** Supports the more efficient 4-bit communication mode for reduced pin usage.

### Key Functions

*   **`lcd_command(uint8_t command)`**: Sends a command to the LCD module.
*   **`lcd_data(uint8_t data)`**: Sends a character to be displayed on the LCD.
*   **`lcd_set_cursor(uint8_t row, uint8_t col)`**: Sets the cursor position on the LCD.
*   **`lcd_print(char* str)`**: Prints a null-terminated string to the LCD.

**Common LCD Operations**

Here are examples of common LCD operations using the provided implementation:

1.  **Clear the Display**

    ```c
    lcd_command(0x01); // Send the clear display command (0x01)
    ```

2.  **Set Cursor Position**

    To set the cursor to a specific row and column:

    ```c
    lcd_set_cursor(0, 2);  // Set cursor to row 0, column 2
    lcd_set_cursor(1, 5);  // Set cursor to row 1, column 5
    ```

3.  **Print a String**

    ```c
    lcd_print("Hello World!"); // Print "Hello World!" at the current cursor position
    ```
