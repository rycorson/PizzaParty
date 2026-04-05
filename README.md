# Pizza Party Calculator

## Overview
This native Android application helps users calculate the exact number of pizzas needed for an event. By taking the number of attendees and their hunger levels into account, the app processes these inputs through custom business logic to return an accurate pizza count. It is designed with a clean, user-friendly interface and handles edge cases like invalid user input gracefully.

## Technologies & Libraries
* **Language:** Java
* **Platform:** Android SDK
* **IDE:** Android Studio
* **UI Layout:** XML (LinearLayout)
* **Architecture Pattern:** Model-View-Controller (MVC) principles

## Key Features & Technical Highlights

* **Separation of Concerns:** The application clearly separates the UI and event-handling logic (MainActivity.java) from the core business logic and state management (PizzaCalculator.java), ensuring the code is modular and easy to test.
* **Dynamic Data Calculation:** Utilizes enumerated types (HungerLevel: LIGHT, MEDIUM, RAVENOUS) to map specific slice requirements per person. The logic uses Math.ceil() against a constant of 8 slices per pizza to ensure the final count always rounds up so no one goes hungry.
* **Input Validation & Error Handling:** Implements a try-catch block to handle NumberFormatException errors, preventing the application from crashing if a user submits an empty or invalid string for the attendee count.
* **Resource Management:** Best practices are used for UI text by isolating strings in the res/values/strings.xml file, allowing for easy localization and dynamic string formatting during runtime.

## How to Run Locally

### 1. Prerequisites
Ensure you have Android Studio installed on your machine along with a configured Android Virtual Device (AVD) emulator or a physical Android device connected via USB debugging.

### 2. Installation
Clone the repository and navigate into the project directory:

```bash
git clone https://github.com/rycorson/pizza-party.git
```

### 3. Execution
*You will need an operational Virtual Device in Android Studio to run the program.*

Open Android Studio.

Select File > Open and navigate to the cloned pizza-party directory.

Allow Gradle to sync the project dependencies.

Click the green Run 'app' button (Shift + F10) in the top toolbar to launch the application on your selected emulator or physical device.

## Author
Ryan Corson
* GitHub: @rycorson
* LinkedIn: https://www.linkedin.com/in/ryan-corson/
