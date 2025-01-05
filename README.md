# Simple Clock Program

This is a basic C++ program that takes user input for hours, minutes, and seconds, and then displays a real-time clock. It demonstrates the use of loops, input validation, and console manipulation for a beginner-friendly project.

---

## Features

- **User Input Validation**: Ensures that the user provides valid time input (hours: 0–23, minutes: 0–59, seconds: 0–59).
- **Real-Time Clock Display**: Updates the clock every second to simulate a real-time clock.
- **Reset Functionality**: Automatically resets seconds, minutes, and hours as needed.

---

## How It Works

1. **Input Phase**:
   - Prompts the user to enter a valid time (hour, minute, and second).
   - Validates the input and clears the console if the input is invalid.

2. **Clock Phase**:
   - Displays the current time in the format `HH:MM:SS`.
   - Updates every second, incrementing seconds, and adjusting minutes and hours when necessary.

---

## Requirements

- **Operating System**: Windows
- **Compiler**: Any C++ compiler that supports C++11 or later.

---

## Setup and Execution

1. Clone the repository:
   ```bash
   git clone https://github.com/Abhianav7255/clock-in-c-
   cd clock-in-c-
   ```

2. Compile the code:
   ```bash
   g++ -o clock clock.cpp
   ```

3. Run the program:
   ```bash
   ./clock
   ```

---

## Code Snippet for Input Validation

```cpp
bool validInput = false;
while (!validInput) {
    cout << "Enter Hour (0-23): ";
    cin >> h;
    cout << "Enter Minute (0-59): ";
    cin >> m;
    cout << "Enter Second (0-59): ";
    cin >> s;

    if (h >= 0 && h < 24 && m >= 0 && m < 60 && s >= 0 && s < 60) {
        validInput = true;
    } else {
        cout << "Invalid time entered. Please try again." << endl;
        Sleep(2000); // Pause for 2 seconds
        clearScreen();
    }
}
```

---

## Future Improvements

- Add cross-platform compatibility by replacing `system("cls")` and `Sleep()` with portable alternatives.
- Implement a GUI version for a more interactive experience.
- Allow the user to set alarms or stop the clock.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contributions

Contributions are welcome! If you find a bug or have suggestions, feel free to open an issue or create a pull request.

---

## Author

**Abhinav**  
GitHub: [https://github.com/Abhianav7255](https://github.com/Abhianav7255)
