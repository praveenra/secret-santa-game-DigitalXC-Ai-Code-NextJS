🎅 **Secret Santa Automator**

An intelligent Secret Santa assignment system built with Next.js and TypeScript. This tool automates the "Secret Child" pairing process while strictly adhering to organizational constraints and historical data.


**🚀 Overview**

This application helps HR or Team Leads manage holiday gift exchanges by automating the pairing process. It uses a modular, OOP-based architecture to handle complex assignment logic.

**⚖️ Assignment Rules**

Self-Exclusion: No employee is ever assigned to themselves.
Historical Variety: No employee is assigned the same Secret Child as the previous year.
Unique Pairs: Every employee receives exactly one unique Secret Child.

**🛠 Features**

CSV Integration: Bulk upload employee lists and historical assignment data.
Validation Engine: Real-time CSV validation to prevent data errors.
One-Click Export: Download the new assignments as a formatted CSV.
Robust Architecture: Built with Next.js (App Router), TypeScript, and OOP principles.
Tested Logic: Comprehensive unit tests for the pairing algorithm.

**📂 CSV Data Formats**

To ensure the logic works correctly, please use the following headers:
1. Current Employees (employees.csv)Employee_NameEmployee_EmailIDJohn Doejohn@example.comJane Smithjane@example.com
2. Previous Year Assignments (past_assignments.csv) - OptionalEmployee_NameEmployee_EmailIDSecret_Child_NameSecret_Child_EmailIDJohn Doejohn@example.comJane Smithjane@example.com
  
**📦 Getting Started**
1. Install Dependencies
  Bash
  
  npm install
  # or
  yarn install
  # or
  pnpm install

2. Run the Development ServerBashnpm 

run dev

Open http://localhost:3000 with your browser to see the result.

**🧪 Running Tests**

We use Jest to ensure the integrity of the Secret Santa algorithm.Bash

npm test

The test suite validates:

[x] Zero self-assignments.
[x] 100% unique pairings across the list.
[x] Successful avoidance of previous year's matches.

**📖 Tech Stack**

Framework: Next.js 14+
Language: TypeScript
Testing: Jest
Styling: Tailwind CSS
