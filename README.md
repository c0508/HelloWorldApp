# Hello World - .NET MVC Training Application

This is a simple "Hello World" application built with ASP.NET Core MVC, designed for training purposes to introduce users to coding and GitHub.

## What is MVC?

**MVC** stands for **Model-View-Controller**, a design pattern that separates an application into three main components:

- **Model**: Represents the data and business logic
- **View**: Displays the data to the user (HTML/CSS)
- **Controller**: Handles user input and coordinates between Model and View

## Project Structure

```
HelloWorldApp/
├── Controllers/          # Controllers handle HTTP requests
│   └── HomeController.cs
├── Views/               # Views contain the HTML/CSS
│   ├── Home/
│   │   └── Index.cshtml
│   └── Shared/
│       └── _Layout.cshtml
├── Models/              # Models represent data
├── wwwroot/             # Static files (CSS, JS, images)
└── Program.cs           # Application entry point
```

## How It Works

1. **User visits the website** → Browser sends HTTP request
2. **Controller receives request** → `HomeController.Index()` method is called
3. **Controller prepares data** → Sets `ViewData["Message"]` to "Hello, World!"
4. **View renders HTML** → `Index.cshtml` displays the message
5. **Response sent to browser** → User sees "Hello, World!"

## Running the Application

### Prerequisites
- .NET SDK (version 9.0 or later)

### Steps

1. **Navigate to the project directory:**
   ```bash
   cd HelloWorldApp
   ```

2. **Restore dependencies:**
   ```bash
   dotnet restore
   ```

3. **Run the application:**
   ```bash
   dotnet run
   ```

4. **Open your browser:**
   - Navigate to `http://localhost:5080`
   - The exact URL will be shown in the terminal

## Key Files Explained

### HomeController.cs
The controller that handles requests to the home page. The `Index()` method is called when someone visits the root URL.

### Index.cshtml
The view that displays the "Hello, World!" message. It receives data from the controller via `ViewData`.

### _Layout.cshtml
The shared layout template that wraps all pages (header, footer, navigation).

## Learning Objectives

After working with this project, you should understand:

- ✅ How MVC applications are structured
- ✅ How controllers pass data to views
- ✅ How to run a .NET application
- ✅ Basic GitHub workflow (clone, commit, push)

## Next Steps

1. Try modifying the message in `HomeController.cs`
2. Change the styling in `Index.cshtml`
3. Add a new controller action and view
4. Practice using GitHub to commit and push changes

## Resources

- [ASP.NET Core Documentation](https://learn.microsoft.com/aspnet/core)
- [MVC Pattern Overview](https://learn.microsoft.com/aspnet/core/mvc/overview)


