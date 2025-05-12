# HashBro

SudoCop HashBro is a powerful file hashing utility designed for digital forensics and evidence verification. It allows users to compute cryptographic hash values for files, compare hashes to identify matching files, and generate detailed reports for documentation.
# Features
Core Functionality

Multiple Hash Algorithms: Support for MD5, SHA1, SHA256, SHA384, SHA512, and RIPEMD160
Batch Processing: Hash multiple files or entire folders at once with recursive scanning
Evidence Tagging: Categorize files as "Original" or "Copy" (or custom categories)
Automatic Match Detection: Identify files with matching hash values across all selected algorithms
Timezone Support: Choose between UTC and local time for reports with the "Use UTC Time" checkbox

# Performance & Processing

High Performance: Optimized for speed with:

Parallel processing with dynamic parallelism adjustment
Efficient memory management with buffer pooling
Memory-mapped file support for large files (>100MB)
Special handling for compressed files
Minimal memory mode for extremely large files


# Smart File Handling:

Automatic retry mechanisms for locked files
Shadow copy creation for inaccessible files
Detailed error reporting with specific error types



# User Interface

Drag & Drop Support: Simply drag files or folders onto the application
Flexible UI Modes:

Normal View: Shows all controls and the data grid
Grid Only View: Hides controls and shows only the data grid
Collapsed View: Hides the data grid to save space
Minimal Mode: Shows only progress info for monitoring long operations


Real-time Progress: Live progress updates with:

File count and completion percentage
Processing speed (MB/s)
Elapsed time with millisecond precision
Animated spinner during processing


Console Theme: Dark theme with green text for a professional appearance

Reporting & Export

Comprehensive Reports: Generate detailed reports in multiple formats:

Text: Human-readable reports with structured sections
HTML: Professional reports with case information, match analysis, and digital signatures
CSV: Structured data with metadata headers
JSON: Machine-readable format with complete data structure


Report Features:

Executive summary
Hash match analysis with group identification
Error analysis and problematic files
Complete file hash inventory
Verification statements
Customizable agency and examiner information



# System Requirements

Operating System: Windows 7 or newer
Framework: .NET Framework 4.6.1 or higher
Minimum RAM: 4GB (8GB+ recommended for processing large files)
Processor: Multi-core processor recommended for optimal performance
Storage: SSD recommended for large batch operations

# Installation

Download the latest release from the releases page
Run the setup.exe file
Follow the installation wizard

Usage
Basic Operation

Launch SudoCop HashBro
Select the hash algorithm(s) you want to use (default is SHA256)
Choose evidence type: "Original" or "Copy" (customizable)
Add files using one of these methods:

Click "Select Files" for individual files
Click "Select Folder" for entire directories (recursive)
Drag and drop files or folders directly onto the application


Files will be processed with real-time progress updates
Matching files will be automatically highlighted and marked as "MATCH"

Case Information
Before generating reports, fill in the case details:

Case ID: Unique identifier for your case
Agency: Your organization or department
Examiner: Person conducting the analysis

Evidence Type Customization

Select either "Original" or "Copy" radio button
Click in the adjacent text box to customize the label
Enter your preferred description (e.g., "Suspect Device", "Reference Files")

Timezone Settings

Check "Use UTC Time" for reports with UTC timestamps
Uncheck for local time timestamps
This setting affects all export formats consistently

View Modes

Grid Only: Click "View Grid Only" to hide controls and maximize data view
Collapsed: Click "<<" to hide the data grid and save space
Minimal Mode: Click "Min Mode" during processing to see only progress
Cancel Operations: Click "Cancel" to stop processing at any time

Report Generation

Process the files you want to include
Click "Generate Report"
Select your preferred format:

PDF: Professional reports with formatting
Text: Plain text for easy reading
CSV: Structured data for analysis
JSON: Machine-readable format


Choose destination and filename
Reports include all processed files, hash values, and matches

# Performance Tips

Large Files: The application automatically optimizes for files over 100MB using memory-mapped files
Batch Processing: For thousands of files, ensure adequate RAM (8GB+ recommended)
Algorithm Selection: Using multiple algorithms increases processing time proportionally
Parallel Processing: The application automatically adjusts thread count based on your hardware

# Error Handling
The application provides detailed error reporting:

File Not Found (FNF): Missing or moved files
Access Error (AE): Permission or security issues
IO Error (IOE): General input/output problems
Memory Error (ME): Files too large for available memory

Files with errors are:

Marked with "ERROR" in the grid
Included in the error analysis section of reports
Listed with specific error descriptions

Advanced Features

Memory Management

Intelligent buffer pooling for efficient memory usage
Garbage collection optimization for large file processing
Automatic adjustment of buffer sizes based on file types

File Type Recognition

Special handling for compressed files (.zip, .rar, .7z, etc.)
Optimized processing for different file types
Automatic adjustment of chunk sizes for optimal performance

Technical Details
Supported Hash Algorithms

MD5: 128-bit (fast but cryptographically broken)
SHA1: 160-bit (legacy, not recommended for security)
SHA256: 256-bit (industry standard)
SHA384: 384-bit (stronger variant)
SHA512: 512-bit (strongest variant)
RIPEMD160: 160-bit (alternative algorithm)

Implementation Notes

All hash calculations use single-pass reading for multiple algorithms
Thread-safe implementation with concurrent collections
Automatic retry mechanisms for transient errors

# License
See the EULA file for details.

Note: This tool is designed for legitimate forensic and security analysis purposes. Users are responsible for compliance with applicable laws and regulations.
