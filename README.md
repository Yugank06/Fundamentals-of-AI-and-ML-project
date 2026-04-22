# Basic Subscription Manager (List Version)

## Overview of the Project

The **Basic Subscription Manager** is a simple command-line Python application designed to help users track their monthly subscriptions and calculate total spending. Users can input multiple subscription names and costs, and the program automatically calculates and displays the total monthly expenditure. This project demonstrates fundamental Python programming concepts including user input validation, list manipulation, loops, and error handling.

## Features

- **Interactive Subscription Entry**: Add multiple subscriptions with custom names and costs through an intuitive command-line interface
- **Input Validation**: Robust error handling ensures users enter valid numeric values for costs
- **Negative Value Protection**: Prevents entry of negative subscription costs
- **Dynamic List Management**: Subscriptions are stored in a list structure for easy manipulation
- **Real-time Feedback**: Confirmation messages display after each subscription is added
- **Automatic Cost Calculation**: Automatically computes and displays the total monthly subscription cost
- **Clean Formatted Output**: Well-organized display of all subscriptions with individual and total costs
- **Exit Control**: Simple 'done' command to finish adding subscriptions

## Technologies/Tools Used

- **Programming Language**: Python 3.x
- **Core Python Concepts**:
  - Lists and nested lists for data storage
  - While loops for continuous input
  - Try-except blocks for error handling
  - String methods (`.strip()`, `.lower()`)
  - Input validation and type casting
  - Formatted string output (f-strings)

## Steps to Install & Run the Project

### Prerequisites
- Python 3.6 or higher installed on your system
- Command-line terminal or IDE with Python support

### Installation Steps

1. **Verify Python Installation**
   ```bash
   python --version
   ```
   or
   ```bash
   python3 --version
   ```

2. **Download the Project**
   - Save the `subscription_manager.py` file to your desired directory

3. **Navigate to Project Directory**
   ```bash
   cd path/to/your/project
   ```

### Running the Application

**Method 1: Using Terminal/Command Prompt**
```bash
python subscription_manager.py
```

**Method 2: Using Python 3 Command**
```bash
python3 subscription_manager.py
```

**Method 3: Using an IDE**
- Open `subscription_manager.py` in your preferred Python IDE (VS Code, PyCharm, IDLE)
- Click the "Run" button or press F5

## Instructions for Testing

### Test Case 1: Normal Subscription Entry
1. Run the program
2. Enter subscription name: `Netflix`
3. Enter cost: `9.99`
4. Enter subscription name: `Spotify`
5. Enter cost: `4.99`
6. Enter subscription name: `done`

**Expected Output:**
```
Total Monthly Cost: $14.98
```

### Test Case 2: Input Validation - Invalid Cost
1. Run the program
2. Enter subscription name: `Amazon Prime`
3. Enter cost: `abc` (invalid input)
4. Program should display error and prompt again
5. Enter cost: `15.99` (valid input)
6. Verify subscription is added successfully

### Test Case 3: Negative Cost Prevention
1. Run the program
2. Enter subscription name: `YouTube Premium`
3. Enter cost: `-10.00`
4. Program should display error about negative values
5. Enter cost: `12.99` (valid input)
6. Verify subscription is added successfully

### Test Case 4: Empty Subscription List
1. Run the program
2. Immediately enter: `done`

**Expected Output:**
```
No subscriptions were entered.
```

### Test Case 5: Multiple Subscriptions with Decimal Values
1. Run the program
2. Add 5+ subscriptions with various decimal costs
3. Verify each is displayed correctly
4. Check that total calculation is accurate

### Test Case 6: Edge Cases
- Test with cost `0` (should accept)
- Test with very large numbers (e.g., `9999.99`)
- Test with single subscription
- Test with names containing spaces and special characters

## Screenshots (Optional but Recommended)

### Example Session:
```
 Welcome to your Basic Subscription Manager (List Version)! 
Enter 'done' for the subscription name when finished adding.
---------------------------------------------
Enter subscription name (or 'done'): Netflix
Enter cost for 'Netflix' (e.g., 9.99): $9.99
Added: Netflix ($9.99)

Enter subscription name (or 'done'): Spotify
Enter cost for 'Spotify' (e.g., 9.99): $4.99
Added: Spotify ($4.99)

Enter subscription name (or 'done'): done

=============================================
 Your Subscriptions:
- Netflix: $9.99
- Spotify: $4.99
---------------------------------------------
 Total Monthly Cost: $14.98
=============================================
```

---

## Project Structure

```
subscription-manager/
│
├── subscription_manager.py    # Main program file
├── README.md                   # This file
└── statement.md               # Project statement document
```

## Future Enhancements

- Save subscriptions to a file for persistence
- Edit or delete existing subscriptions
- Monthly/yearly cost breakdown
- Category-based organization
- Export data to CSV format
- Subscription renewal date tracking

## Author

VIT Bhopal Student Project

## License

This project is created for educational purposes as part of coursework at VIT Bhopal.
