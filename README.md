# Invoice PDF Generator

This is a simple console application built with .NET Core that converts UBL (Universal Business Language) XML invoices into printable PDF files.

## Features

- Deserialize UBL XML invoices into C# objects.
- Generate PDF files from the invoice data.
- Simple command-line interface for easy usage.

## Requirements

- .NET Core SDK 6.0 or later
- [iTextSharp.LGPLv2.Core](https://www.nuget.org/packages/iTextSharp.LGPLv2.Core/) - For generating PDF files.

## Installation

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/yourusername/invoice-pdf-generator.git
   cd invoice-pdf-generator

2. Restore the NuGet packages:

   ```bash
   dotnet restore
   
3. Build the project:

   ```bash
    dotnet build
   



## Usage
After building the project, you can run the application from the command line. The application expects two arguments: the path to the XML invoice file and the path where the generated PDF should be saved.

```bash
dotnet run -- /path/to/invoice.xml /path/to/output.pdf
```

For example:

```bash
dotnet run -- ~/Documents/invoice.xml ~/Documents/invoice.pdf
```

## Project Structure

````
InvoiceApp/
│
├── Program.cs                 # Main entry point
├── XmlInvoiceReader.cs        # Handles XML deserialization
├── PdfInvoiceGenerator.cs     # Handles PDF generation
├── Invoice.cs                 # Contains the Invoice and related classes
│
├── InvoiceApp.csproj          # Project file

