```markdown
# Simple WinUI 3 C# GUI Application

## Overview

This project is a simple desktop GUI application built using **C# and WinUI 3**. The application demonstrates the creation of a user interface with multiple interactive controls and event-driven programming.

The application allows users to enter their name, select a course option, confirm an agreement using a checkbox, and submit their information. The program then displays a personalized response based on the user's selections.

This project was created to demonstrate the fundamentals of Windows desktop application development using the WinUI framework.

---

## Features

- User-friendly graphical interface
- Text input handling
- Dropdown selection menu
- Checkbox validation
- Button click event handling
- Dynamic output display
- Basic user input validation

---

## Technologies Used

- **Language:** C#
- **Framework:** WinUI 3
- **Platform:** Windows Desktop
- **IDE:** Visual Studio / JetBrains Rider
- **UI Design:** XAML
- **Version Control:** Git & GitHub

---

## GUI Controls Used

The application includes four unique WinUI controls:

### 1. TextBox

Allows users to enter their name.

Example:

```

Enter your name:
Tyrone

```

---

### 2. ComboBox

Provides a dropdown list where users can select a course.

Available options:

- Computer Science
- Information Technology
- Engineering

---

### 3. CheckBox

Allows users to confirm an agreement before submitting.

Example:

```

☑ I agree to continue

```

---

### 4. Button

Triggers the application logic when clicked.

The button processes the user's input and displays the result.

---

## Application Preview

Example interaction:

```

Enter your name:
Tyrone

Select your course:
Computer Science

☑ I agree to continue

[Submit]

Output:

Hello Tyrone! You selected Computer Science.

```

---

## Project Structure

```

SimpleWinUIApp
│
├── Assets
│
├── SimpleGUI
│   │
│   ├── App.xaml
│   ├── App.xaml.cs
│   ├── MainWindow.xaml
│   ├── MainWindow.xaml.cs
│   └── SimpleWinUIApp.csproj
│
├── SimpleGUI.sln
│
└── .gitignore

````

---

## How It Works

### User Input

The user enters information through the graphical interface:

- Name entered through the TextBox
- Course selected through the ComboBox
- Agreement confirmed through the CheckBox

---

### Button Event

When the Submit button is clicked:

1. The program reads the user's name.
2. The selected course is retrieved.
3. The checkbox status is checked.
4. A message is displayed.

Example:

```csharp
private void Submit_Click(object sender, RoutedEventArgs e)
{
    string name = NameInput.Text;

    string course =
        (CourseSelection.SelectedItem as ComboBoxItem)
        ?.Content.ToString();

    bool accepted = AgreeCheck.IsChecked == true;
}
````

---

## Requirements

Before running the application, ensure you have:

* Windows 10 version 1809 or later
* Windows 11 recommended
* Visual Studio 2022
* .NET SDK installed
* Windows App SDK
* WinUI 3 project templates

---

## Installation

### Clone Repository

Using GitHub Desktop:

1. Open GitHub Desktop
2. Select **File → Clone Repository**
3. Choose this repository
4. Open the `.sln` file

---

### Run Application

1. Open the solution in Visual Studio
2. Restore dependencies if required
3. Build the project

Shortcut:

```
Ctrl + Shift + B
```

4. Run:

```
F5
```

---

## Future Improvements

Possible enhancements:

* Add additional UI themes
* Add database integration
* Store user input
* Improve input validation
* Add animations
* Add navigation between pages

---

## Learning Objectives

This project demonstrates:

* Creating a WinUI 3 desktop application
* Designing interfaces using XAML
* Working with C# event handlers
* Handling user input
* Connecting UI elements with application logic

---

## Author

**Tyrone Darby**

Computer Science Student

---

## License

This project is available for educational purposes.

```

This README will look professional on GitHub and matches a beginner/intermediate WinUI 3 project.
```
