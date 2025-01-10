# Tip Calculator Android App

A simple Android application that calculates tips for a given bill amount using both standard (15%) and custom tip percentages. 

## Repository

GitHub: [Tip Calculator Android App](https://github.com/AbidKhan01ak/Tip-calculator-Android-App)

## Features

- Calculate a 15% tip automatically.
- Adjust the tip percentage using a slider for custom calculations.
- Displays formatted output for the tip amount and total bill using currency and percentage formats.

## Code Overview

### `MainActivity.java`

#### Imports

- **`java.text.NumberFormat`**: Used for formatting numbers as currency and percentages.
- **Android Imports**: 
  - `Activity`: Base class for the activity.
  - `Bundle`: To save state information.
  - `EditText`: For user input of the bill amount.
  - `SeekBar`: To adjust custom tip percentages dynamically.
  - `TextView`: To display results.

#### Class: `MainActivity`

This is the main activity of the app that calculates tips and handles user interactions.

- **`currencyFormat`**: Formats numbers as currency (e.g., `$12.34`).
- **`percentFormat`**: Formats numbers as percentages (e.g., `15%`).

#### Variables

- **`billAmount`**: Holds the bill amount entered by the user.
- **`customPercent`**: Stores the custom tip percentage, initialized to `18%`.
- Various `TextView` objects to display the bill amount, tip amounts, and total amounts for both standard and custom percentages.

#### Methods

1. **`onCreate`**
   - Initializes the activity, binds UI elements, and sets up listeners for user interactions.
   - Calls `updateStandard()` and `updateCustom()` to update the tip amounts and totals based on initial values.

2. **`updateStandard`**
   - Calculates and displays the 15% tip and total bill.

3. **`updateCustom`**
   - Calculates and displays the custom tip and total bill based on the slider position.

4. **SeekBar Listener**
   - Updates the `customPercent` when the SeekBar is adjusted.
   - Calls `updateCustom()` to refresh the display with new calculations.

5. **TextWatcher for `EditText`**
   - Monitors changes in the bill amount input.
   - Parses the input, updates `billAmount`, and refreshes the tip calculations.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/AbidKhan01ak/Tip-calculator-Android-App.git
    ```

2. Open the project in Android Studio:
   - Launch Android Studio.
   - Select **"Open an Existing Project"**.
   - Navigate to the cloned repository folder and select it.

3. Build the project:
   - Click on **Build** in the top menu.
   - Select **Make Project** to compile the source code.

4. Run the app:
   - Connect an Android device or start an emulator.
   - Click the **Run** button or select **Run > Run 'app'** from the menu.

5. Test the app:
   - Enter a bill amount in the input field.
   - View the calculated 15% tip and total amount.
   - Adjust the custom tip percentage using the slider to see real-time updates.
   
## Dependencies

- **Android SDK**: Required for building and running the app.
- **Java JDK**: Ensure a compatible Java Development Kit is installed.
- **Gradle**: Dependency management and build tool, included with Android Studio.
- **Android Studio**: IDE for Android app development.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, reach out to:

- **Developer**: [Abid Khan](https://github.com/AbidKhan01ak)  
- **GitHub**: [AbidKhan01ak](https://github.com/AbidKhan01ak)  
- **LinkedIn**: [Abid Khan](https://linkedin.com/in/abidkhan01ak)

