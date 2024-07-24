# EURO 2024 Dispatcher Bot

## Project Description

This UiPath process automates the initial handling of Euro 2024 player data files created by the [EURO 2024](https://github.com/yehiarasheed/EURO-2024) repository. Each file is named after a country and contains a sheet with player details for that country's Euro 2024 team, including player name, team, age, weight, and height.

### Dispatcher Bot Overview

The dispatcher bot takes user input for three country names, validates the existence of corresponding files, logs any invalid entries, and adds valid country names and file paths to a queue. This process sets the stage for the performer bot, which processes these entries efficiently.

### Performer Bot Overview

The performer bot, which runs unattended and is triggered by the queue populated by the dispatcher bot, is located in the [EURO 2024 Performer](https://github.com/yehiarasheed/EURO-2024-Performer) repository.


> [!IMPORTANT]
> All file paths used in the project are relative paths, so any user can clone the project and use it right out of the box. In the `Additional Files` folder, you will find the Excel workbooks containing all the player and team data by country name inside the `Inputs` folder.

## How to Install

### Prerequisites

- UiPath Studio installed.
- Access to the Euro-2024 player data files.
- Microsoft Excel.
- Microsoft Access Database Engine ODBC.

### Steps

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yehiarasheed/EURO-2024-Dispatcher
   cd EURO-2024-Dispatcher
   ```

   **Alternatively, Clone the Repository in UiPath Studio:**
   - Open UiPath Studio.
   - Go to the `Team` tab.
   - Click on `Clone Repository`.
   - Enter the repository URL: `https://github.com/yehiarasheed/EURO-2024-Dispatcher`.
   - Select the destination folder and click `Open` using your authentication method of choice.

2. **Install UiPath Studio:**
   Download and install UiPath Studio from the [official UiPath website](https://www.uipath.com).

3. **Open the Project in UiPath Studio:**
   - Launch UiPath Studio.
   - Click on `Open` in the Start tab.
   - Navigate to the cloned repository folder and open the `.xaml` file.

4. **Install Microsoft Excel:**
   Ensure Microsoft Excel is installed on your computer, as it is required for handling Excel files in this project.

5. **Install Microsoft Access Database Engine ODBC:**
   Download and install the [Microsoft Access Database Engine ODBC](https://www.microsoft.com/en-us/download/details.aspx?id=54920).

6. **Install Necessary Packages in UiPath:**
   - Open UiPath Studio.
   - Go to the `Manage Packages` section.
   - Install `UiPath.Excel.Activities`.
   - Install the `UiPath.Database.Activities` package.

## Dependencies

This project requires the following dependencies:

- **Microsoft Excel**: Required for handling Excel files.
- **UiPath.Excel.Activities**: For interacting with Excel files.
- **UiPath.System.Activities**: For general automation tasks.
- **Microsoft Access Database Engine ODBC**: Required for accessing Excel files via ODBC.
- **UiPath.Database.Activities**: Available in UiPath's Package Manager.

These dependencies can be managed through UiPath Studio's Package Manager. Make sure all required packages are installed and up to date.

---
