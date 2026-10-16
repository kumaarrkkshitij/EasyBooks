# EasyBooks – Bookkeeping System

EasyBooks is a web-based bookkeeping and tax management application designed to help small business owners, freelancers, and entrepreneurs manage their financial records more efficiently. The system simplifies income and expense tracking, automates financial calculations, and generates organized tax reports.

## Features

- **Income Management** – Record, view, update, and delete income transactions.
- **Expense Management** – Track business expenses and organize financial records.
- **Automated Tax Computation** – Calculate Output VAT, Input VAT, and VAT owed for VAT-registered users, with a separate report for non-VAT users.
- **Financial Dashboard** – View income, expenses, and daily financial trends through charts and summary metrics.
- **Date Range Filtering** – Filter transactions and reports by a selected date range.
- **Tax Reports** – Generate financial summaries based on VAT registration status.
- **CSV Export** – Export financial records for further analysis.
- **Secure Authentication** – Manage user accounts through Supabase Authentication.
- **Row-Level Security (RLS)** – Restrict access to financial records based on the authenticated user.

## Tech Stack

- **Framework:** Flutter
- **Language:** Dart
- **Backend and Database:** Supabase, PostgreSQL
- **Authentication:** Supabase Auth
- **Charts:** fl_chart
- **Data Export:** csv, file_saver
- **Development Tools:** Visual Studio Code, Android Studio, Git, GitHub

## System Architecture

EasyBooks uses Flutter for its user interface and Supabase for authentication, database management, and backend services. PostgreSQL functions aggregate daily financial data for charts and reports, while Row-Level Security helps ensure that users can access only their own records.

## Installation and Setup

### Prerequisites

- Flutter SDK
- Dart SDK
- Visual Studio Code or another compatible IDE
- A Supabase project
- Git

### 1. Clone the Repository

```bash
git clone <repository-url>
cd <repository-folder>
```

Replace the placeholders with your repository URL and folder name.

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Configure Supabase

Configure the application with your Supabase project URL and anonymous key. The project uses build-time environment definitions:

```bash
flutter run -d chrome \
  --dart-define=SUPABASE_URL=your_supabase_url \
  --dart-define=SUPABASE_ANON_KEY=your_supabase_anon_key
```

Replace the placeholder values with your own Supabase project credentials. Never commit private service-role keys or other secrets to the repository.

### 4. Run the Application

Run the application in a supported browser using the command above, or build the web version:

```bash
flutter build web \
  --dart-define=SUPABASE_URL=your_supabase_url \
  --dart-define=SUPABASE_ANON_KEY=your_supabase_anon_key
```

The generated web application is available in the `build/web/` directory.

## Project Structure

The application is organized around its core features and services:

- **Authentication** – Handles user sign-in, registration, and session management.
- **Dashboard** – Displays financial summaries and daily income and expense charts.
- **Income and Expenses** – Manages transaction records and related calculations.
- **Tax Reports** – Computes and displays tax-related financial summaries.
- **CSV Export** – Supports exporting records for a selected date range.
- **Supabase Integration** – Handles authentication, database operations, and daily data aggregation.

*Note: The exact directory structure may vary depending on the repository version.*

## Team Contributions

**My Role: Frontend Developer / Documentation Lead**

- Developed responsive frontend components to improve application interactivity.
- Coordinated project workflow and tracked documentation progress.
- Maintained consistency and organization across the project report.

The project was developed collaboratively by the team, with responsibilities spanning frontend development, authentication, backend logic, database integration, and documentation.

## Platform Support

EasyBooks is primarily designed for desktop and laptop web browsers. It uses Philippine Peso (₱) for financial transactions and is intended for individual users and small businesses.

## Future Improvements

Potential enhancements include:

- AI-powered financial insights and forecasting.
- Bank and GCash transaction imports.
- Customizable dashboards.
- Multi-currency support.
- Improved mobile experience and offline synchronization.
- Receipt uploads and automated tax reminders.

**EasyBooks — Simplifying bookkeeping through technology.**
