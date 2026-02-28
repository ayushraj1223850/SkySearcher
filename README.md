# SkySearcher: Flight Search Engine ✈️

A modern, responsive flight search engine built with **ASP.NET Core (MVC)** and **SQL Server**.

## 🚀 Features
- **Real-Time Search**: Fetch flight results instantly based on source and destination.
- **Flight + Hotel Bundles**: Search for combined packages including luxury stay options.
- **Premium UI**: Modern dark/light modes, animations (Animate.css), and responsive design.
- **Dynamic Data**: Powered by stored procedures for efficient searching.

---

## 🛠️ Setup Instructions

### 1. Prerequisites
- **.NET SDK** (Version 8.0 or later)
- **SQL Server Management Studio (SSMS)**
- **SQL Express** or **LocalDB**

### 2. Database Setup
1. Open SSMS and connect to your local server (e.g., `.\SQLEXPRESS`).
2. Open and execute `Database/schema.sql` to create the `FlightDB` database and tables.
3. Open and execute `Database/stored_procedures.sql` to add the necessary search logic.

### 3. Application Configuration
1. Rename `appsettings.Example.json` to `appsettings.json`.
2. Update the `DefaultConnection` string in `appsettings.json` to point to your specific SQL server instance if it's different from `.\SQLEXPRESS`.

### 4. Run the Project
```bash
dotnet build
dotnet run
```
Open your browser to `http://localhost:5175` (or the port shown in your terminal).

---

## 🏗️ Project Structure
- **/Controllers**: MVC logic for searching and results.
- **/Models**: Search and result data objects.
- **/Views**: Responsive Razor views for the search UI.
- **/Data**: `DatabaseHelper` class for data access.
- **/Database**: SQL scripts for schema and stored procedures.
- **/wwwroot**: Static assets (CSS, images, icons).

---

Developed with ❤️ for a premium flight searching experience.
