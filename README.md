# Library App

## Description
Library App is a console application designed to manage library operations such as searching for patrons, viewing patron details, managing loans, and renewing memberships. The application uses JSON files to store data and leverages dependency injection for service management.

## Project Structure
- **AccelerateDevGitHubCopilot.sln**: Solution file
- **README.md**: Project documentation
- **src**
  - **Library.ApplicationCore**
    - **Entities**: Contains core entities like `Patron`, `Loan`, `Book`, and `Author`
    - **Enums**: Contains enumerations like `LoanReturnStatus` and `MembershipRenewalStatus`
    - **Interfaces**: Contains interfaces like `IPatronRepository` and `ILoanService`
    - **Services**: Contains service implementations like `LoanService` and `PatronService`
    - **Library.ApplicationCore.csproj**: Project file
  - **Library.Console**
    - **appSettings.json**: Configuration file for JSON paths
    - **CommonActions.cs**: Defines common actions for the console application
    - **ConsoleApp.cs**: Main console application class
    - **ConsoleState.cs**: Defines the states of the console application
    - **Json**: Contains JSON data files like `Patrons.json` and `Loans.json`
    - **Library.Console.csproj**: Project file
    - **Program.cs**: Entry point of the console application
  - **Library.Infrastructure**
    - **Data**: Contains data access classes like `JsonData`, `JsonPatronRepository`, and `JsonLoanRepository`
    - **Library.Infrastructure.csproj**: Project file
- **tests**
  - **UnitTests**
    - **ApplicationCore**
      - **LoanService**: Contains unit tests for `LoanService`
      - **PatronService**: Contains unit tests for `PatronService`
    - **UnitTests.csproj**: Project file

## Key Classes and Interfaces
- **Entities**
  - `Patron`: Represents a library patron
  - `Loan`: Represents a book loan
  - `Book`: Represents a book
  - `Author`: Represents an author
- **Enums**
  - `LoanReturnStatus`: Enum for loan return statuses
  - `MembershipRenewalStatus`: Enum for membership renewal statuses
- **Interfaces**
  - `IPatronRepository`: Interface for patron repository
  - `ILoanRepository`: Interface for loan repository
  - `ILoanService`: Interface for loan service
  - `IPatronService`: Interface for patron service
- **Services**
  - `LoanService`: Implements loan-related operations
  - `PatronService`: Implements patron-related operations
- **Data Access**
  - `JsonData`: Handles loading and saving data from/to JSON files
  - `JsonPatronRepository`: Implements `IPatronRepository` using JSON data
  - `JsonLoanRepository`: Implements `ILoanRepository` using JSON data
- **Console Application**
  - `ConsoleApp`: Main class for the console application
  - `Program`: Entry point of the console application

## Usage
1. Clone the repository.
2. Open the solution file `AccelerateDevGitHubCopilot.sln` in Visual Studio.
3. Build the solution to restore dependencies and compile the projects.
4. Run the console application by starting the `Library.Console` project.
5. Follow the on-screen instructions to search for patrons, view details, manage loans, and renew memberships.

## License
This project is licensed under the MIT License.
