# Pizza Restaurant Management System

A desktop pizza ordering application built with C# and Windows Forms. The application provides two ordering paths: customers can create a custom pizza or choose from ready-made pizza options, then review and confirm their order through a dedicated summary screen.

## Overview

Pizza Restaurant Management System is a practical Windows Forms application designed to simulate a simple pizza ordering workflow. It focuses on desktop user interface development, event-driven programming, order configuration, price calculation, and communication between multiple forms.

The project was developed as part of hands-on .NET and C# practice, with an emphasis on Object-Oriented Programming, Windows Forms controls, form navigation, input selection, and structured application logic.

## Features

### Custom Pizza Ordering

- Choose the pizza size: Small, Medium, or Large.
- Select the crust type: Thin or Thick.
- Choose the dining option: Eat In or Take Out.
- Add optional toppings, including extra cheese, tomatoes, mushrooms, olives, onions, and green peppers.
- Calculate the order price according to the selected size, crust, and toppings.
- Reset the order and start again when needed.

### Ready-Made Pizza Ordering

- Choose from available ready-made pizza types, including Cheese Pizza and Vegetable Pizza.
- Select the available size for each pizza type.
- Calculate the total price automatically based on the selected options.

### Order Review and Confirmation

- Display the selected pizza details in an order summary.
- Review the pizza type, size, crust, toppings, dining option, and total price.
- Cancel the order and return to the previous ordering screen.
- Confirm the order through a confirmation dialog.

### User Interface

- Multi-form Windows Forms interface.
- Interactive radio buttons and checkboxes for selecting order options.
- Visual feedback for selected controls.
- Styled buttons and dialogs using Guna UI2 WinForms.
- Application navigation through welcome, pizza type, custom order, ready-made order, and summary forms.

## Technologies Used

- C#
- .NET 6.0 for Windows
- Windows Forms
- Guna UI2 WinForms
- Object-Oriented Programming
- Event-Driven Programming
- Visual Studio

## Application Flow

```text
Main Screen
    |
    v
Choose Ordering Method
    |-----------------------------|
    v                             v
Custom Pizza                 Ready-Made Pizza
    |                             |
    v                             v
Select size, crust,       Select pizza type and size
 toppings, and dining option       |
    |                             |
    |-------------|---------------|
                  v
           Order Summary
                  |
                  v
        Confirm or Cancel Order
```

## Project Structure

```text
Pizza-Restaurant-Management-System/
├── WinFormsApp2.sln
└── WinFormsApp2/
    ├── Program.cs
    ├── MainForm.cs
    ├── TypeOrderPizza.cs
    ├── Form1.cs
    ├── Form2.cs
    ├── OrderSummary.cs
    ├── Properties/
    └── Resources/
```

### Main Forms

| Form | Responsibility |
|---|---|
| `MainForm` | Displays the welcome screen and starts the ordering process. |
| `TypeOrderPizza` | Allows the user to choose between custom and ready-made pizza. |
| `Form1` | Handles custom pizza configuration, toppings, crust, dining option, and price calculation. |
| `Form2` | Handles ready-made pizza selection, sizes, and price calculation. |
| `OrderSummary` | Displays the order details and handles confirmation or cancellation. |

## Requirements

- Windows operating system.
- Visual Studio 2022 or a compatible .NET development environment.
- .NET 6 SDK with Windows Desktop development support.
- Internet access may be required to restore the `Guna.UI2.WinForms` NuGet package during the first build.

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/AbdulSalamalQadi/Pizza-Restaurant-Management-System.git
cd Pizza-Restaurant-Management-System
```

### Open the Project

Open `WinFormsApp2.sln` in Visual Studio.

### Restore Dependencies

Restore the NuGet packages from Visual Studio, or build the solution and allow the required packages to be restored automatically.

### Run the Application

Select the `WinFormsApp2` project as the startup project and press `F5`, or use **Debug > Start Without Debugging**.

## How to Use

1. Launch the application from the welcome screen.
2. Choose whether to make a custom pizza or select a ready-made pizza.
3. Select the available pizza options.
4. Review the calculated price and order details.
5. Open the order summary.
6. Confirm the order or cancel it and return to the previous screen.

## Current Scope

The current version focuses on the desktop ordering experience and in-memory order calculations. It does not currently include user authentication, online payment, persistent order storage, or a database-backed administration panel.

## Possible Future Improvements

- Add SQL Server database integration for products, orders, customers, and prices.
- Add customer and employee authentication.
- Add an administration dashboard for managing pizzas, toppings, and prices.
- Add order history and persistent storage.
- Add more pizza types, sizes, crusts, and toppings.
- Add input validation and automated tests.
- Improve separation between the user interface, business logic, and data access layers.

## Author

**Abdul Salam Ismail Al-Qadi**

.NET Developer focused on C#, Windows Forms, practical application development, and database integration.

- GitHub: [AbdulSalamalQadi](https://github.com/AbdulSalamalQadi)
- LinkedIn: [Abdul Salam Ismail Al-Qadi](https://www.linkedin.com/in/abdul-salam-ismail-al-qadi-949909366/)

## License

This project is available for educational and portfolio purposes. Add a specific license file if you decide to distribute or reuse the project publicly.
