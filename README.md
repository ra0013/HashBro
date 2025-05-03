# SudoCop HashBro

SudoCop HashBro is a powerful file hashing utility designed for digital forensics and evidence verification. It allows users to compute cryptographic hash values for files, compare hashes to identify matching files, and generate detailed reports for documentation.

## Features

- **Multiple Hash Algorithms**: Support for MD5, SHA1, SHA256, SHA384, SHA512, and RIPEMD160
- **Batch Processing**: Hash multiple files or entire folders at once
- **Evidence Tagging**: Categorize files as "Original" or "Copy" (or custom categories)
- **Automatic Match Detection**: Identify files with matching hash values
- **High Performance**: Optimized for speed with parallel processing and efficient memory management
- **Drag & Drop Support**: Simply drag files or folders onto the application
- **Comprehensive Reports**: Generate detailed reports in various formats (PDF, Text, CSV, JSON)
- **Flexible UI**: Multiple view modes including normal, grid-only, collapsed, and minimal mode

## System Requirements

- **Operating System**: Windows 7 or newer
- **Framework**: .NET Framework 4.6.1 or higher
- **Minimum RAM**: 4GB (8GB+ recommended for processing large files)
- **Processor**: Multi-core processor recommended

## Installation

1. Download the latest release from the releases page
2. Extract the ZIP file to your preferred location
3. Run setup.exe

## Usage

### Basic Operation

1. Launch SudoCop HashBro
2. Select the hash algorithm(s) you want to use (default is SHA256)
3. Choose whether files are "Original" or "Copy" evidence
4. Click "Select Files" or "Select Folder" to add files for hashing
5. Alternatively, drag and drop files or folders directly onto the application
6. Files will be processed, and hash values will be displayed in the grid
7. Matching files will be automatically highlighted and marked as "MATCH"

### Customizing Evidence Types

You can customize the evidence type labels:
1. Click in the text box next to the "Original" or "Copy" radio buttons
2. Enter your preferred label (e.g., "Suspect Device", "Reference Files")

### Generating Reports

1. Process the files you want to include in the report
2. Click "Generate Report"
3. Select the report format (PDF, Text, CSV, or JSON)
4. Choose the destination and filename
5. The report will include file details, hash values, and any matches found

### UI Modes

- **Normal View**: Shows all controls and the data grid
- **Grid Only View**: Hides controls and shows only the data grid (click "View Grid Only"/"Show Controls")
- **Collapsed View**: Hides the data grid to save space (click the "<<" button)
- **Minimal Mode**: Shows only the progress bar for monitoring long operations (click "Min Mode")

## Performance Tips

- For very large files (>2GB), the application will automatically adjust processing settings
- When processing thousands of files, consider using a 64-bit system with 8GB+ RAM
- SSD storage will significantly improve performance for large batches

## Error Handling

The application detects and reports various error types:
- File not found errors
- Access denied errors
- I/O errors
- Memory errors for extremely large files

Files with errors are marked with "ERROR" in the status column and included in the error section of reports.

## License

